
include ../../GDALmake.opt

OBJ	=	openjpegdataset.o



ifneq ($(OPENJPEG_VERSION),)
CPPFLAGS 	:=	$(CPPFLAGS) -DOPENJPEG_VERSION=$(OPENJPEG_VERSION)
endif

CPPFLAGS        :=       -I.. $(CPPFLAGS)


default:	$(OBJ:.o=.$(OBJ_EXT))

clean:
	rm -f $(OBJ) $(O_OBJ)

install-obj:	$(O_OBJ:.o=.$(OBJ_EXT))
