# Generated from jar.pro.

qt_get_android_sdk_jar_for_api("android-16" android_sdk)

set(java_sources
    src/org/qtproject/qt/android/gamepad/QtGamepad.java
)

qt_internal_add_jar(QtAndroidGamepad
    INCLUDE_JARS ${android_sdk}
    SOURCES ${java_sources}
    OUTPUT_DIR "${QT_BUILD_DIR}/jar"
)

install_jar(QtAndroidGamepad
    DESTINATION jar
    COMPONENT Devel
)

