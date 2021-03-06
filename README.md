# Tag My Outfit - gRPC Interface

## Overview

This project defines the gRPC interface for the Tag My Outfit Service. The service aims to classify clothing parts within a set a categories as well as predict attributes for such parts.

This interface is implemented by a gRPC server with the service above mentioned and can be used by the clients to communicate with such server.

## Technologies

 * [gRPC](https://grpc.io)

 * [Python](https://www.python.org)

## Usage

### Python package

#### Install

This project offers a python package with the gRPC generated sources. The package can be locally installed by executing the following steps:

 * Clone the github repository *(Specific versions are marked by tags)*:

 ```
 $ git clone https://github.com/sipg-isr/tag_my_outfit_interface.git
 ```

 * Inside the project folder, navigate to the python folder:

 ```
 $ cd python
 ```

 * Install the interface package *(This step will also install the grpcio-tools package to generate the gRPC code)*:

 ```
 $ make
 ```

 * Remove the generated gRPC sources *(This is a cleaning step and is not necessary for the package installation)*:

 ```
 $ make clean_sources
 ```

 * Remove the grpcio-tools package *(The package is only used to generate the sources and can now be deleted)*:

 ```
 $ make clean_tools
 ```

#### Uninstall

The package can be uninstalled by execution one of the following options:

 * Using pip:

 ```
 $ pip uninstall -y outfit-tagging-interface
 ```

 * Using the provided Makefile inside the python folder:

 ```
 $ make uninstall
 ```

### Proto compiler

The project [service proto file](proto/outfit_tagging/interface/service.proto) can also be downloaded and manually compiled with the proto compiler for any supported language.

## License

This project is released under the [MIT License](LICENSE.md).
