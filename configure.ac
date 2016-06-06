AC_INIT([bdwtabs], 0.1)
AC_CONFIG_SRCDIR([src])

AM_INIT_AUTOMAKE([no-dist-gzip dist-bzip2])
GNOME_MAINTAINER_MODE_DEFINES

# Enable silent rules is available
m4_ifdef([AM_SILENT_RULES], [AM_SILENT_RULES([yes])])

AM_MAINTAINER_MODE

AC_PATH_PROG(GLIB_COMPILE_RESOURCES, glib-compile-resources)

AC_PROG_CC
AC_PROG_CC_STDC
AC_PROG_INSTALL

pkg_modules="gtk+-3.0 >= 3.10"
PKG_CHECK_MODULES(bdwtabs, [$pkg_modules])
AC_SUBST(bdwtabs_CFLAGS)
AC_SUBST(bdwtabs_LIBS)

AC_CONFIG_FILES([
	Makefile
	src/Makefile
])
AC_OUTPUT

