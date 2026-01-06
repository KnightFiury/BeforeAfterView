[![](https://jitpack.io/v/KnightFiury/BeforeAfterView.svg)](https://jitpack.io/#KnightFiury/BeforeAfterView)

# BeforeAfterView

A lightweight Android custom view to display **before and after images with a slider**. Perfect for image comparisons in apps.

![BeforeAfterView Example](https://raw.githubusercontent.com/KnightFiury/BeforeAfterView/refs/heads/main/sample.gif)

---

## Features

- Slide between **before** and **after** images
- Fully **customizable via XML attributes**
- Lightweight, dependency-free
- Works on **Android API 21+**

---

## Installation

### **Using JitPack**

1. Add JitPack to your project-level `build.gradle`:

```gradle
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
```

2. Add the dependency to your app-level `build.gradle`:


```gradle
dependencies {
    implementation 'com.github.KnightFiury:BeforeAfterView:1.0.0'
}
```

## Usage

### XML Layout

```xml
<com.knightfiury.slidable.BeforeAfterView
    android:id="@+id/square"
    android:layout_width="match_parent"
    android:layout_height="300dp"
    app:beforeImage="@drawable/before"
    app:afterImage="@drawable/after"
    app:sliderPosition="0.5"
    app:dividerColor="@android:color/white"
    app:dividerWidth="2dp"
    app:knobColor="@android:color/white" 
    app:knobRadius="8dp"
    app:initialPosition="0.5"/>

<com.knightfiury.slidable.CircularBeforeAfterView
    android:id="@+id/circle"
    android:layout_width="match_parent"
    android:layout_height="300dp"
    app:beforeImage="@drawable/before"
    app:afterImage="@drawable/after"
    app:sliderPosition="0.5"
    app:dividerColor="@android:color/white"
    app:dividerWidth="2dp"
    app:knobColor="@android:color/white" 
    app:knobRadius="8dp"
    app:initialPosition="0.5"/>
```

### Attribute Set 
| Element | Usage |
|---------|-------|
| `app:beforeImage` | Sets the image that appears on the left (before) side of the slider. |
| `app:afterImage` | Sets the image that appears on the right (after) side of the slider. |
| `app:dividerColor` | Changes the color of the dividing line between the two images. |
| `app:dividerWidth` | Sets the thickness of the dividing line. |
| `app:knobColor` | Defines the color of the movable knob/handle. |
| `app:knobRadius` | Sets the radius (size) of the knob. |
| `app:initialPosition` | Determines the starting position of the knob (value between 0 and 1). |
