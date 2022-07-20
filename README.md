# INE-DL (INE course downloader)

[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Anon-Exploiter/ine-dl.js/graphs/commit-activity)
[![python](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/)
![GitHub](https://img.shields.io/github/license/Anon-Exploiter/ine-dl)
![GitHub closed issues](https://img.shields.io/github/issues-closed/Anon-Exploiter/ine-dl)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Follow%20%40syed_umar)](https://twitter.com/syed__umar)
[![LinkedIn][linkedin-shield]][linkedin-url]

[contributors-shield]: https://img.shields.io/github/contributors/Anon-Exploiter/ine-dl.svg?style=flat-square
[contributors-url]: https://github.com/Anon-Exploiter/ine-dl/graphs/contributors
[issues-shield]: https://img.shields.io/github/issues/Anon-Exploiter/ine-dl?style=flat-square
[issues-url]: https://github.com/Anon-Exploiter/ine-dl/issues
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/syedumararfeen/

**Python script to download INE courses including labs, exercises, quizzes, slides, and, videos!**

<img src="https://user-images.githubusercontent.com/18597330/179950027-c5856feb-bec0-4d32-bae9-0998fbb715a8.png" />


### Requirements

- Python (3.6.* - 3.8.*)
- Python `pip3`
- Python module `requests_toolbelt`
- Python module `requests`
- Python module `loguru`


### Install modules

	pip3 install -r requirements.txt
	

### Works on

- ~Windows 7/8/8.1~ (It should work fine in WSL but not in cmd/PS)
- Ubuntu 18.04 LTS
- Ubuntu 20.04 LTS
 

### Download ine-dl

You can download the latest version of ine-dl by cloning the GitHub repository.

	git clone https://github.com/Anon-Exploiter/ine-dl --depth 1


### Usage

***Running the Script (displays help menu with no args)***

	python ine-dl.py

***Listing all the courses***

	python ine-dl.py -lc

***Listing course categories***

	python ine-dl.py -lct 

***Listing all the courses of a specific category***

	python ine-dl.py -lcct {category_id}

***Logging the script's output into a log file***

	python ine-dl.py <general_args> -l logfile.log

***Downloading all the INE course (your subscription has access to, with/without parallel processing)***

	python ine-dl.py --all
    python ine-dl.py --all -p 2

***Downloading a single course***

	python ine-dl.py -c {course_id}

***Downloading all courses of specified category (with/without parallel processes)***

	python ine-dl.py -ct {category_id}
    python ine-dl.py -ct {category_id} -p 2
	

### To DOs
- [x] Fetch all the courses and write into a file
- [x] Fetch & Match the subscriptions and then put stuff into the course file
- [x] Implement downloading of video files (highest resolution and so-on)
- [x] Implement quiz downloading
    - [x] Write the quizzes into an text file and then write it's correct results (json:is_correct) into another file!
- [x] Implement exercise downloading
- [x] Implement iframe downloading
    - [x] Implement html, css, js, woff, img files downloading
- [x] Implement lab downloading
    - [x] Check if description_html exists and if not, write the json object of the whole lab for user satisfaction
- [x] Downloading the files_uuids zip/pdf files
- [x] Write a json into the course directory containing whole course data
- [x] Implement all argparse arguments


### Screenshots

<img src="https://user-images.githubusercontent.com/18597330/179950027-c5856feb-bec0-4d32-bae9-0998fbb715a8.png" />
<img src="https://user-images.githubusercontent.com/18597330/179954269-c4d4b09b-a023-429d-b6d8-2082423ce8ff.png" />
<img src="https://user-images.githubusercontent.com/18597330/179954376-31f59667-b64d-4ee4-8888-a05564a9128a.png" />
<img src="https://user-images.githubusercontent.com/18597330/179954527-c6709ede-6172-4b0e-a548-dab47d4233d6.png" />


### Note 
Please use the script w.r.t the usage guidelines of INE. Do not exhaust their backend servers. Do not dump and share the courses publicly. 

Please use this on your own risk, If your account is blocked by the usage of this script, I won't be responsible. 
