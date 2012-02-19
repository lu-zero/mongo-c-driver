AC_PREREQ(2.61)
AC_INIT([mongoc], [m4_esyscmd([./git-version-gen .tarball-version])],
        [http://www.mongodb.org/display/DOCS/C+Language+Center])
AC_CONFIG_AUX_DIR(config)
AM_INIT_AUTOMAKE([dist-bzip2 no-dist-gzip foreign subdir-objects])

m4_ifdef([AM_SILENT_RULES], [AM_SILENT_RULES([yes])])
AM_MAINTAINER_MODE

AC_PROG_CC_C99

LT_INIT

AC_CONFIG_HEADER([config.h])

AC_CONFIG_MACRO_DIR([m4])

LT_CURRENT=1
LT_REVISION=0
LT_AGE=0

MONGOC_MAJOR=1
MONGOC_MINOR=0
MONGOC_MICRO=4

dnl VERSION="${LT_CURRENT}.${LT_REVISION}.${LT_AGE}"

AC_SUBST(LT_CURRENT)
AC_SUBST(LT_REVISION)
AC_SUBST(LT_AGE)

AC_SUBST(MONGOC_MAJOR)
AC_SUBST(MONGOC_MINOR)
AC_SUBST(MONGOC_MICRO)

AC_CONFIG_FILES([Makefile
                 pkgconfig/mongo-c-driver.pc
                 pkgconfig/mongo-c-driver-uninstalled.pc])

AC_OUTPUT
