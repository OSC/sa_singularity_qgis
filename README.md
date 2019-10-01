# Singularity QGIS

[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/3587)
[![GitHub License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)

Singularity image for [QGIS](https://qgis.org/en/site/index.html). It was built on top of the base Docker image [ubuntu](https://hub.docker.com/_/ubuntu). Packages installed: `qgis qgis-plugin-grass`

## Build

You can build a local Singularity image named `qgis.sif` with:

```sh
sudo singularity build qgis.sif Singularity
```

## Deploy

Instead of building it yourself you can download the pre-built image from [Singularity Hub](https://www.singularity-hub.org) with:

```sh
singularity pull qgis.sif shub://OSC/sa_singularity_qgis
```

## Run

### Start QGIS
QGIS is started using the default run command:
```sh
singularity run qgis.sif
```
or as a native command
```sh
./qgis.sif
```


## License

The code is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
