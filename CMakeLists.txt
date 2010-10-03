# Copyright (C) 2007-2009 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(luma NONE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

# Install all files and documentation
INSTALL (FILES src/luma.lua DESTINATION ${INSTALL_LMOD})
INSTALL (FILES src/re.lua src/cosmo.lua DESTINATION ${INSTALL_LMOD}/luma )

INSTALL (FILES bin/expand bin/luma DESTINATION ${INSTALL_BIN})
INSTALL(DIRECTORY tests/ DESTINATION ${INSTALL_TEST})
INSTALL(DIRECTORY samples/ DESTINATION ${INSTALL_EXAMPLE})
INSTALL(DIRECTORY doc/ DESTINATION ${INSTALL_DOC})
