cmake_minimum_required(VERSION 3.4.1)

add_library( # Sets the name of the library.
             pvr_ui_renderer

             # Sets the library as a shared library.
             STATIC

             # Provides a relative path to your source file(s).
             src/main/cpp/PVRUIRenderer/Sprite.cpp
             src/main/cpp/PVRUIRenderer/UIRenderer.cpp )

target_link_libraries( # Specifies the target library.
                       pvr_ui_renderer

                       # Links the target library to the log library
                       pvr_gles pvr_core)