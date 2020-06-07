AC_INIT([Automake install paths test],
        [0.0.1],
	[https://github.com/ndim/automake-install-paths-test/issues],
	[automake-install-paths-test],
	[https://github.com/ndim/automake-install-paths-test])
AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_HEADER([aip-config.h])
AC_CONFIG_SRCDIR([aip-main.c])
AM_INIT_AUTOMAKE([
foreign
-Wall
-Werror
])

AC_PROG_CC

AC_ARG_VAR([CMP], [cmp file compare program])
AC_PATH_PROG([CMP], [cmp], [false])
AS_IF([test "x$CMP" = "xfalse"],
      [AC_MSG_ERROR([CMP must be a cmp program])])

AC_CONFIG_FILES([
Makefile
])
AC_OUTPUT
