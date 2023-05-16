# OPENMPI
Open MPI is a Message Passing Interface library project combining technologies and resources from several other projects.

## Setup

### Window
 - On Windows 10 and above
 - Enable WLS from Window Feature on and off.
 - Install Linux from microsoft store.
 - ls /mnt/ to access windows drive
 
 Note: Rest of steps will be common from Windows and Linux machines
 
### Linux
 - Download openmpi-4.1.4.tar.bz2 from https://www.open-mpi.org/software/ompi/v4.1/
 - Copy to Linux machine cp /mnt/d/OpenMP/LP5/openmpi-4.1.4.tar.bz2 LP5
 - install sudo apt install bzip2
 - tar -jxf openmpi-4.1.4.tar.bz2 
 - sudo apt-get install g++
 - ./configure --prefix=$HOME/opt/openmpi
 - sudo apt install make
 - make all install
 - echo "export PATH=\$PATH:\$HOME/opt/openmpi/bin" >> $HOME/.bashrc
 - echo "export LD_LIBRARY_PATH=\$LD_LIBRARY_PATH:\$HOME/opt/openmpi/lib">>$HOME/.bashrc
 - sudo apt install lam4-dev
 - sudo apt install gedit
 - lamboot
 
 Note: Run all the above mentioned commands to install the required software and libraries.
 
## Checking the System
 - Write or copy hello.c program 
 - Run *mpicc hello.c* to compile
 - Run *mpirun -np N ./a.out* to run the hello.c program
 
 Note: Only after execution of a sample program successfully the system is ready for running the assignment.

## Running the Addition program.
 - Compile the addition program by running *mpicc addition.c*
 - Run the addtion program by running *mpirun -np N ./a.out*
 
