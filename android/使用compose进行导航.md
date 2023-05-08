# 使用compose进行导航
须在build.gradle(:app)/dependencies中添加
```kotlin
dependencies {
    def nav_version = "2.5.3"
    implementation "androidx.navigation:navigation-compose:$nav_version"
}
