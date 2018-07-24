
SRC = conv.pg   conv2.pg  conv3.pg  nfe_k.pg  nfe_n.pg  pop_k1.pg pt_n.pg   supply.pg
OBJ = $(addsuffix .eps, $(basename $(SRC)))

%.eps : %.pg %.txt
	gnuplot $<

all:	$(OBJ)
	cp *eps ..
clean:
	rm -rf $(OBJ)

