CIR = $(wildcard *.cir)
NAMES = $(patsubst %.cir, %, $(CIR))

all: $(CIR)
	@for i in $(NAMES);\
	do \
		hspice "$$i"'.cir' >  "$$i"'.out';\
	done

.PHONY: clean
clean:
	rm *.ic* *.st* *.sw* *.tr* *.out
