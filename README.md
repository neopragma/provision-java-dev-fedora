# provision-java-dev-training-vm

Provision an instance of Fedora Linux with software to support programming exercises for a training course in Test-Driven Development and Object-Oriented Design in Java. Once you have a provisioned VM, you can clone git repositories for one or more sample projects designed for use in training classes. These instructions are used by an instructor preparing a VM to be copied and distributed to participants in a training class.

## Steps

The instructions assume you will provision a virtual machine with Fedora Linux. This has been tested with the following operating systems:

* Fedora GNU/Linux 3.11.10-301.fc20.x86_64 

### Step 1 - Download Fedora iso

Open a browser and navigate to http://fedoraproject.org. Download the iso for the version of Fedora you want to install.

### Step 2 - Create VM

Using the virtualization product you want your students to use, create a VM and install Fedora on it. This procedure has been tested with the following virtualization products:

* VMware Player 6.0.2 Linux 64-bit

### Step 3 - Install git

 Install git.

```shell
sudo yum install git
```

### Step 4 - Clone this repo

With git installed, you can load this provisioning project on the new instance:

```shell
cd
git clone https://github.com/neopragma/provision-java-dev-training-vm-fedora
```

### Step 5 - Run the setup script

Run the setup script.

```shell
cd ~/provision-java-dev-training-vm-fedora
./setup
```

### Step 6 - Verify the setup

The last thing the setup script does is to run a script named verify. Check the output from verify and see if any of the installation steps failed. If so, investigate and resolve the problems. If you discover a problem with the setup script, fix it and make a pull request.

### Step 7 - Install course-specific project(s)

At this point, the VM is ready to support Java training course projects available from Neo Pragma LLC Github repositories.






