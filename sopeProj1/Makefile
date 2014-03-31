CFILES := main.c
PROG := sopeProj1
CFLAGS := -Wall -Wextra -g
LDFLAGS :=

CFLAGS += -MMD
CC := gcc

OBJFILES := $(CFILES:.c=.o)
DEPFILES := $(CFILES:.c=.d)

$(PROG) : $(OBJFILES)
		$(LINK.o) $(LDFLAGS) -o $@ $^

clean :
		rm -f $(PROG) $(OBJFILES) $(DEPFILES)

-include $(DEPFILES)