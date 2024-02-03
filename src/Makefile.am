## Process this file with automake to produce Makefile.in

## Created by Anjuta

AM_CPPFLAGS = \
	-DPACKAGE_LOCALE_DIR=\""$(localedir)"\" \
	-DPACKAGE_SRC_DIR=\""$(srcdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(pkgdatadir)"\" \
	$(LCS_CFLAGS)

AM_CFLAGS =\
	 -Wall\
	 -g

lib_LTLIBRARIES = liblcs.la


liblcs_la_SOURCES = \
	lib.c

liblcs_la_LDFLAGS = 

liblcs_la_LIBADD = $(LCS_LIBS)


if PLATFORM_WIN32
liblcs_la_LDFLAGS += -no-undefined
endif

if NATIVE_WIN32
liblcs_la_LDFLAGS += -export-dynamic
endif

include_HEADERS = \
	lcs.h

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = lcs-0.1.pc

EXTRA_DIST = \
	lcs-0.1.pc.in
