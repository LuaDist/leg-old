# Copyright (C) 2007-2009 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(leg NONE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

# Install
INSTALL(FILES src/grammar.lua src/init.lua src/parser.lua src/scanner.lua  DESTINATION ${INSTALL_LMOD}/leg)
INSTALL(FILES README COPYRIGHT release DESTINATION ${INSTALL_DATA})
INSTALL(DIRECTORY doc/ DESTINATION ${INSTALL_DOC})
INSTALL(DIRECTORY tests/ DESTINATION ${INSTALL_TEST})
INSTALL(DIRECTORY examples/ DESTINATION ${INSTALL_EXAMPLE})
