# Eclipse SmartHome Packaging Sample

This repo contains a sample of how to create a small working runtime package that uses the Eclipse SmartHome framework.
You can use this example to build an own minimal distribution running in the Karaf Container.

More information about Karaf: http://karaf.apache.org/

## Prerequisites

* Maven

## Checkout

Checkout the source code from GitHub, e.g. by running:

```
git clone https://github.com/maggu2810/smarthome-packaging-sample-karaf.git
```

## Build the distribution

```sh
mvn clean install
```

The maven build will create a tar.gz that contains the full distribution in the target directory.

In the `target/assembly` folder contains the content of this archive.
So you can start it directly using e.g. `target/assembly/bin/karaf`

## Start runtime

Extract the distribution archive and chdir into or use the already unpacked runtime in the target/assembly directory:

```sh
bin/karaf
```

## Using the UI

The distribution already includes the PaperUI.
  [http://your-host:8181/ui/index.html](http://your-host:8181/ui/index.html)

Also included is the Apache Karaf Web Console. The Apache Karaf Web Console is a simple tool to inspect and manage OSGi framework and the Karaf Container itself.
  [http://your-host:8181/system/console/](http://your-host:8181/system/console/)

```text
username: karaf
password: karaf
```

