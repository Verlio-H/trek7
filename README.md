This fork contains a version of TREK7 updated to compile in current compilers and work on unix platforms.

This version is known to successfully compile, link, and run using gfortran 15.2.0, flang 21.1.7, and ifort 2021.10.0

Multiplayer functionality is available using an output and input file for each player.

One possible configuration to use this is to first make named pipe for the input file with mkfifo
Then, on another tty run `cat > (pipe name)`
When prompted for the terminal name, supply the device file of the other tty
You will then be prompted for an input file, where you supply the pipe name.

All additions to the code are done in lowercase.
