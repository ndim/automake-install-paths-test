BUILT_SOURCES =
CLEANFILES =
bin_PROGRAMS =

CLEANFILES    += install-paths.h
CLEANFILES    += install-paths.stamp
BUILT_SOURCES += install-paths.stamp
install-paths.stamp:
	echo '/* Autogenerated file. Do not modify. */' > install-paths.h.tmp
	echo '#define BINDIR "$(bindir)"' >> install-paths.h.tmp
	@if test -f install-paths.h \
	   && $(CMP) install-paths.h.tmp install-paths.h; then \
	  echo "Not updating install-paths.h: it is up to date"; \
	  rm -f install-paths.h.tmp; \
	else \
	  echo "Updating install-paths.h"; \
	  mv -f install-paths.h.tmp install-paths.h; \
	fi

bin_PROGRAMS     += aip-test
aip_test_SOURCES  =
aip_test_SOURCES += aip-main.c
