#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ(2.59)
AC_INIT(oll, 0.01, hillbig@is.s.u-tokyo.ac.jp)
AC_CONFIG_SRCDIR([oll.cpp])
AC_CONFIG_HEADER([config.h])
AM_INIT_AUTOMAKE(oll, 0.01)

# Checks for programs.
AC_PROG_CXX

# Checks for libraries.
AC_PROG_LIBTOOL

# Checks for header files.
# AC_CHECK_HEADERS([memory.h sys/types.h sys/stat.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_HEADER_STDBOOL
AC_C_CONST
AC_C_INLINE
AC_TYPE_SIZE_T

# Checks for library functions.
AC_HEADER_STDC
AC_FUNC_SELECT_ARGTYPES
# AC_CHECK_FUNCS([memset select])

# Default Compiler Option
if test x$CC = xgcc; then
  CFLAGS="$CFLAGS -Wall -Wformat=2 -pipe -Wno-sign-compare -D_FORTIFY_SOURCE=1 -Wcast-qual -Wcast-align -Wpointer-arith -Wwrite-strings"
fi

if test x$CXX = xg++; then
  CPPFLAGS="$CPPFLAGS -Wall -Wformat=2 -pipe -Wno-sign-compare -D_FORTIFY_SOURCE=1 -Wcast-qual -Wcast-align -Wpointer-arith -Wwrite-strings -Woverloaded-virtual"
fi

AC_CONFIG_FILES([Makefile])
AC_OUTPUT
