## Microcontroller Interconnect Network protocol version 2.0

This MIN repository includes the specification, a standard C API and
reference implementations for C and Python. See the Wiki for further
details:

http://github.com/min-protocol/min/wiki

If you are using this as a library, you should only build and include the files in src/. The other files are just examples or code generation files.

File structure:

    src/	            Embedded code. Everything else is extraneous.
        min.c               MIN code designed to run on an embedded system (from 8-bit MCUs upwards)
        min.h               Header file that defines the API to min
    target/
	sketch_example1     Arduino sketch for an example program
    host/                   Python code to run on a host PC
        min.py              MIN 2.0 reference implementation with support for MIN via Pyserial
	    listen.py       Example program to run on a host and talk to an Arduino board
    builder/ 		    Files for generating code for the library. Users can ignore.
    	...

There is also a Rust implementation of MIN for both host and target:

https://github.com/qianchenzhumeng/min-rs

All software and documentation available under the terms of the MIT License:

	The MIT License (MIT)
	
	Copyright (c) 2014-2017 JK Energy Ltd.
	
	Permission is hereby granted, free of charge, to any person obtaining a copy
	of this software and associated documentation files (the "Software"), to deal
	in the Software without restriction, including without limitation the rights
	to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
	copies of the Software, and to permit persons to whom the Software is
	furnished to do so, subject to the following conditions:
	
	The above copyright notice and this permission notice shall be included in
	all copies or substantial portions of the Software.
	
	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
	IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
	FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
	AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
	LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
	OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
	THE SOFTWARE.
