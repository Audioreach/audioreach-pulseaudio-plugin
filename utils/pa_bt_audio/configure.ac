#                                               -*- Autoconf -*-
# configure.ac -- Autoconf script for pulseaudio client
#

# Process this file with autoconf to produce a configure script.

# Requires autoconf tool later than 2.61
AC_PREREQ([2.69])
AC_INIT([pa_bt_audio_client_wrapper],1.0.0)
# Does not strictly follow GNU Coding standards
AM_INIT_AUTOMAKE([foreign])
# Disables auto rebuilding of configure, Makefile.ins
#AM_MAINTAINER_MODE
# defines some macros variable to be included by source
AC_CONFIG_HEADERS([config.h])
# defines some macros variable to be included by source
AC_CONFIG_MACRO_DIR([m4])

# Checks for programs.
AM_PROG_AS
AC_PROG_CC
AM_PROG_CC_C_O
AC_PROG_CXX
AC_PROG_LIBTOOL
AC_PROG_AWK
AC_PROG_CPP
AC_PROG_INSTALL
AC_PROG_LN_S
AC_PROG_MAKE_SET
PKG_PROG_PKG_CONFIG

PKG_CHECK_MODULES([GIO], [gio-2.0])
AC_SUBST([GIO_CFLAGS])
AC_SUBST([GIO_LIBS])

#pulseaudio
PKG_CHECK_MODULES([LIBPULSE], [libpulse])
AC_SUBST([LIBPULSE_CFLAGS])
AC_SUBST([LIBPULSE_LIBS])

AC_CONFIG_FILES([ \
        Makefile
        pabtaudio.pc
        ])

AC_OUTPUT
