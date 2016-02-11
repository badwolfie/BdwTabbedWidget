AC_INIT([bdwtabs], 0.1)
AC_CONFIG_SRCDIR([src])

AM_INIT_AUTOMAKE([no-dist-gzip dist-bzip2])

m4_ifdef([AM_SILENT_RULES], [AM_SILENT_RULES([yes])])

# Check for programs
AC_PROG_CC

# Initialize libtool
LT_PREREQ([2.2.6])
LT_INIT

# ***************************
# Check for required packages
# ***************************

pkg_modules="gtk+-3.0 >= 3.14 glib-2.0 >= 2.44"
PKG_CHECK_MODULES(BDWTABS, [$pkg_modules])
AC_SUBST(bdwtabs_CFLAGS)
AC_SUBST(bdwtabs_LIBS)

AC_CONFIG_FILES([
	Makefile
	src/Makefile
])

AC_OUTPUT

