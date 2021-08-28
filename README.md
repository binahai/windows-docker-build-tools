# windows-docker-build-tools

A Dockerfile to be downloaded for building the image presented in - https://docs.microsoft.com/en-us/visualstudio/install/build-tools-container?view=vs-2019

This recipe includes the following packages:

- [Chocolatey](https://chocolatey.org/)
- [CMake](https://cmake.org/)
- [Git](https://community.chocolatey.org/packages/git) (and Bash)
- [Info-ZIP (unzip)](https://community.chocolatey.org/packages/unzip)
- [llvm](https://community.chocolatey.org/packages/llvm)
- [Python](https://www.python.org/)
- [Vim](https://community.chocolatey.org/packages/vim)
- [Visual Studio Workload VCTools](https://community.chocolatey.org/packages/visualstudio2019-workload-vctools)

## Getting Started

Download the Dockerfile file

```bash
curl -sL -o Dockerfile.buildtools "https://raw.githubusercontent.com/binahai/windows-docker-build-tools/master/Dockerfile.buildtools"
```
