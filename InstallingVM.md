# Installing the HMT VM #

Prerequisites:
- git
- vagrant
- virtual box

1. Open a terminal session.
2. Change directories to where you want to install the virtual machine (e.g. to go to your desktop enter the following: cd Desktop)
3. Download the vagrant file from [github](https://github.com/homermultitext/vm2015). Copy the clone URL and enter the command (git clone). It should look like this:

    git clone https://github.com/homermultitext/vm2015.git

4. Change directories to the VM (cd vm2015).
5. Run the command: vagrant up (This will start the virtual machine, and the first time you do it, it will build the VM from scratch).
6. Find something to occupy yourself for awhile. It is a lengthy process, especially if multiple people are using the same network to build a vm. Make sure you have a good internet connection and don't forget you're building a machine and do something silly like shut your laptop. It has happened.
7. You will be prompted with a login screen. The username and password are both 'vagrant'.
8. When you are done working in the virtual machine, you can log out.
9. Back in your terminal window you need to run the command: vagrant halt. This is equivalent to shutting down the machine. You will want to remember to do this because otherwise the machine will keep running and draining your battery.
10. Helpful documentation about the VM can be found [here](http://homermultitext.github.io/vm2015/)
