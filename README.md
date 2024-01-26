## Reproducer JdkImageWorkaround using jdk 17 and toolchains java >= 20
1. Set jdk 17
2. Execute `./gradlew assembleDebug`

Output:
```
Could not resolve all files for configuration ':app:androidJdkImage'.
> Failed to transform core-for-system-modules.jar to match attributes {artifactType=_internal_android_jdk_image_extracted, org.gradle.libraryelements=jar, org.gradle.usage=java-runtime}.
  > Execution failed for ExtractJdkImageTransform: /Users/kio/.gradle/caches/transforms-3/31c03c19ffa2efbfdca13ab345c3e937/transformed/output.
    > Unsupported major.minor version 64.0

```
Build Scan: https://ge.solutions-team.gradle.com/s/xxfvpjobrydpc
