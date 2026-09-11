cmake_minimum_required(VERSION 3.16)

project(wallpapers)
set(PROJECT_VERSION "6.7.5")

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
install(DIRECTORY SonicDamascusSteel DESTINATION ${KDE_INSTALL_WALLPAPERDIR})
install(DIRECTORY SonicEternalDragon DESTINATION ${KDE_INSTALL_WALLPAPERDIR})
install(DIRECTORY SonicForestDragon DESTINATION ${KDE_INSTALL_WALLPAPERDIR})
install(DIRECTORY SonicForged DESTINATION ${KDE_INSTALL_WALLPAPERDIR})
install(DIRECTORY SonicGraffiti DESTINATION ${KDE_INSTALL_WALLPAPERDIR})
install(DIRECTORY SonicIce DESTINATION ${KDE_INSTALL_WALLPAPERDIR})
