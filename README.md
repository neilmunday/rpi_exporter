# rpi_exporter

A Prometheus metrics exporter for the Raspberry Pi.

Exports CPU and GPU temperatures using Prometheus Python module.

It can be run like so:

```
./rpi_exporter [ -p PORT ]
```

The default port is `9111` unless specified on the command line.

An Arch Linux PKGBUILD file is also included if you want to package it for Arch Linux, e.g.:

```
git clone https://github.com/neilmunday/rpi_exporter
cd rpi_exporter
makepkg -si
```
