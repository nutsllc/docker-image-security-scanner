# Docker Image Security Scanner

Docker Image Security scanner is a wrapper script of the [Clair](https://github.com/coreos/clair) which has been developed by CoreOS as open source project.

You would be able to scan vulnerability data in local docker container.

## What is Clair

>Vulnerability data is continuously imported from a known set of sources and correlated with the indexed contents of container images in order to produce lists of vulnerabilities that threaten a container. When vulnerability data changes upstream, the previous state and new state of the vulnerability along with the images they affect can be sent via webhook to a configured endpoint. All major components can be customized programmatically at compile-time without forking the project.

* [more detail](https://github.com/coreos/clair/blob/master/README.md)

## Usage

Just type three commands below to scan your local docker image. That's all.

```bash
$ git clone https://github.com/nutsllc/docker-image-checker.git
$ cd docker-image-checker
$ sh scanner <Docker Image ID>
```

When you exexute ``sh checker <Docker Image ID>``, what all you need components will be automatically seted-up and be running.

So, only you need to do is ``clone`` repo. and ``sh scanner <Docker Image ID>`` for scaning target docker image by Clair 

### Find docker image id

```bash
$ docker images
```

## License

* Clair - The Apache 2.0 Licence
* PostgreSQL - The PostgreSQL License
