FC=gfortran

all: main_force

OBJ= module.o number_of_line.o get_data_number.o \
     main_force.o get_data_matrix.o fitting.o 

main_force: $(OBJ)
	$(FC) $^ -o $@

%.o: %.f90
	$(FC) -c $<

clean:
	rm -rf *.o

