#  Drawing-Android-App

###  **Technology:** Java (Android Development)
###  **Platform:** Android

---

##  Project Overview

The **Drawing-Android-App** is a simple yet robust mobile application developed in **Java** that allows users to create freehand drawings directly on their Android devices. This project serves as a clear demonstration of core Android development skills, specifically mastering the **Canvas** and **Paint** APIs for graphical rendering.

It provides an intuitive interface for drawing, making it an excellent foundation for more complex graphical editors or note-taking applications.

##  Technical Features & Implementation

The application is built entirely using native Android components and Java programming, focusing on efficiency and responsiveness for a smooth drawing experience.

### 1. Canvas and Paint Architecture

*   **Custom View:** Implements a custom `View` component to override the `onDraw()` method, creating a dedicated drawing surface (the Canvas).
*   **Touch Handling:** Utilizes the `onTouchEvent()` listener to accurately capture user input, translating screen coordinates (X, Y) into smooth drawing strokes.
*   **Path Tracking:** Employs the `Path` object to store and represent the sequence of points for each stroke, ensuring lines are drawn correctly as a continuous movement rather than individual dots.
*   **Styling (Paint Object):** Manages the visual properties of the strokes using the `Paint` object, allowing for dynamic control over color, stroke width, and smoothness (anti-aliasing).

### 2. Core Functionality

*   **Freehand Drawing:** Allows users to draw fluid lines using touch or stylus input.
*   **Color Selection:** Provides a mechanism (e.g., color picker or button options) to easily change the brush color.
*   **Stroke Width Control:** Enables users to adjust the thickness of the drawing line (brush size).
*   **Erasing Capability:** Implements an "eraser" function by setting the brush color to match the canvas background or using specific blending modes.
*   **Undo/Redo (Potential):** Designed with an architecture that can be easily extended to implement full undo/redo functionality by maintaining a history stack of the `Path` objects.

##  Future Enhancements

*   **Persistence:** Implement features to save the drawing as an image file (e.g., JPEG or PNG) to the device's storage.
*   **Shape Tools:** Add options for drawing predefined shapes like circles, rectangles, and lines.
*   **Palette:** Introduce a more advanced, customizable color palette or HSB/RGB selection tool.

##  Getting Started

### Prerequisites

*   Android Studio
*   Android SDK (Target API Level 21+)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/SdIlias/Drawing-Android-App.git
    ```
2.  **Open in Android Studio:**
    Open the cloned directory as a new Android Studio project.
3.  **Build and Run:**
    Sync the Gradle files and run the application on an Android Emulator or a physical device.

---

## 📂 Project Structure

The project follows a standard Android application structure:

```
Drawing-Android-App/
├── app/                  # Main application module
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com.example.drawingapp/ # Your Java source code
│   │   │   │       └── ...
│   │   │   └── res/      # Resources (layouts, drawables, etc.)
│   └── build.gradle      # Module-level Gradle configuration
├── .gitignore
├── build.gradle          # Top-level Gradle configuration
└── settings.gradle       # Defines project modules
```
