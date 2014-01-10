# Makefile.in generated automatically by automake 1.4-p4 from Makefile.am

# Copyright (C) 1994, 1995-8, 1999 Free Software Foundation, Inc.
# This Makefile.in is free software; the Free Software Foundation
# gives unlimited permission to copy and/or distribute it,
# with or without modifications, as long as this notice is preserved.

# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY, to the extent permitted by law; without
# even the implied warranty of MERCHANTABILITY or FITNESS FOR A
# PARTICULAR PURPOSE.


SHELL = c:/bin/sh

srcdir = .
top_srcdir = ..

prefix = /usr/local
exec_prefix = ${prefix}

bindir = ${exec_prefix}/bin
sbindir = ${exec_prefix}/sbin
libexecdir = ${exec_prefix}/libexec
datadir = ${prefix}/share
sysconfdir = ${prefix}/etc
sharedstatedir = ${prefix}/com
localstatedir = ${prefix}/var
libdir = ${exec_prefix}/lib
infodir = ${prefix}/info
mandir = ${prefix}/man
includedir = ${prefix}/include
oldincludedir = /usr/include

DESTDIR =

pkgdatadir = $(datadir)/stunnel
pkglibdir = $(libdir)/stunnel
pkgincludedir = $(includedir)/stunnel

top_builddir = ..

ACLOCAL = aclocal
AUTOCONF = autoconf
AUTOMAKE = automake
AUTOHEADER = autoheader

INSTALL = c:/unixos2/bin/install.exe
INSTALL_PROGRAM = ${INSTALL} $(AM_INSTALL_PROGRAM_FLAGS)
INSTALL_DATA = ${INSTALL} -m 644
INSTALL_SCRIPT = ${INSTALL}
transform = s,x,x,

NORMAL_INSTALL = :
PRE_INSTALL = :
POST_INSTALL = :
NORMAL_UNINSTALL = :
PRE_UNINSTALL = :
POST_UNINSTALL = :
host_alias = 
host_triplet = i386-pc-os2-emx
AS = @AS@
CC = gcc
DLLTOOL = @DLLTOOL@
ECHO = print -r
EXEEXT = .exe
LIBTOOL = $(SHELL) $(top_builddir)/libtool
LN_S = ln
MAKEINFO = makeinfo
OBJDUMP = @OBJDUMP@
OBJEXT = o
PACKAGE = stunnel
RANDOM_FILE = 
RANLIB = echo
STRIP = strip
USE_DH = 0
VERSION = 4.05
host = i386-pc-os2-emx
ssldir = /usr

DISTCLEANFILES = stunnel.pem
EXTRA_DIST = ca.html ca.pl importCA.html importCA.sh script.sh 	stunnel.spec stunnel.mak stunnel.cnf


confdir = $(sysconfdir)/stunnel
conf_DATA = stunnel.conf-sample stunnel.pem

docdir = $(datadir)/doc/stunnel
examplesdir = $(docdir)/examples
examples_DATA = ca.html ca.pl importCA.html importCA.sh script.sh 	stunnel.spec stunnel.init


openssl = $(ssldir)/bin/openssl
mkinstalldirs = $(SHELL) $(top_srcdir)/auto/mkinstalldirs
CONFIG_CLEAN_FILES =  stunnel.conf-sample stunnel.init
DATA =  $(conf_DATA) $(examples_DATA)

DIST_COMMON =  Makefile.am Makefile.in stunnel.conf-sample.in \
stunnel.init.in


DISTFILES = $(DIST_COMMON) $(SOURCES) $(HEADERS) $(TEXINFOS) $(EXTRA_DIST)

TAR = tar
GZIP_ENV = --best
all: all-redirect
.SUFFIXES:
$(srcdir)/Makefile.in: Makefile.am $(top_srcdir)/configure.ac $(ACLOCAL_M4) 
	cd $(top_srcdir) && $(AUTOMAKE) --gnu --include-deps tools/Makefile

Makefile: $(srcdir)/Makefile.in  $(top_builddir)/config.status
	cd $(top_builddir) \
	  && CONFIG_FILES=$(subdir)/$@ CONFIG_HEADERS= $(SHELL) ./config.status

stunnel.conf-sample: $(top_builddir)/config.status stunnel.conf-sample.in
	cd $(top_builddir) && CONFIG_FILES=$(subdir)/$@ CONFIG_HEADERS= $(SHELL) ./config.status
stunnel.init: $(top_builddir)/config.status stunnel.init.in
	cd $(top_builddir) && CONFIG_FILES=$(subdir)/$@ CONFIG_HEADERS= $(SHELL) ./config.status

install-confDATA: $(conf_DATA)
	@$(NORMAL_INSTALL)
	$(mkinstalldirs) $(DESTDIR)$(confdir)
	@list='$(conf_DATA)'; for p in $$list; do \
	  if test -f $(srcdir)/$$p; then \
	    echo " $(INSTALL_DATA) $(srcdir)/$$p $(DESTDIR)$(confdir)/$$p"; \
	    $(INSTALL_DATA) $(srcdir)/$$p $(DESTDIR)$(confdir)/$$p; \
	  else if test -f $$p; then \
	    echo " $(INSTALL_DATA) $$p $(DESTDIR)$(confdir)/$$p"; \
	    $(INSTALL_DATA) $$p $(DESTDIR)$(confdir)/$$p; \
	  fi; fi; \
	done

uninstall-confDATA:
	@$(NORMAL_UNINSTALL)
	list='$(conf_DATA)'; for p in $$list; do \
	  rm -f $(DESTDIR)$(confdir)/$$p; \
	done

install-examplesDATA: $(examples_DATA)
	@$(NORMAL_INSTALL)
	$(mkinstalldirs) $(DESTDIR)$(examplesdir)
	@list='$(examples_DATA)'; for p in $$list; do \
	  if test -f $(srcdir)/$$p; then \
	    echo " $(INSTALL_DATA) $(srcdir)/$$p $(DESTDIR)$(examplesdir)/$$p"; \
	    $(INSTALL_DATA) $(srcdir)/$$p $(DESTDIR)$(examplesdir)/$$p; \
	  else if test -f $$p; then \
	    echo " $(INSTALL_DATA) $$p $(DESTDIR)$(examplesdir)/$$p"; \
	    $(INSTALL_DATA) $$p $(DESTDIR)$(examplesdir)/$$p; \
	  fi; fi; \
	done

uninstall-examplesDATA:
	@$(NORMAL_UNINSTALL)
	list='$(examples_DATA)'; for p in $$list; do \
	  rm -f $(DESTDIR)$(examplesdir)/$$p; \
	done
tags: TAGS
TAGS:


distdir = $(top_builddir)/$(PACKAGE)-$(VERSION)/$(subdir)

subdir = tools

distdir: $(DISTFILES)
	@for file in $(DISTFILES); do \
	  d=$(srcdir); \
	  if test -d $$d/$$file; then \
	    cp -pr $$d/$$file $(distdir)/$$file; \
	  else \
	    test -f $(distdir)/$$file \
	    || ln $$d/$$file $(distdir)/$$file 2> /dev/null \
	    || cp -p $$d/$$file $(distdir)/$$file || :; \
	  fi; \
	done
info-am:
info: info-am
dvi-am:
dvi: dvi-am
check-am: all-am
check: check-am
installcheck-am:
installcheck: installcheck-am
install-exec-am:
install-exec: install-exec-am

install-data-am: install-confDATA install-examplesDATA
	@$(NORMAL_INSTALL)
	$(MAKE) $(AM_MAKEFLAGS) install-data-hook
install-data: install-data-am

install-am: all-am
	@$(MAKE) $(AM_MAKEFLAGS) install-exec-am install-data-am
install: install-am
uninstall-am: uninstall-confDATA uninstall-examplesDATA
uninstall: uninstall-am
all-am: Makefile $(DATA)
all-redirect: all-am
install-strip:
	$(MAKE) $(AM_MAKEFLAGS) AM_INSTALL_PROGRAM_FLAGS=-s install
installdirs:
	$(mkinstalldirs)  $(DESTDIR)$(confdir) $(DESTDIR)$(examplesdir)


mostlyclean-generic:

clean-generic:

distclean-generic:
	-rm -f Makefile $(CONFIG_CLEAN_FILES)
	-rm -f config.cache config.log stamp-h stamp-h[0-9]*
	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)

maintainer-clean-generic:
mostlyclean-am:  mostlyclean-generic

mostlyclean: mostlyclean-am

clean-am:  clean-generic mostlyclean-am clean-local

clean: clean-am

distclean-am:  distclean-generic clean-am
	-rm -f libtool

distclean: distclean-am

maintainer-clean-am:  maintainer-clean-generic distclean-am
	@echo "This command is intended for maintainers to use;"
	@echo "it deletes files that may require special tools to rebuild."

maintainer-clean: maintainer-clean-am

.PHONY: uninstall-confDATA install-confDATA uninstall-examplesDATA \
install-examplesDATA tags distdir info-am info dvi-am dvi check \
check-am installcheck-am installcheck install-exec-am install-exec \
install-data-am install-data install-am install uninstall-am uninstall \
all-redirect all-am all installdirs mostlyclean-generic \
distclean-generic clean-generic maintainer-clean-generic clean \
mostlyclean distclean maintainer-clean

stunnel.pem: stunnel.cnf
	if test -r "$(RANDOM_FILE)"; \
		then dd if="$(RANDOM_FILE)" of=stunnel.rnd bs=256 count=1; \
			RND="-rand stunnel.rnd"; \
		else RND=""; fi; \
	$(openssl) req -new -x509 -days 365 -nodes $$RND \
		-config $(srcdir)/stunnel.cnf -out stunnel.pem -keyout stunnel.pem; \
	test $(USE_DH) -eq 0 || $(openssl) gendh $$RND 512 >> stunnel.pem
	$(openssl) x509 -subject -dates -fingerprint -noout \
		-in stunnel.pem

install-data-hook:
	chmod 0600 $(DESTDIR)$(confdir)/stunnel.pem

clean-local:
	-rm -f stunnel.rnd

# Tell versions [3.59,3.63) of GNU make to not export all variables.
# Otherwise a system limit (for SysV at least) may be exceeded.
.NOEXPORT:
