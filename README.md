# CS-470-Operating-Systems-Homework-1-solution

Download Here: [CS 470 ­ Operating Systems Homework 1 solution](https://jarviscodinghub.com/assignment/cs-470-operating-systems-homework-1-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

The purpose of this homework is provide experience with using a virtual machine (VM) and developing a
(trivial) kernel module in Linux.
(15 points) This assignment consists of three parts: creating a virtual machine, creating a simple kernel module
that can be loaded and removed from the kernel, and using the kernel linked list structure.
For the virtual machine, use VirtualBox. VirtualBox is available on the lab machines (both Linux and
Windows), or can be downloaded from the VirtualBox website (https://www.virtualbox.org) and installed.
The file /home/hwang/cs470/hwk1/cs470­ubuntu.zip on csserver is a zipfile containing a
VirtualBox virtual disk image (cs470­ubuntu.vdi) that is to be used to create a virtual Linux machine.
Copy the zipfile to your own development space. Extract the VDI files from the zipfile. (Please note that the
zipfile is about 3GB and the extracted VDI file is about 7GB. ) To create the VM do the following:
1. Start up VirtualBox, click on the New button. This will open the VM wizard for creating a new VM.
2. Give your VM a name like “cs470­ubuntu”. The OS type is ubuntu, and the version should be 64­bit,
then click Next. If there is only 32­bit for version, you either have a 32­bit machine, in which case you’ll
need to do this assignment on a lab machine. Or you need to turn on hardware virtualization (in
particular, HP machine have it turned off by default) in which case, you’ll need go into the BIOS settings
and turn it on, then try again.
3. Set base memory size to 2048 GB, and click Next.
4. Click on the radio button for “Use an existing virtual hard disk file”. Browse to the VDI file (cs470­
ubuntu.vdi), then click Create.
5. To start a VM, select it, then click on the Start button. The OS will boot up. The default user name is
cs470admin and the password is GoPurpleAces!. This account has administrator privileges, which
means the it can run the sudo command by providing the account password.
Implement the Linux Kernel Module project on pages 96­101 of the textbook using this VM. In the
homework1 directory of the cs470admin account, there are two files: a kernel module stub (simple.c) and a
makefile. The makefile will compile the stub into a kernel module as described in the textbook. You should not
change the makefile or the names of the files.
Implement the Linux Kernel Module project as outlined in the textbook. The coding for this homework is to be
done individually, though you can confer with others regarding how to use the kernel data structures and
commands. Note that the purpose of this assignment is deal with allocating kernel structures on loading the
module and deallocating them upon removing the module, so the birthday list should not be deallocated until the
module is removed. To demonstrate this, the simple_exit function should print out each node’s data before
deallocating it.
01/15/2017 Page 1 of 2 D. Hwang
(5 points) Demonstrate the project to the instructor as outlined in the textbook no later than 5:00pm on
Wednesday, January 24. Appointments may be made during most times the instructor does not have scheduled
activities. Demos may be attempted at most two times after which late penalties for this portion will accrue per
attempt.
What to Submit
Create a tarfile or a zipfile containing a well­documented simple.c file and the makefile for the kernel
module. Submit your archive using the submission system (https://submission.evansville.edu) by 11:59pm on
Wednesday, January 24, for full credit (i.e., use a web browser in the VM). Your username for this course is
your ACENET username with suffix “­cs470” appended to it (e.g. dh27­cs470), and your password is your
student ID number including the leading 0 (i.e. 7 digits). The grading script only will accept submissions. It
will not run anything.

