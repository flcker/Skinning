cmake_minimum_required(VERSION 3.4.1)

add_library( # Sets the name of the library.
             pvr_core

             # Sets the library as a shared library.
             STATIC

             # Provides a relative path to your source file(s).
             src/main/cpp/PVRCore/AndroidAssetStream.cpp
             src/main/cpp/PVRCore/BufferStream.cpp
             src/main/cpp/PVRCore/ConsoleMessenger.cpp
             src/main/cpp/PVRCore/FilePath.cpp
             src/main/cpp/PVRCore/FileStream.cpp
             src/main/cpp/PVRCore/FileWrapStream.cpp
             src/main/cpp/PVRCore/Log.cpp
             src/main/cpp/PVRCore/NativeLibrary.cpp
             src/main/cpp/PVRCore/StringFunctions.cpp
             src/main/cpp/PVRCore/Time.cpp
             src/main/cpp/PVRCore/UnicodeConverter.cpp )

add_compile_options( -DPUGIXML_NO_EXCEPTIONS )

target_link_libraries( # Specifies the target library.
                       pvr_core

                       # Links the target library to the log library
                       )