## Setting up module command on debian <tested on> [
Check OS properties  using ``` lsb_release -a ``` or just cat ``` cat /etc/os-release ``` for yours.
###Tested on ``` 6.0.0-2parrot1-amd64 ```

## Confirm ```tcl``` and ```tclx8.6``` packages are installed 
## For tcl* related packages install using
```
$ sudo apt install tcl* -y
```
```
$ curl -LJO https://github.com/cea-hpc/modules/releases/download/v5.1.1/modules-5.1.1.tar.gz
$ tar xfz modules-5.1.1.tar.gz
$ cd modules-5.1.1
$ sudo ./configure
$ sudo ./make
$ sudo make install
$ PREFIX='/usr/local/Modules'
$ sudo ln -s $PREFIX/init/profile.sh /etc/profile.d/modules.sh
$ sudo ln -s $PREFIX/init/profile.csh /etc/profile.d/modules.csh
$ source /usr/local/Modules/init/bash
```

## All set 
## sanity check ```[ OK ] ```
## module check ```[ Ok ] ```
use module manual for ```usage```
