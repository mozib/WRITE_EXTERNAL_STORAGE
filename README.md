# WRITE_EXTERNAL_STORAGE
 Element uses-permission#android.permission.WRITE_EXTERNAL_STORAGE at AndroidManifest.xml:42:5-108 duplicated with element declared at AndroidManifest.xml:36:5-81


 Solution:

 Step 1 : Open Plugin folder -> cordova -plugin-camera-> plugin.xml

 find this part 
    <config-file target="AndroidManifest.xml" parent="/*">
            <!-- <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" android:maxSdkVersion="32" /> -->
            <uses-permission android:name="android.permission.READ_MEDIA_IMAGES" />
            <uses-permission android:name="android.permission.READ_MEDIA_VIDEO" />
        </config-file>

  Comment that part

  Step 2 : ionic cordova build android 

  
