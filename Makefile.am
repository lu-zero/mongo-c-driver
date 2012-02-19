dist_doc_DATA = README.md

lib_LTLIBRARIES = libmongoc.la libbson.la

pkginclude_HEADERS = src/bson.h \
                     src/gridfs.h \
		     src/mongo.h \
		     src/platform.h \
		     src/encoding.h \
		     src/md5.h \
		     src/net.h

libmongoc_la_SOURCES = src/md5.c src/mongo.c src/net.c src/gridfs.c src/bson.c src/numbers.c src/encoding.c

libbson_la_SOURCES = src/md5.c src/bson.c src/numbers.c src/encoding.c

libmongoc_la_LDFLAGS = -version-info $(LT_CURRENT):$(LT_REVISION):$(LT_AGE)

libbson_la_LDFLAGS = -version-info $(LT_CURRENT):$(LT_REVISION):$(LT_AGE)

ACLOCAL_AMFLAGS = -I m4

INCLUDES = -I. -I${top_srcdir}/src
