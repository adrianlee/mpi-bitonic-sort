ECSE420 Parallel Assignment 4
Dec 3, 2012
Adrian Lee
260272188

Files included:
    bitonic.c
    bitonic.h
    bitonic [executable]
    README.txt

How to run:
    1. Compile: $ mpicc bitonic.c -o bitonic
    2. Run:     $ mpirun -n 4 ./bitonic 32000000

Note:
    Bitonic program takes in one args(# of random numbers to sort)

Example:
    $ mpirun -n 1 ./bitonic 32000000
    $ mpirun -n 2 ./bitonic 32000000
    $ mpirun -n 8 ./bitonic 64000000
    $ mpirun -n 4 ./bitonic 128000000
    $ mpirun -n 8 ./bitonic 128000000


Other notes:
    Not sure why setting 64 processes doesn't work for me.
    Would have been cool to see how fast it would take.

References:
    Assignment 4 Supplement - Parallel Bitonic Sort Algorithm
    Sorting Algorithms - http://www-users.cs.umn.edu/~karypis/parbook/Algorithms/pchap9.pdf
    Bionic Sorting - http://www.thi.informatik.uni-frankfurt.de/~klauck/PDA07/Bitonic%20Sorting.pdf