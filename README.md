## Why
### Container VS direct installation

* Good software nowadays runs across platforms. The main purpose of using a container is not to run Linux programs in Windows or Mac.
* A direct installtion may cost time and require knowledge about a particular piece of software that is not important for regular users. A container of a set of common software helps save time and effort for both experienced and new users.

### Docker VS Singularity

* Singularity is needed for running parallele jobs on a Linux HPC cluster as there are security concerns to run Docker images there.
* Docker Desktop on Windows uses WLS2, which is more lightweighted and better integrated with Windows than VirtualBox that is used by Singularity on Windows. A detailed comparison between various VM solutions can be found [here](https://www.quora.com/Should-I-use-Linux-on-VM-or-in-Windows-Subsystem)
* [ROOT][] provides Docker images, which can be used by Singularity.

The best solution would be to develop Docker image reciepes for Windows and Mac users and use those images through Singularity in a Linux cluster.

[ROOT]: http://root.cern.ch
