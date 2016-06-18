# Simplified environment for building CirrOS images.

This is an Ubuntu 12.04 based image which can be utilized to build CirrOS images for the x86_64 architecture.
Currently, the latest stable version of CirrOS and the corresponding pre-built version of buildroot is used.

## Usage

`docker run --privileged -i -v $OUTPUT_DIR:/root/images -t hferenc/cirros-image-builder`

> **Note:** `--privileged` is necessary because the build process uses loop mount

> **Note:** `$OUTPUT_DIR` is the path where the resulting images will be placed on the local file system
