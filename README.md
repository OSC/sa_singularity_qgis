# Singularity OpenEXR

[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/3584)[![GitHub License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)

Singularity image for [OpenEXR](https://www.openexr.com/). It was built on top of the base Docker image [ubuntu](https://hub.docker.com/_/ubuntu)

## Build

You can build a local Singularity image named `openexr.sif` with:

```sh
sudo singularity build openexr.sif Singularity
```

## Deploy

Instead of building it yourself you can download the pre-built image from [Singularity Hub](https://www.singularity-hub.org) with:

```sh
singularity pull --name openexr.sif shub://OSC/sa_singularity_openexr
```

## Run

### Render .EXR image

The `exrdisplay` command is launched using the command:

```sh
singularity exec openexr.sif exrdisplay -h
```

Example:

```console
$ singularity exec openexr.sif exrdisplay rendertest_0001.exr
```

## License

The code is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
