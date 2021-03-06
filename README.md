![MTuner logo](https://github.com/milostosic/MTuner/blob/master/img/logo.png)

[![Build status](https://ci.appveyor.com/api/projects/status/fo9uy9h3bcka20kk?svg=true)](https://ci.appveyor.com/project/milostosic/MTuner)
[![License](https://img.shields.io/badge/license-BSD--2%20clause-blue.svg)](https://github.com/milostosic/MTuner/blob/master/LICENSE)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/milostosic/MTuner.svg)](http://isitmaintained.com/project/milostosic/MTuner "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/milostosic/MTuner.svg)](http://isitmaintained.com/project/milostosic/MTuner "Percentage of issues still open")

**MTuner** is a C/C++ memory profiler and memory leak finder for Windows, PS4, PS3, etc.

**MTuner** utilizes a novel approach to memory profiling and analysis, keeping entire time-based history of memory operations. This gives an unique insight in memory related behavior of your software by making queries over the entire data set.

![MTuner screenshot](https://github.com/milostosic/MTuner/blob/master/img/mtuner_screenshot.png)

Source Code
======

You can get the latest source code by cloning it from github:

      git clone https://github.com/milostosic/MTuner.git 

Dependencies
======

MTuner uses [Qt](https://www.qt.io/) framework for user interface.

Dependencies can be obtained by cloning the following repositories:

	git clone https://github.com/milostosic/build.git
	git clone https://github.com/milostosic/rbase.git
	git clone https://github.com/milostosic/rdebug.git
	git clone https://github.com/milostosic/rmem.git
	git clone https://github.com/milostosic/rqt.git
	git clone https://github.com/milostosic/MTunerCmd.git
	git clone https://github.com/milostosic/MTunerDLL.git
	git clone https://github.com/milostosic/MTunerInject.git

DIA (Debug Interface Access) SDK - **Windows only**

	git clone https://github.com/milostosic/DIA.git 

Download
======

[<img src="http://mtuner.net/zip.png" width=32 height=32> **zip**](http://mtuner.net/mtuner64.zip)  
[<img src="http://mtuner.net/msi.png" width=32 height=32> **msi**](http://mtuner.net/mtuner64.msi)  

Build
======

After cloning the repository and dependencies, here are the steps to build MTuner.

**MinGW**

	$ cd MTuner/genie
	$ genie --gcc=mingw-gcc gmake
	$ cd ../../.build/windows/mingw-gcc/projects/MTuner
	$ make
MINGW environment variable must be set and point to the MinGW installation directory.  
Tested with [TDM64 MinGW](http://tdm-gcc.tdragon.net/download) using [OpenMP package](http://sourceforge.net/projects/tdm-gcc/files/TDM-GCC%205%20series/5.1.0-tdm64-1/gcc-5.1.0-tdm64-1-openmp.zip/download)

**Visual Studio**

	> cd MTuner/genie
	> genie vs2015
Solution will be located here: *{Clone root}/.build/windows/vs2015/projects/MTuner/MTuner.sln*

Documentation
======

Documentation is currently hosted on [MTuner website](http://mtuner.net).  
Starting page of documentation is [here](http://mtuner.net/documentation.html)  

Support development
======

**MTuner** is free and will remain so but there's plenty more features and polish to do.  
Consider donating to support the ongoing development and maintenance of **MTuner**

Monthly donations:  
[<img src="https://s3-us-west-1.amazonaws.com/patreon-reward-images/1537701.png" height=70>](https://www.patreon.com/MTuner)

One time donations:  
[<img src="https://www.paypalobjects.com/webstatic/mktg/merchant_portal/button/donate.en.png" width=228 height=44>](https://www.paypal.me/MTuner)

For private support and similar requests, please contact the author - see below.

Author
======

The author of **MTuner** is Milos Tosic  
[ <img src="https://github.com/milostosic/build/blob/master/img/twitter.png">](https://twitter.com/milostosic)[ <img src="https://github.com/milostosic/build/blob/master/img/linkedin.png">](https://www.linkedin.com/in/milostosic/)[ <img src="https://github.com/milostosic/build/blob/master/img/mail.png">](mailto:milostosic77@gmail.com)  

License (BSD 2-clause)
======

<a href="http://opensource.org/licenses/BSD-2-Clause" target="_blank">
<img align="right" src="http://opensource.org/trademarks/opensource/OSI-Approved-License-100x137.png">
</a>

	Copyright (c) 2017 Milos Tosic. All rights reserved.
	
	https://github.com/milostosic/MTuner
	
	Redistribution and use in source and binary forms, with or without
	modification, are permitted provided that the following conditions are met:
	
	   1. Redistributions of source code must retain the above copyright notice,
	      this list of conditions and the following disclaimer.
	
	   2. Redistributions in binary form must reproduce the above copyright
	      notice, this list of conditions and the following disclaimer in the
	      documentation and/or other materials provided with the distribution.
	
	THIS SOFTWARE IS PROVIDED BY COPYRIGHT HOLDER ``AS IS'' AND ANY EXPRESS OR
	IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
	MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
	EVENT SHALL COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
	INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
	(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
	LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
	ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
	(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
	THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. 
