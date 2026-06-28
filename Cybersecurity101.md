# Try Hack Me
## Cybersecurity 101
- offensive security red teaming pentesters are basically methodologies and individuals that
  hack a system in an ethical legal way to find flaws and weaknesses and vulnerabilities
  before a real attacker does and for this first you need to understand the system find the
  vulnerabilities and then exploit them in websites first in order to find hidden or all the
  directories or web pages we use the dirb domain or url or use the gobuster tool with
  command: gobuster dir --url http://www.onlineshop.thm/ -w /usr/share/wordlists/dirbuster/
  directory-list.txt and when a secret page is found that can give privilage level or give
  some sort or administrator role we exploit that by either bruteforcing the password or
  do a dictionary attack for dictionary attack we use hydra for passwords if the admin name
  is know : hydra -l admin -P passlist.txt www.onlineshop.thm http-post-form "/login:username
  =^USER^&password=^PASS^:F=incorrect" -V first they do enumeration that is finding and
  gethering information related to the system this process is done by both the red teamers
  are black hat hackers
- defensive security blue teaming and methodologies used for defending and protecting a system
  against malacious actors they maintain the  cia triad methodology and for this they have
  to first understand the system and then secure it from hackers and monitor the activity in it
  they prevent detect and mitigate attacks
- shodan is the tools used as a browser for iot devices like it deals with all the devices that
  have a public ip and scans them for open ports servers gives details to them like versions
  countries
- virustotal is a tool that lets user scan a file a url a domain against 70+ known virus
  detection engine adn scanners that will flag the input and give off the malacious factor
  score
- cve common vulnerability and exposure is a database for all the known vulnerabilities in
  this database their are vulnerabilities with naming as cve-year-unique number we can check
  cves and their cvss commom vulnerability scoring system in cve official website nist nvd
  national vulnerability database and also for proof of concepts and exploit codes we can use
  github which also has detailed technical reports for a cve 
- in linux if a user wants to get details about a cerrtain tool or commad they use man or -h
  for it like man toolname/command or toolname/command -h man stands for manual and h stands
  for help we can alos use whatis command/toolname
- Linux is basically an os kernel that was built by linus torvalds and it was bundled with
  GNU softwares and packages to create an os called GNU/linux which is basically the parent os
  for all the distributions that are existing today like ubuntu debian kali linux rhel fedora etc
- now some bash commands
  ``` bash
  echo hello world  // give us the output on the screen
  whoami  // tells us about the current user
  ls  // lists all the files and directories in the current folder
  cd foldername  // change the directory to teh name mentioned
  cd ..  // goes back one directory
  cat filename  // outpust the text in the file on the screen
  pwd  // prints working directory or current directory
  find -name filename.txt  // finding the file in a directory
  find -name *.txt  // the wildcard is used for finding all the files with the .txt extension
  find . -type d -name "directory name"  //  . for searching within active directory or ~ for home directory or / for root directory
  touch filname  // to create a file
  echo "hello"  // to write content
  echo "text" > filename or >>filename
  nano filename  // used for booting the text editor
  rm filename  // delating a file
  rm -rf foldername  // deleting a folder
  ssh username@ipaddress  // secure shell
  su - root  // for root access
  su - username  // switching users
  history  // command for checking the command typed in the past
  ```
