if DEBUG
  AM_CFLAGS =-I$(top_srcdir)/src/bin -I$(top_srcdir)/src/lib -Wall -g -O3
else
  AM_CFLAGS =-I$(top_srcdir)/src/bin -I$(top_srcdir)/src/lib -Wall -O3
endif

AM_CFLAGS += $(GLIB_CFLAGS)
AM_CFLAGS += $(SQLITE3_CFLAGS)

bin_PROGRAMS = pocsqlite
pocsqlite_SOURCES = main.c

pocsqlite_LDADD = $(top_builddir)/src/lib/libpocsqlite-base.a $(AM_LDFLAGS)
pocsqlite_LDADD += $(GLIB_LIBS)
pocsqlite_LDADD += $(SQLITE3_LIBS)
