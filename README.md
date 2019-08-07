# Useful Bash Scripts 
My personal list of useful bash scripts for grad school. 

 **List of Scripts** 
* *mountwc*   - For mounting the wheelchair working directory over ssh on a remote machine for software development on the remote machine *this logs into chris@wc by default*
* *unmountwc* - To unmount the above wheelchair's directory over ssh on a remote machine
* *wclogin*   - To log into the wheelchair over remote and launch byobu
* *myDocker*  - To launch my docker container on the wheelchair
* *newDocker* - To create a new docker container instance
* *quickrviz* - To launch rviz for the wheelchair 

**Requirements** 
* basic_perp.rviz to be placed in /home/chris/.rviz
* Install `sshpass` by running `sudo apt-get install sshpass`; [link to sshpass](https://gist.github.com/arunoda/7790979). This is for autologin for logging into the wheelchair and other systems. **Do not use this for logging into the secure file storage. This stores your password in plaintext and would leave you at risk for identity theft and make our fileshare non-IRB compliant.**
* After cloning the repository, edit mountwc for your user account/password if you wish to use this script. 

Passwords not provided and need to be manually entered for security. 

**Installation**
* 0) Ensure all requirements above are met. 
* 1) Clone this repository into your home directory by running: `cd ~/ && git clone https://github.com/chrisxmiller/usefulbashscripts.git`
* 2) Check out the list below of scripts and delete any you don't like and 
* 3) Edit your bashrc so that Ubuntu knows where to find your bash scripts. Open this file by running `code $HOME/.bashrc` (assumes you're using Visual Studio Code as your text editor. If you're using Sublime use `subl` and if you're using Atom use `atom` in-lieu of `code`). 
* 4) Append to the bottom of the bashrc file the following line: `export PATH="$HOME/usefulbashscripts:$PATH"`
* 5) Save the bashrc file, close, and then reopen your terminal. Then, reopen the terminal. 
* 6) Check that the scripts run by trying to run one of them. 
