# Android Camera


### Instructions for running the application source code
Add ***maven {}*** and ***mavenCentral()*** into file ***build.gradle*** project

```
allprojects {
    repositories {
        mavenCentral()
        .....
        .....
        maven { url 'https://jitpack.io' }
    }
}
```

Import library into file ***build.gradle*** module: app 

```
dependencies {
    .....
    implementation 'com.jakewharton:butterknife:8.8.1'

    implementation 'com.theartofdev.edmodo:android-image-cropper:2.7.+'
    implementation 'com.github.jkwiecien:EasyImage:1.3.1'
    implementation 'com.github.bumptech.glide:glide:4.7.1'

    annotationProcessor 'com.jakewharton:butterknife-compiler:8.8.1'
    annotationProcessor 'com.github.bumptech.glide:compiler:4.7.1'
}
```
Add permission into file ***AndroidManifest.xml***

```
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
```

Last, add activity ***CropImageActivity*** into file ***AndroidManifest.xml***

```
<application
       ......
        android:theme="@style/AppTheme">
        ......
        <activity android:name="com.theartofdev.edmodo.cropper.CropImageActivity"
            android:theme="@style/Base.Theme.AppCompat"/>
            
    </application>
```

## Author

Akbar Pambudi Utomo

Don't forget to follow and give me ★
# AndroidCamera
