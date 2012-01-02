
#  Makefile for QuartzCore
#
#  Copyright (C) 2011 Free Software Foundation, Inc.
#
#  Written by: Amr Aboelela
#  Date: December, 2011
#
#  This file is part of QuartzCore.
#
#  This library is free software; you can redistribute it and/or
#  modify it under the terms of the GNU Lesser General Public
#  License as published by the Free Software Foundation; either
#  version 2 of the License, or (at your option) any later version.
#
#  This library is distributed in the hope that it will be useful,
#  but WITHOUT ANY WARRANTY; without even the implied warranty of
#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
#  Lesser General Public License for more details.
#
#  You should have received a copy of the GNU Lesser General Public
#  License along with this library; see the file COPYING.LIB.
#  If not, see <http://www.gnu.org/licenses/> or write to the
#  Free Software Foundation, 51 Franklin Street, Fifth Floor,
#  Boston, MA 02110-1301, USA.

ifeq ($(GNUSTEP_MAKEFILES),)
  GNUSTEP_MAKEFILES := $(shell gnustep-config --variable=GNUSTEP_MAKEFILES 2>/dev/null)
  ifeq ($(GNUSTEP_MAKEFILES),)
    $(error You need to set GNUSTEP_MAKEFILES before compiling!)
  endif
endif

include $(GNUSTEP_MAKEFILES)/common.make

LIBRARY_NAME = libQuartzCore
libQuartzCore_HEADER_FILES = \
        CAAnimation.h \
        CAGradientLayer.h \
        CAReplicatorLayer.h \
        CATiledLayer.h \
        CAValueFunction.h \
        CABase.h \
        CALayer.h \
        CAScrollLayer.h \
        CATransaction.h \
        CoreAnimation.h \
        CADisplayLink.h \
        CAMediaTiming.h \
        CAShapeLayer.h \
        CATransform3D.h \
        QuartzCore.h \
        CAEAGLLayer.h \
        CAMediaTimingFunction.h \
        CATextLayer.h \
        CATransformLayer.h

libQuartzCore_HEADER_FILES_INSTALL_DIR = QuartzCore
libQuartzCore_OBJC_FILES = $(wildcard *.m) 

include $(GNUSTEP_MAKEFILES)/library.make