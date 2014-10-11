BOOST.Test finder script
========================

This script automatically find for you cpp files containing boost unit test and
generate a makefile with the following target:

 * `all:` compile and link all the test to create the runner executable.
 * `run:` start the runner.
 * `clean:` remove all files generated.

How to use
==========

To run the script, you just need to have python to be installed in you environment.
If you're on linux, just make sure the file is marked as executable:
 ```s```
