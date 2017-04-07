cmake_minimum_required(VERSION 3.4.1)

add_library( # Sets the name of the library.
             pvr_shell

             # Sets the library as a shared library.
             STATIC

             # Provides a relative path to your source file(s).
             src/main/cpp/PVRShell/CommandLine.cpp
             src/main/cpp/PVRShell/Shell.cpp
             src/main/cpp/PVRShell/StateMachine.cpp
             src/main/cpp/PVRShell/OS/Android/ShellOS.cpp
             src/main/cpp/PVRShell/EntryPoint/android_main/main.cpp )

target_link_libraries( # Specifies the target library.
                       pvr_shell

                       # Links the target library to the log library
                       android_native_app_glue pvr_egl pvr_core)