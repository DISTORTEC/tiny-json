#
# file: CMakeLists.txt
#
# author: Copyright (C) 2020 Kamil Szczygiel http://www.distortec.com http://www.freddiechopin.info
#
# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0. If a copy of the MPL was not
# distributed with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
#

add_library(tiny-json STATIC
		tiny-json.c)
target_compile_options(tiny-json PRIVATE
		-Wno-char-subscripts)
target_include_directories(tiny-json INTERFACE
		${CMAKE_CURRENT_LIST_DIR})
