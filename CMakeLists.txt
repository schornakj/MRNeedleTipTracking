cmake_minimum_required(VERSION 3.5)

project(LocalizationTools)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://slicer.org/slicerWiki/index.php/Documentation/Nightly/Extensions/LocalizationTools")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "Joseph Schornak (WPI AIM Lab)")
set(EXTENSION_DESCRIPTION "Extension for feature localization via MRI data")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/LocalizationTools.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/LocalizationTools/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a space separated string, a list or 'NA' if any

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(NeedleTipLocalizer)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
