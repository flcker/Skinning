cmake_minimum_required(VERSION 3.4.1)

add_library( # Sets the name of the library.
             pvr_native_gles


             # Sets the library as a shared library.
             STATIC

             # Provides a relative path to your source file(s).
             src/main/cpp/PVRNativeGles/OGLES/ApiErrors.cpp
             src/main/cpp/PVRNativeGles/OGLES/BufferUtilsGles.cpp
             src/main/cpp/PVRNativeGles/OGLES/ConvertToApiTypes.cpp
             src/main/cpp/PVRNativeGles/OGLES/ExtensionLoaderGles.cpp
             src/main/cpp/PVRNativeGles/OGLES/LibraryLoaderGles.cpp
             src/main/cpp/PVRNativeGles/OGLES/ShaderUtils.cpp
             src/main/cpp/PVRNativeGles/OGLES/TextureUtils.cpp )

target_link_libraries( # Specifies the target library.
                       pvr_egl

                       # Links the target library to the log library
                       pvr_egl pvr_assets pvr_core)