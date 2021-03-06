edu_web_scraper

Overview:<br/>
edu_web_scraper scrapes the web, specifically google search results for gender and educational information
based on full name and email address.

It takes a csv file as input with full name and email address columns. It runs google search on each name
and/or email address and scrapes the educational degree and educational institution associated with each name
and/or email adddress. It also scrapes genderize.io and behindthename.com for gender information
based on first name.

At this point it is a Python script. There is no UI to speak of. To run it in your terminal specify 
the script file and test names/emails csv file to be discovered:<br/>

python gapjump.py test_profiles.csv

Upon completion pie chart is saved to your local directory/machine with the degree breakdown
among the individuals listed in the csv file.

## Table of Contents📖

* [Tech Stack](#tech-stack)
* [Setup/Installation](#installation)
* [To-Do](#future)
* [License](#license)

## <a name="tech-stack"></a>Tech Stack

__Backend:__ Python 2.7, Matplotlib, Mechanize, BeautifulSoup <br/>
__Database:__ Postgres<br/>

## <a name="installation"></a>Setup/Installation

####Requirements:

- PostgreSQL
- Python 2.7
- Vagrant/VM set up 'vagrant' db

To have this app running on your local computer, please follow the below steps:

Clone repository:
```
$ git clone https://github.com/skakanka/edu_web_scraper.git
```
Create a virtual environment:
```
$ virtualenv env
```
Activate the virtual environment:
```
$ source env/bin/activate
```
Install dependencies:
```
$ pip install -r requirements.txt
```
Run the app from the command line.
```
$ python gapjumper.py test_profiles.csv
```

## <a name="future"></a>TODO
* Find a way to use LinkedIn API
* Use OAuth
* Create User Interface
* Evaluate ways to encrypt data before it is stored in db
* Fine tune scraping to get more accurate results


## <a name="license"></a>License

The MIT License (MIT)
Copyright (c) 2017 Anka Kondraska 

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.