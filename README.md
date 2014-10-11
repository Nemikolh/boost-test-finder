BOOST.Test finder script
------------------------

This script automatically find for you cpp files containing boost unit test and
generate a makefile with the following target:

 * `all:` compile and link all the test to create the runner executable.
 * `run:` start the runner.
 * `clean:` remove all files generated.

Requirements
------------

To run the script, you just need to have python to be installed in you environment.
If you're on linux, just make sure the file is marked as executable:

    chmod +x test-finder.py

How to use
----------

The following arguments are available:

 * Positional arguments:
   * `FILE|FOLDER [FILE|FOLDER ...]` a list of folder or files containing Boost.Test.
 * Optional arguments:
   * `-o MAKEFILE, --output MAKEFILE` path for the output makefile.
   * `-l [LIBRARIES ...], --libraries [LIBRARIES ...]` a list of libraries to link with (for instance: `-l GL`)
   * `-f [FLAGS ...], --flags [FLAGS ...]` a list of compiler flags.
   * `--runner RUNNER` name of the executable.
   * `--compiler COMPILER` name of the compiler.
