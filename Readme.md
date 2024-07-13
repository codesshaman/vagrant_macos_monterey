# Vagrant virual machine with MacOS

Your need install vagrant and vmware for up this configuration.

Your need install [vagrant](https://github.com/hashicorp/vagrant-installers/releases/tag/v2.3.4.dev%2Bmain "vagrant") and  [vmware](https://www.vmware.com/ "vmware") for up this configuration. Optional you can use [make](https://www.gnu.org/software/make/ "make").

### Step 1

Download box droy/macMonterey for vmware from [vagrantup](https://app.vagrantup.com/droy/boxes/macMonterey "vagrantup").

### Step 2

Clonr this repository: git clone https://github.com/codesshaman/vagrant_macos_monterey.git

### Step 3

Copy box and go inside the repository folder:

``mv ~/Downloads/b842e537-cddc-415a-8a34-edfd19c56638 path_to/vagrant_macos_monterey/macos``

``cd vagrant_macos_monterey``

### Step 4

Inicialize configuration:

``vagrant box add droy/macMonterey debian``

or with make:

``make build``

### Step 5

Install configuration:

``vagrant up --provider=vmware_desktop``

or with make:

``make``

### Step 6

WinRM transport may not set, you can install vbox guest addition in the ssl installation step and abort vagrant installing. All be work.

### Step 7

Connect to centos:

``ssh vagrant@192.168.58.108``

or with make:

``make connect``
