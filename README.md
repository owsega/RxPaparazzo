RxJava extension for Android to take photos using the camera, select files or photos from the device and optionally crop or rotate any selected images.

# RxPaparazzo

This is purely a clone of [RxPaparazzo](https://github.com/miguelbcr/RxPaparazzo) with the [dimanych's pull request](https://github.com/miguelbcr/RxPaparazzo/pull/97) merged in.

Please refer to the original project or the pull request for details on general usage.
However, to switch the default camera mode to the front camera you can do something like
```java
RxPaparazzo.single(activity)
        .setCameraMode(CameraMode.FRONT)
        .usingCamera()
```
More details on that are in [dimanych's repo](https://github.com/dimanych/RxPaparazzo)

# Usage
There is a jitpack release for this patched repo but you'd have to use
```gradle
     implementation "com.github.owsega:RxPaparazzo:0.6.2-alpha"
```
instead of
```gradle
    compile "com.github.miguelbcr:RxPaparazzo:0.6.1-2.x"
```
