## Contents
* [About EbookScrapper](https://github.com/nntoan/ebookscrapper#ebookscrapper)
* [Help & Usage Instructions](https://github.com/nntoan/ebookscrapper#help--usage)
* [Example Usage](https://github.com/nntoan/ebookscrapper#example-usage)
* [Screenshots](https://github.com/nntoan/ebookscrapper#screenshots)

# EbookScrapper 

```
       ____              _                     
      |  _ \            | |                    
   ___| |_) | ___   ___ | | __                 
  / _ \  _ < / _ \ / _ \| |/ /                 
 |  __/ |_) | (_) | (_) |   <                  
  \___|____/ \___/ \___/|_|\_\                 
    _____
   / ____|                                     
  | (___   ___ _ __ __ _ _ __  _ __   ___ _ __ 
   \___ \ / __| '__/ _` | '_ \| '_ \ / _ \ '__|
   ____) | (__| | | (_| | |_) | |_) |  __/ |   
  |_____/ \___|_|  \__,_| .__/| .__/ \___|_|   
                        | |   | |              
                        |_|   |_|              

                                 By : Toan Nguyen
```

It is simple, easy, and fast command line tool to download ebook's and save them in a directory. It is compatible with Python 2.7.x+ and Python 3.3.x+.

Ebook's are scrapped from [AllItEbooks](http://www.allitebook.com/). All these customizations are provided by this tool in addition to several others.

** EbookScrapper** makes use of 3rd party libraries for HTTP Requests and HTML processing. You need to fulfill these requirements before using this tool.

Fulfill the requirements by executing the following in bash shell.

```	
pip install -r requirements.txt
```

The *requirements.txt* file is present in the repo.

# Help & Usage


	usage: ebookscrapper.py [-h HELP] [-l LOCATION]
	                [-le LASTEST] [-n EBOOK_NAME] 

    EbookScrapper is simple, easy, and fast CLI tool to download ebook's and also
    save them in current directory.

    optional arguments:
      -h, --help            show this help message and exit
      -n, --name            Download a specified ebook by its name.
      -i, --isbn            Download a specified ebook by ISBN-10.
      -c, --category        Download all ebooks in a specified category.
      -l LOCATION, --location LOCATION
                            The location where ebook has to be downloaded. By
                            default stored in the current directory.
      -le, --latest         Download the newest version of an eBook.
							

# Example Usage


#### To download all ebooks or just one specified ebook

	python ebookscrapper.py <ebook_name>
						or
	python ebookscrapper.py <isbn>
	
*Example:-* 	

	python ebookscrapper.py "Reactive Web Applications"

	python ebookscrapper.py 1786460300

#### To download all ebooks in a specified category

	python ebookscrapper.py -c <category-name>
						or
	python ebookscrapper.py --category <category-name>
	
*Example:-*

	python ebookscrapper.py --category "Programming"

#### To download the latest eBooks.

	python ebookscrapper.py <ebook_name> -le
	                or
	python ebookscrapper.py <ebook_name> --latest

*Example:-*

	python ebookscrapper.py "Reactive Web Applications" --latest


## Screenshots

Downloading all ebooks from "Programming"

![Downloading ebooks in "Programming"](http://i.imgur.com/.png)
---

Help Options

![Help Options](http://i.imgur.com/.png)
---

Directory structure.

![Usage Demo and Directory Structure made](https://i.imgur.com/.png)
---
