# MSP430 Energia port of ino
## Changes to Energia source files to fix compilation errors.
1. Missing itoa header file include in energia-0101E0015/hardware/msp430/cores/msp430/WString.cpp
  * Fix by adding "#include "itoa.h""
## Changes to msp430 gcc tools to fix compilation errors.
1. SR register and "status\_register" read/write macros redefine msp430 built-in functions.
  * Copy the header files from msp430\_gcc to the msp430 gcc/include directory. 
