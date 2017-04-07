cmake_minimum_required(VERSION 3.4.1)

add_library( # Sets the name of the library.
             pvr_assets

             # Sets the library as a shared library.
             STATIC

             # Provides a relative path to your source file(s).
             src/main/cpp/PVRAssets/Geometry.cpp
             src/main/cpp/PVRAssets/PixelFormat.cpp
             src/main/cpp/PVRAssets/ShadowVolume.cpp
             src/main/cpp/PVRAssets/FileIO/PaletteExpander.cpp
             src/main/cpp/PVRAssets/FileIO/PFXReader.cpp
             src/main/cpp/PVRAssets/FileIO/TextureReaderBMP.cpp
             src/main/cpp/PVRAssets/FileIO/TextureReaderKTX.cpp
             src/main/cpp/PVRAssets/FileIO/TextureReaderTGA.cpp
             src/main/cpp/PVRAssets/FileIO/TextureWriterDDS.cpp
             src/main/cpp/PVRAssets/FileIO/TextureWriterLegacyPVR.cpp
             src/main/cpp/PVRAssets/FileIO/PFXParser.cpp
             src/main/cpp/PVRAssets/FileIO/PODReader.cpp
             src/main/cpp/PVRAssets/FileIO/TextureReaderDDS.cpp
             src/main/cpp/PVRAssets/FileIO/TextureReaderPVR.cpp
             src/main/cpp/PVRAssets/FileIO/TextureReaderXNB.cpp
             src/main/cpp/PVRAssets/FileIO/TextureWriterKTX.cpp
             src/main/cpp/PVRAssets/FileIO/TextureWriterPVR.cpp
             src/main/cpp/PVRAssets/Model/Animation.cpp
             src/main/cpp/PVRAssets/Model/Camera.cpp
             src/main/cpp/PVRAssets/Model/Light.cpp
             src/main/cpp/PVRAssets/Model/Mesh.cpp
             src/main/cpp/PVRAssets/Model/Model.cpp
             src/main/cpp/PVRAssets/Texture/MetaData.cpp
             src/main/cpp/PVRAssets/Texture/PVRTDecompress.cpp
             src/main/cpp/PVRAssets/Texture/Texture.cpp
             src/main/cpp/PVRAssets/Texture/TextureHeader.cpp
             src/main/cpp/PVRAssets/Texture/TextureHeaderWithMetaData.cpp )

target_link_libraries( # Specifies the target library.
                       pvr_assets

                       # Links the target library to the log library
                       pvr_core)