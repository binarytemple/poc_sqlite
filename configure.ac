AC_PREREQ([2.69])


AC_INIT([pocsqlite], [0.1], [pocsqlite@binarytemple.co.uk])
AC_CONFIG_SRCDIR([src/bin/main.c])
AC_CONFIG_HEADERS([config.h])
AM_INIT_AUTOMAKE

# Checks for programs.
AC_PROG_CPP
AC_PROG_CC_C99
AC_PROG_RANLIB

# Use the C language and compiler for the following checks
AC_LANG([C])

# Checks for libraries.
PKG_CHECK_MODULES([GLIB], [glib-2.0], [have_libglib=yes], [have_libglib=no])
AM_CONDITIONAL([GLIB],  [test "$have_libglib" = "yes"])

PKG_CHECK_MODULES([SQLITE3], [sqlite3], [have_libsqlite3=yes], [have_libsqlite3=no])
AM_CONDITIONAL([LIB_SQLITE3],  [test "$have_libsqlite3" = "yes"])

# Checks for header files.
AC_HEADER_STDC
AC_CHECK_HEADERS([stdio.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T

# Checks for library functions.

AC_CONFIG_FILES([Makefile
                 src/bin/Makefile])
AC_OUTPUT
