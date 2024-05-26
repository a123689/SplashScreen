# SplashScreen
1.Trong tệp build.gradle, hãy thay đổi compileSdkVersion và đưa thư viện khả năng tương thích SplashScreen vào các phần phụ thuộc.

build.gradle

android {
   compileSdkVersion 31
}

dependencies {
   implementation 'androidx.core:core-splashscreen:1.0.0-beta02'
}


2. Tạo một giao diện có thành phần mẹ của Theme.SplashScreen
   <style name="Theme.App.Starting" parent="Theme.SplashScreen">
   <!-- Set the splash screen background, animated icon, and animation
   duration. -->
   <item name="windowSplashScreenBackground">@color/...</item>

   <!-- Use windowSplashScreenAnimatedIcon to add a drawable or an animated
        drawable. One of these is required. -->
   <item name="windowSplashScreenAnimatedIcon">@drawable/...</item>
   <!-- Required for animated icons. -->
   <item name="windowSplashScreenAnimationDuration">200</item>

   <!-- Set the theme of the Activity that directly follows your splash
   screen. This is required. -->
   <item name="postSplashScreenTheme">@style/Theme.App</item>
</style>
