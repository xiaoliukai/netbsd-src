#	$NetBSD: Makefile,v 1.6 2014/03/09 22:01:31 christos Exp $

# $FreeBSD: src/cddl/usr.bin/ctfmerge/Makefile,v 1.1.4.1 2009/08/03 08:13:06 kensmith Exp $

.include <bsd.own.mk>

.include	"../../Makefile.inc"
.include	"../../Makefile.ctf"

.PATH:          ${OPENSOLARIS_USR_DISTDIR}/tools/ctf/cvt

PROG=		ctfmerge

SRCS=		alist.c \
		barrier.c \
		ctf.c \
		ctfmerge.c \
		fifo.c \
		hash.c \
		iidesc.c \
		input.c \
		list.c \
		memory.c \
		merge.c \
		output.c \
		strtab.c \
		symbol.c \
		tdata.c \
		traverse.c \
		util.c

LDADD+=-lrt -lpthread
DPADD+=${LIBRT} ${LIBPTHREAD}

.include <bsd.prog.mk>
