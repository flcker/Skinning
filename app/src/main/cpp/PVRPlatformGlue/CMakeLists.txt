cmake_minimum_required(VERSION 3.4.1)

add_library( # Sets the name of the library.
             pvr_egl

             # Sets the library as a shared library.
             STATIC

             # Provides a relative path to your source file(s).
             src/main/cpp/PVRPlatformGlue/EGL/EglPlatformContext.cpp
             src/main/cpp/PVRPlatformGlue/EGL/ExtensionLoaderEgl.cpp
             src/main/cpp/PVRPlatformGlue/EGL/NativeLibraryEgl.cpp )

target_link_libraries( # Specifies the target library.
                       pvr_egl

                       # Links the target library to the log library
                       pvr_core)