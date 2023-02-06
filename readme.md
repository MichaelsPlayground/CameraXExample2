# CameraX example

Tutorial: https://akhilbattula.medium.com/android-camerax-java-example-aeee884f9102

Source: https://github.com/akhilbattula/android-camerax-java

working !

Tested on Android 8: Environment.getExternalStorageDirectory() is working, an image is stored there

Tested on Android 13: Environment.getExternalStorageDirectory() is NOT working (permiision issue ?), 
usage of getFilesDir() (internal storage is working as a simple workaround)

AndroidManifest:
```plaintext
    <uses-permission android:name="android.permission.CAMERA" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
```

Gradle:
```plaintext
    def camerax_version = "1.1.0"
    implementation "androidx.camera:camera-camera2:$camerax_version"
    implementation "androidx.camera:camera-lifecycle:$camerax_version"
    implementation "androidx.camera:camera-view:$camerax_version"
```