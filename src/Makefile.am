# This is _NOT_ the library release version, it's an API version.
# Please read Chapter 6 "Library interface versions" of the libtool documentation before making any modification
LIBVERSION=0:0:0

INCLUDES = $(all_includes) -I$(top_srcdir)/include
AM_CFLAGS = ${CFLAGS} -fPIC ${SYMBOL_VISIBILITY}

lib_LTLIBRARIES = libmirisdr.la

libmirisdr_la_SOURCES = libmirisdr.c tuner_msi001.c
libmirisdr_la_LDFLAGS = -version-info $(LIBVERSION)

bin_PROGRAMS         = miri_sdr

miri_sdr_SOURCES     = miri_sdr.c
miri_sdr_LDADD       = libmirisdr.la
