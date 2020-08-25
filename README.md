# Python3.8

```
user1@debian:~$ sudo add-apt-repository ppa:deadsnakes/ppa
[sudo] password for user1: 
 This PPA contains more recent Python versions packaged for Ubuntu.

Disclaimer: there's no guarantee of timely updates in case of security problems or other issues. If you want to use them in a security-or-otherwise-critical environment (say, on a production server), you do so at your own risk.

Update Note
===========
Please use this repository instead of ppa:fkrull/deadsnakes.

Reporting Issues
================

Issues can be reported in the master issue tracker at:
https://github.com/deadsnakes/issues/issues

Supported Ubuntu and Python Versions
====================================

- Ubuntu 16.04 (xenial) Python 2.3 - Python 2.6, Python 3.1 - Python3.4, Python 3.6 - Python3.9
- Ubuntu 18.04 (bionic) Python2.3 - Python 2.6, Python 3.1 - Python 3.5, Python3.7 - Python3.9
- Ubuntu 20.04 (focal) Python3.5 - Python3.7, Python3.9
- Note: Python2.7 (all), Python 3.5 (xenial), Python 3.6 (bionic), Python 3.8 (focal) are not provided by deadsnakes as upstream ubuntu provides those packages.
- Note: for focal, older python versions require libssl1.0.x so they are not currently built

The packages may also work on other versions of Ubuntu or Debian, but that is not tested or supported.

Packages
========

The packages provided here are loosely based on the debian upstream packages with some modifications to make them more usable as non-default pythons and on ubuntu.  As such, the packages follow debian's patterns and often do not include a full python distribution with just `apt install python#.#`.  Here is a list of packages that may be useful along with the default install:

- `python#.#-dev`: includes development headers for building C extensions
- `python#.#-venv`: provides the standard library `venv` module
- `python#.#-distutils`: provides the standard library `distutils` module
- `python#.#-lib2to3`: provides the `2to3-#.#` utility as well as the standard library `lib2to3` module
- `python#.#-gdbm`: provides the standard library `dbm.gnu` module
- `python#.#-tk`: provides the standard library `tkinter` module

Third-Party Python Modules
==========================

Python modules in the official Ubuntu repositories are packaged to work with the Python interpreters from the official repositories. Accordingly, they generally won't work with the Python interpreters from this PPA. As an exception, pure-Python modules for Python 3 will work, but any compiled extension modules won't.

To install 3rd-party Python modules, you should use the common Python packaging tools.  For an introduction into the Python packaging ecosystem and its tools, refer to the Python Packaging User Guide:
https://packaging.python.org/installing/

Sources
=======
The package sources are available at:
https://github.com/deadsnakes/

Nightly Builds
==============

For nightly builds, see ppa:deadsnakes/nightly https://launchpad.net/~deadsnakes/+archive/ubuntu/nightly
 More info: https://launchpad.net/~deadsnakes/+archive/ubuntu/ppa
Press [ENTER] to continue or ctrl-c to cancel adding it

gpg: keybox '/tmp/tmpp47as7og/pubring.gpg' created
gpg: /tmp/tmpp47as7og/trustdb.gpg: trustdb created
gpg: key BA6932366A755776: public key "Launchpad PPA for deadsnakes" imported
gpg: Total number processed: 1
gpg:               imported: 1
gpg: no valid OpenPGP data found.


user1@debian:~$ sudo apt-get update
Ign:1 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy InRelease                                                                                
Hit:2 http://security.debian.org/debian-security stretch/updates InRelease                                                                           
Ign:3 http://ftp.ua.debian.org/debian stretch InRelease                                                                            
Hit:4 http://security.debian.org stretch/updates InRelease                                                                                           
Ign:5 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy InRelease                                                                             
Hit:6 http://ftp.ua.debian.org/debian stretch Release                                                                          
Ign:7 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy Release                                                                 
Ign:8 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy Release                                                              
Ign:9 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 Packages                           
Ign:10 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all Packages                                                      
Ign:11 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en_US                                                 
Ign:12 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en                                                    
Ign:13 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 DEP-11 Metadata                                             
Ign:15 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all DEP-11 Metadata                                              
Ign:16 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main DEP-11 64x64 Icons                     
Ign:17 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all Packages                        
Ign:18 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 Packages                       
Ign:19 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en
Ign:20 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en_US
Ign:21 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:22 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:23 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Ign:9 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 Packages
Ign:10 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all Packages
Ign:11 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en_US
Ign:12 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en
Ign:13 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:15 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:16 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Ign:17 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all Packages
Ign:18 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 Packages
Ign:19 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en
Ign:20 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en_US
Ign:21 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:22 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:23 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Ign:9 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 Packages
Ign:10 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all Packages
Ign:11 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en_US
Ign:12 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en
Ign:13 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:15 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:16 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Ign:17 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all Packages
Ign:18 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 Packages
Ign:19 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en
Ign:20 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en_US
Ign:21 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:22 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:23 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Ign:9 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 Packages
Ign:10 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all Packages
Ign:11 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en_US
Ign:12 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en
Ign:13 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:15 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:16 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Ign:17 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all Packages
Ign:18 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 Packages
Hit:24 http://packages.dotdeb.org stretch InRelease
Ign:19 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en
Ign:20 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en_US
Ign:21 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:22 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:23 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Ign:9 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 Packages
Ign:10 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all Packages
Ign:11 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en_US
Ign:12 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en
Ign:13 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:15 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:16 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Ign:17 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all Packages
Ign:18 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 Packages
Ign:19 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en
Ign:20 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en_US
Ign:21 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:22 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:23 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Err:9 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 Packages
  404  Not Found [IP: 91.189.95.83 80]
Ign:10 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all Packages
Ign:11 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en_US
Ign:12 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main Translation-en
Ign:13 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:15 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:16 http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Ign:17 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all Packages
Err:18 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 Packages
  404  Not Found [IP: 91.189.95.83 80]
Ign:19 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en
Ign:20 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main Translation-en_US
Ign:21 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main i386 DEP-11 Metadata
Ign:22 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main all DEP-11 Metadata
Ign:23 http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy/main DEP-11 64x64 Icons
Reading package lists... Done                       
W: The repository 'http://ppa.launchpad.net/deadsnakes/ppa/ubuntu groovy Release' does not have a Release file.
N: Data from such a repository can't be authenticated and is therefore potentially dangerous to use.
N: See apt-secure(8) manpage for repository creation and user configuration details.
W: The repository 'http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu groovy Release' does not have a Release file.
N: Data from such a repository can't be authenticated and is therefore potentially dangerous to use.
N: See apt-secure(8) manpage for repository creation and user configuration details.
E: Failed to fetch http://ppa.launchpad.net/deadsnakes/ppa/ubuntu/dists/groovy/main/binary-i386/Packages  404  Not Found [IP: 91.189.95.83 80]
E: Failed to fetch http://ppa.launchpad.net/gwibber-daily/ppa/ubuntu/dists/groovy/main/binary-i386/Packages  404  Not Found [IP: 91.189.95.83 80]
E: Some index files failed to download. They have been ignored, or old ones used instead.

user1@debian:~$ sudo apt-get install python3.8
Reading package lists... Done
Building dependency tree       
Reading state information... Done
E: Unable to locate package python3.8
E: Couldn't find any package by glob 'python3.8'
E: Couldn't find any package by regex 'python3.8'
```
