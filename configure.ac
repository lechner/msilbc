# Process this file with autoconf to produce a configure script.
AC_INIT([msilbc],[2.0.2])
AC_PREREQ(2.64)
AC_CONFIG_SRCDIR([ilbc.c])
AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_MACRO_DIR([m4])

AM_INIT_AUTOMAKE([tar-ustar])

AC_ARG_VAR(MSILBC_CFLAGS,
	[Extra C compiler flags for msilbc, such as -DUSE_30MS_PACKETS=1])

# initialize libtool
LT_INIT([disable-static])

# Checks for libraries that have pkg-config files installed
PKG_CHECK_MODULES(ORTP, ortp >= 0.16.0)
PKG_CHECK_MODULES(MEDIASTREAMER, mediastreamer >= 2.0.0)
PKG_CHECK_MODULES(ILBC, ilbc >= 0.0.0)

# Create the following files from their .in counterparts
AC_CONFIG_FILES([
  Makefile
])
AC_OUTPUT

