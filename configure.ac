AC_PREREQ (2.61)
AC_INIT ([BdwTabbedWidget], [0.1a], [mailto:ihernandezs@openmailbox.org], [bdwtabs])

AC_CONFIG_SRCDIR ([src])
AC_CONFIG_HEADERS ([config.h])
AC_CONFIG_MACRO_DIR ([m4])
AC_CONFIG_AUX_DIR ([build-aux])

AM_INIT_AUTOMAKE ([1.10 foreign dist-bzip2 no-dist-gzip])

m4_ifdef ([AM_SILENT_RULES], [AM_SILENT_RULES ([yes])])

# Check for programs
AX_CHECK_ENABLE_DEBUG
AC_PROG_CC

# Initialize libtool
LT_PREREQ ([2.2.6])
LT_INIT

# ***************************
# Check for required packages
# ***************************

pkg_modules="gtk+-3.0 >= 3.14 glib-2.0 >= 2.44"
PKG_CHECK_MODULES (BDWTABS, [$pkg_modules])

AC_CONFIG_FILES ([
	Makefile
	src/Makefile
])

AC_OUTPUT

