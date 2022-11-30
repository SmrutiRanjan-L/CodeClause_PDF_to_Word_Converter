# CodeClause_PDF_to_Word_Converter

### Introduction

The website http://pdf2doc.com/ offers the ability to convert PDF files to Word documents online. During testing, it was found to be a better converter than many other online and offline alternatives. I wanted to develop a local client that utilized this website behind the scenes.

### Dependencies

* [Python 2.7+](https://www.python.org/downloads/)
	* Comes preinstalled on most Linux and OS X versions
* [requests](http://docs.python-requests.org/en/master/)
	* `pip install requests`

* [requests-toolbelt](https://github.com/sigmavirus24/requests-toolbelt)
	* `pip install requests-toolbelt`

Windows and OS X binaries will be available soon.

[//]: # "Make sure UI looks right!"

### Usage

Via console:
>python main.py pdf

Alternatively, in Windows, you can simply drag a PDF over `main.py` to begin the procedure. This is because, in Windows, any file dragged over an executable is added as a command line argument.

The file must end in `pdf`. The software will open up a window where you can view the progress of the conversion and any errors that may be encountered. Finally, the converted `doc` will be downloaded and placed into the same directory as the executable.

### Exploration

The process of reverse engineering http://pdf2doc.com/ was outlined in [EXPLORATION.md](/EXPLORATION.md).

### Next Steps

* Simplify code?

* Windows release

* OS X release?
	* Can be done with py2app
	* OS X already comes with Python, so the only trouble saved will be through avoiding dependencies

