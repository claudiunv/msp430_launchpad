# Simply Embedded Tutorials
---
> Author: Chris Karaplis, info@simplyembedded.org
> Copyright (c) 2015, simplyembedded.org
> All rights reserved.
---

Terms of use
---
```
Redistribution and use in source and binary forms, with or without 
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, 
   this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" 
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE 
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE 
ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE 
LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR 
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF 
SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS 
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN 
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) 
ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE 
POSSIBILITY OF SUCH DAMAGE.
```
How to build
---

**Prerequisites:**

 * TI / Redhat MSP430-GCC toolchain
 * make

---
**or:**

 * TI MSP430-GCC  4_02_00_00 (latest stable) binaries
 * make

Modify `makefile` to have CC variable path set for `msp430-elf-gcc` like this:

```
# Toolchain variables
# Set this variable to use the TI's builded toolchain
CC:=$(TOOLCHAIN_ROOT)/bin/msp430-elf-gcc
#
# Set this variable to use the toolchain compiled on how is described on
# tutorial
# CC:=$(TOOLCHAIN_ROOT)/bin/msp430-gcc
```
---

If the toolchain is not installed under /opt/msp430-toolchain, set the environment
variable TOOLCHAIN_ROOT to point to the toolchain root directory.

To build, execute the following command from the console in the project root directory:

    make all


To perform a full clean of the build including intermediate files and dependancies, run

    make clean

Questions or comments?
-----------------------
Please contact us at info@simplyembedded.org

