cmake_minimum_required(VERSION 3.16)

project(wallpapers)
set(PROJECT_VERSION "6.7.4")

include(WriteBasicConfigVersionFile)
include(FeatureSummary)

set(KF5_MIN_VERSION "5.102.0")
set(KDE_COMPILERSETTINGS_LEVEL "5.82")

find_package(ECM ${KF5_MIN_VERSION} REQUIRED NO_MODULE)
set(CMAKE_MODULE_PATH ${ECM_MODULE_PATH} )

include(KDEInstallDirs)
include(KDECMakeSettings)
include(KDECompilerSettings)
include(GenerateExportHeader)

install(DIRECTORY SonicBallLightning DESTINATION ${KDE_INSTALL_WALLPAPERDIR})

