CXXFLAGS =	-g3 -fmessage-length=0 -Wno-narrowing -Wno-macro-redefined

OBJS =		Centipede.o Scorpion.o Segment.o Spider.o ScoreBoard.o Flea.o Player.o MoveableObject.o MushroomArr.o Mushroom.o Fire.o GameObject.o Position.o Board.o util.o game.o

LIBS = -L/usr/X11R6/lib -L/sw/lib -L/usr/sww/lib -L/usr/sww/bin -L/usr/sww/pkg/Mesa/lib -lglut -lGLU -lX11 -lGL -sLEGACY_GL_EMULATION -o game.html -sWASM=1 -sSTACK_SIZE=2097152 -sEXIT_RUNTIME=1 -sGL_UNSAFE_OPTS=0



TARGET =	game


$(TARGET):	$(OBJS) 
	$(CXX) -o $(TARGET) $(OBJS) $(LIBS)

all:	$(TARGET)

clean:
	rm -f $(OBJS) $(TARGET)
