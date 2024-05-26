# SplashScreen
1.Trong tệp build.gradle, hãy thay đổi compileSdkVersion và đưa thư viện khả năng tương thích SplashScreen vào các phần phụ thuộc.

build.gradle

android {
   compileSdkVersion 31
}

dependencies {
   implementation 'androidx.core:core-splashscreen:1.0.0-beta02'
}
