# $FreeBSD$
.PATH:  ${.CURDIR}/../../dev/mlx4/mlx4_en

KMOD=	mlx4en
SRCS=	device_if.h bus_if.h pci_if.h vnode_if.h \
	opt_inet.h opt_inet6.h \
	mlx4_en_cq.c \
	mlx4_en_main.c \
	mlx4_en_netdev.c \
	mlx4_en_port.c \
	mlx4_en_resources.c \
	mlx4_en_rx.c \
	mlx4_en_tx.c

CFLAGS+= -I${.CURDIR}/../../ofed/include
CFLAGS+= -I${.CURDIR}/../../compat/linuxkpi/common/include
CFLAGS+= -I${.CURDIR}/../../contrib/ck/include

.include <bsd.kmod.mk>
