# $FreeBSD: src/cddl/lib/drti/Makefile,v 1.1.4.1 2009/08/03 08:13:06 kensmith Exp $

.include	"../../Makefile.inc"

.PATH:		${OPENSOLARIS_USR_DISTDIR}/lib/libdtrace/common

SRCS=		drti.c
FILES=		${SRCS:R:S/$/.o/g}
FILESOWN=	${LIBOWN}
FILESGRP=	${LIBGRP}
FILESMODE=	${LIBMODE}
FILESDIR=	${LIBDIR}/dtrace
WARNS?=		6
CLEANFILES=	${FILES}

CFLAGS+=	-I${.CURDIR}/../../../sys/cddl/compat/opensolaris \
		-I${.CURDIR}/../../../cddl/compat/opensolaris/include \
		-I${OPENSOLARIS_USR_DISTDIR}/head \
		-I${OPENSOLARIS_USR_DISTDIR}/lib/libctf/common \
		-I${OPENSOLARIS_USR_DISTDIR}/lib/libdtrace/common \
		-I${OPENSOLARIS_SYS_DISTDIR}/uts/common

.include <bsd.prog.mk>
