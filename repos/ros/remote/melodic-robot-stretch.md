## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:17a0847a9b5ce7a42be5402573c9fdaf0110b900e044f1f00ae9bc3881f028b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:38117f96d6af8e99349af8fe8fbcb9dee526da958b440d3446173be62873922a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **553.0 MB (553002199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80818d63ed894e7b9db0f605691f2256d6badaa1edf201bdcc978aab15ba7d5e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Sep 2018 21:21:24 GMT
ADD file:58d5c21fcabcf1eec94e8676a3b1e51c5fdc2db5c7b866a761f907fa30ede4d8 in / 
# Tue, 04 Sep 2018 21:21:24 GMT
CMD ["bash"]
# Wed, 05 Sep 2018 07:22:37 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 07:22:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 05 Sep 2018 07:22:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu `lsb_release -sc` main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 05 Sep 2018 07:23:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 07:23:16 GMT
ENV LANG=C.UTF-8
# Wed, 05 Sep 2018 07:23:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Sep 2018 07:23:29 GMT
RUN rosdep init     && rosdep update
# Wed, 05 Sep 2018 07:43:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Sep 2018 07:45:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 07:45:32 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Wed, 05 Sep 2018 07:45:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Sep 2018 07:45:33 GMT
CMD ["bash"]
# Wed, 05 Sep 2018 07:46:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 07:47:20 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05d1a5232b461a4b35424129580054caa878cd56f100e34282510bd4b4082e4d`  
		Last Modified: Tue, 04 Sep 2018 21:25:27 GMT  
		Size: 45.3 MB (45310060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d35d34ad2c05d7e708e20b396a12d694b5e2dceeda1ddda67bfaefeaec8581`  
		Last Modified: Wed, 05 Sep 2018 08:02:07 GMT  
		Size: 21.1 MB (21067826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0408d25913963c576e46702fe9023e80e080e9c27b1c1d1fab77729c5c1c12f3`  
		Last Modified: Wed, 05 Sep 2018 08:01:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffee8a2335bce7bd1008574802d3675d5f1e3eff4b359b4179ba7f8bbf69efdf`  
		Last Modified: Wed, 05 Sep 2018 08:01:57 GMT  
		Size: 5.0 KB (4969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaee5e7cb601a6d1b39d0b015aa32b24ffd64b96df60c68aa2a255d0d102fad`  
		Last Modified: Wed, 05 Sep 2018 08:02:20 GMT  
		Size: 53.5 MB (53504558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab149d2c39ddc435ef0ac48243f46eddda94657a0acc6ce125df28d7429c0dd9`  
		Last Modified: Wed, 05 Sep 2018 08:01:58 GMT  
		Size: 809.8 KB (809758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a0f8a5d2ea24d8809d8166d09ce55cdd868d396acebb7726ba091c483e3267`  
		Last Modified: Wed, 05 Sep 2018 08:11:03 GMT  
		Size: 268.5 MB (268529695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad8be9c57c9af46660e4285acf2658b38133d7debbff2cd53439dc7a199726`  
		Last Modified: Wed, 05 Sep 2018 08:10:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5332e05f7c7e2f3e16f83440f160205b843a8207742fe782ce7f2813e2499d3`  
		Last Modified: Wed, 05 Sep 2018 08:11:32 GMT  
		Size: 108.5 MB (108462047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae66a479b0088da6923d38d1977f925610827f0fe86b895b1cb3f19bafca3609`  
		Last Modified: Wed, 05 Sep 2018 08:11:54 GMT  
		Size: 55.3 MB (55311714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e87964d5c9f7947b60a27ecd0474cc0a57dbcbed28f0ceee0c9b80d052b75fc6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **493.4 MB (493359730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3588bf4d0ce71800e94ca26d4485ca9fd938c7b99101dd44cf4e17316a16b56`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Sep 2018 08:50:16 GMT
ADD file:4e01bc399974f6fe22cd2b4421c2e52c52380aa00a770986939071dbc59d734e in / 
# Wed, 05 Sep 2018 08:50:30 GMT
CMD ["bash"]
# Wed, 05 Sep 2018 19:12:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 19:12:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 05 Sep 2018 19:12:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu `lsb_release -sc` main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 05 Sep 2018 19:14:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 19:14:19 GMT
ENV LANG=C.UTF-8
# Wed, 05 Sep 2018 19:14:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Sep 2018 19:15:07 GMT
RUN rosdep init     && rosdep update
# Wed, 05 Sep 2018 19:51:04 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Sep 2018 20:00:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 20:01:09 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Wed, 05 Sep 2018 20:01:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Sep 2018 20:01:11 GMT
CMD ["bash"]
# Wed, 05 Sep 2018 20:04:23 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 20:10:30 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:421608e4e92275f9265604523f9299cf5f4bd493a1ea3affd62c265b38fc8823`  
		Last Modified: Wed, 05 Sep 2018 09:06:53 GMT  
		Size: 43.1 MB (43123621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2b999e6626b77886e3c38e8a785a7e1a7e36e0039445255654d5bc5ad24d76`  
		Last Modified: Wed, 05 Sep 2018 20:30:40 GMT  
		Size: 19.7 MB (19730993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac738c1923ba135a921c240522fdce8b7030d13698f3f0904005bbea14ee354`  
		Last Modified: Wed, 05 Sep 2018 20:29:12 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f424c24b55fa5004b2452d07e0a983ea358de7216774776775ad9a9c919767d7`  
		Last Modified: Wed, 05 Sep 2018 20:29:09 GMT  
		Size: 5.0 KB (4974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ce9c4049ae683de69beffcf613062f883f5de22797cf56c118afff6a7e4e5a`  
		Last Modified: Wed, 05 Sep 2018 20:31:42 GMT  
		Size: 51.5 MB (51465804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e1ffb408b178aa6dcc279a4dd049a621c4035340001992130302a183cece83`  
		Last Modified: Wed, 05 Sep 2018 20:29:12 GMT  
		Size: 811.0 KB (810967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e095f4ebfc58fbc0e9ca060686e26159e7083364a2415e5cc4e17422fb6b83`  
		Last Modified: Wed, 05 Sep 2018 20:41:33 GMT  
		Size: 222.7 MB (222710108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d983a971d341024ea176f029f0af9393f7e958ffb1637a7b2d17263017492cb2`  
		Last Modified: Wed, 05 Sep 2018 20:39:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513127a77e4b6379353506a75e47109ee28775891e912de72bffbc7beb16231`  
		Last Modified: Wed, 05 Sep 2018 20:42:38 GMT  
		Size: 102.9 MB (102934966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2203af899fb3155f70a9e1a67b7edd37f1881ea2a4a665b157e700ba18d444a0`  
		Last Modified: Wed, 05 Sep 2018 20:43:28 GMT  
		Size: 52.6 MB (52576726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
