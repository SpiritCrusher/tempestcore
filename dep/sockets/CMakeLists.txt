# Copyright (C) 2008 - 2010 Trinity <http://www.trinitycore.org/>
#
# Copyright (C) 2010 Myth Project <http://mythproject.org/>
#
# This file is free software; as a special exception the author gives
# unlimited permission to copy and/or distribute it, with or without
# modifications, as long as this notice is preserved.
#
# This program is distributed in the hope that it will be useful, but
# WITHOUT ANY WARRANTY, to the extent permitted by law; without even the
# implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

file(GLOB sources *.cpp)

set(trinitysockets_STAT_SRCS
  ${sources}
)

include_directories(
  ${CMAKE_CURRENT_SOURCE_DIR}/include
)

add_library(trinitysockets STATIC ${trinitysockets_STAT_SRCS})
