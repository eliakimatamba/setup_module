## setting up module command on debian <tested on> 
check OS properties  using ``` lsb_release -a ``` or just cat ``` cat /etc/os-release ``` for yours.
Tested on ``` 6.0.0-2parrot1-amd64 ```
```
$ curl -LJO https://github.com/cea-hpc/modules/releases/download/v5.1.1/modules-5.1.1.tar.gz
$ tar xfz modules-5.1.1.tar.gz
