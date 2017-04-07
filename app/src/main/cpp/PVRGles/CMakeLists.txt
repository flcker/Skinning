cmake_minimum_required(VERSION 3.4.1)

add_library( # Sets the name of the library.
             pvr_gles

             # Sets the library as a shared library.
             STATIC

             # Provides a relative path to your source file(s).
             src/main/cpp/PVRGles/EffectApi_2.cpp
             src/main/cpp/PVRGles/RenderManager.cpp
             src/main/cpp/PVRGles/OGLES/ApiCommandsGles.cpp
             src/main/cpp/PVRGles/OGLES/CommandBufferGles.cpp
             src/main/cpp/PVRGles/OGLES/ContextGles.cpp
             src/main/cpp/PVRGles/OGLES/FboGles.cpp
             src/main/cpp/PVRGles/OGLES/PipelineConfigStateCreateParam.cpp
             src/main/cpp/PVRGles/OGLES/RenderPassGles.cpp
             src/main/cpp/PVRGles/OGLES/Sync.cpp
             src/main/cpp/PVRGles/OGLES/AssetStore.cpp
             src/main/cpp/PVRGles/OGLES/CommandPoolGles.cpp
             src/main/cpp/PVRGles/OGLES/DescriptorSetGles.cpp
             src/main/cpp/PVRGles/OGLES/GpuCapabilities.cpp
             src/main/cpp/PVRGles/OGLES/PipelineConfigStates.cpp
             src/main/cpp/PVRGles/OGLES/SamplerGles.cpp
             src/main/cpp/PVRGles/OGLES/TextureGles.cpp
             src/main/cpp/PVRGles/OGLES/BufferGles.cpp
             src/main/cpp/PVRGles/OGLES/ComputePipelineGles.cpp
             src/main/cpp/PVRGles/OGLES/EffectApi.cpp
             src/main/cpp/PVRGles/OGLES/GraphicsPipelineGles.cpp
             src/main/cpp/PVRGles/OGLES/PipelineLayoutGles.cpp
             src/main/cpp/PVRGles/OGLES/ShaderGles.cpp
             src/main/cpp/PVRGles/OGLES/TextureUtilsGles.cpp )

target_link_libraries( # Specifies the target library.
                       pvr_gles

                       # Links the target library to the log library
                       pvr_egl pvr_assets pvr_core)