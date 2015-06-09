# Installing Virtual Box and Vagrant #

## Virtual Box ##

1. Go to the following [link](https://www.virtualbox.org/wiki/Downloads).
2. Select the appropriate download for your operating system (Mac, Windows, Linux, etc...)

## Vagrant ##

1. Go to the following [link](https://www.vagrantup.com/downloads.html).
2. Select the appropriate download for your operating system (Mac, Windows, Linux, etc...)

## Testing your Installation ##

1. On your desktop (or another convenient location) create a new empty folder. You can name it something obvious like "test."
2. Open a bash shell.
3. Change directories to the new test folder you created.

  cd desktop/test
  
4. Enter the following two commands in your bash shell:

  vagrant init hashicorp/precise64
  
  vagrant up

These two commands will first download a very basic 64-bit virtual machine and then attempt to build it. If they run successfully, then you know that you have correctly installed your virtual machine software. If they do not run successfully, you should reinstalled Virtual Box and Vagrant and try again.
