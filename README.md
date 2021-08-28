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

### Download the Dockerfile file

```bash
mkdir -p "c:/temp/emptydir"
curl -sL -o "c:/temp/emptydir/Dockerfile.buildtools" "https://raw.githubusercontent.com/binahai/windows-docker-build-tools/master/Dockerfile.buildtools"
```

### Build Docker image

This step is done on an EC2 that is based on the **Windows Docker Build Dotnet SDK** AMI.

```bash
mkdir -p "c:/temp/emptydir"
docker build -m 4G -t "buildtools2019" -f "c:/temp/emptydir/Dockerfile.buildtools" "c:/temp/emptydir"
```
