# camerax

Custom CameraX module based on PictureSelector camerax, updated to AndroidX CameraX 1.4.2.

## Usage

Add JitPack:

```kotlin
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()
        maven("https://jitpack.io")
    }
}
```

Add dependency:

```kotlin
implementation("com.github.Frank97129:camerax:v3.11.3-camera1.4.2")
```

## v3.11.3-camera1.4.2

- Fix a null `Display` crash in `CustomCameraView.DisplayListener.onDisplayChanged()` when the preview detaches or loses its display.
- Observe display changes only while the preview is attached. Stop observing on detach or destruction, and restore the current rotation on reattach.
- Keep AndroidX CameraX at 1.4.2.
