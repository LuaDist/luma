# Copyright (C) 2007-2012 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( luma NONE )
cmake_minimum_required ( VERSION 2.8 )
include ( cmake/dist.cmake )
include ( lua )

# Install all files and documentation
install_lua_module ( luma src/luma.lua )
install_lua_module ( luma.re src/re.lua )
install_lua_module ( luma.cosmo src/cosmo.lua )
install_lua_executable ( expand bin/expand )
install_lua_executable ( luma bin/luma )
install_test ( tests/ )
install_example ( samples/ )
install_doc ( doc/ )
