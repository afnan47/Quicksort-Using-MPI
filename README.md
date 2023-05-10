# Quicksort-Using-MPI
Parallel QuickSort Implementation using MPI

## Windows Users 
Getting the MPI library set up on windows is quite a hassel. The best way to setup MPI programs is to use WSL[[Windows Subsystem For Linux]](https://learn.microsoft.com/en-us/windows/wsl/install).
### Steps:
1. Open windows command prompt or powershell by running as administrator and run the following command `wsl --install`.
2. After installation is done, set up your username and password.
3. Run commands `sudo apt-get update`, `sudo apt install mpich` and `sudo apt install git`.
4. Clone this repo: `git clone https://github.com/afnan47/Quicksort-Using-MPI`.
5. Move into the directory cloned: `cd Quicksort-Using-MPI/`.
6. Compile the code: `mpiCC quick_sort_MPI.cpp -o quick_sort_MPI`.
7. Edit input file: `nano input.txt` or `vim input.txt`.(If you are not used to Linux editors, run `explorer.exe .` command to open explorer in the current folder. You can then edit the input file using notepad or use other tools such as VSCode)
8. First enter the number of elements in your array and then the elements. For Example: 5 71 64 -12 434 3.
9. Save your input file and exit.
10. Run `mpirun -np 4 ./quick_sort_MPI input.txt output.txt`.

According to the number of processes you want you can change the value for the `-np` flag. 
For example, `-np 4`, `-np 10`.
You do not need to compile the program again if you make changes in `input.txt`, simply do step 10.

### Linux Users can start from step 3.

