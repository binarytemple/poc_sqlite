# The libraries to build
noinst_LIBRARIES = libpocsqlite-base.a
noinst_HEADERS = pocsqlite-base.h

# The files to add to the library and to the source distribution
libpocsqlite_base_a_SOURCES = \
                         $(libpocsqlite_base_a_HEADERS) \
                         pocsqlite-base.c

if DEBUG
  AM_CFLAGS =-I$(top_srcdir)/src/lib -Wall -g -O3
else
  AM_CFLAGS =-I$(top_srcdir)/src/lib -Wall
endif

