## `buildpack-deps:cosmic-scm`

```console
$ docker pull buildpack-deps@sha256:5fd148b3013f4d040b2b2238b35721c3b37862644b1bc2f85675bb1eb0fd6342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:cosmic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1f779c7995f33b211cf98eca86f19d998acf04e2ecf04a4b8520f2ce186676a0
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91145314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb95f58644c08c53af1c68a5e6e47ac53469e7fba5dc1338a3c60bed92fc833`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:10 GMT
ADD file:ece2c9fa61cd3461f10cd8ec579bca502b3627fda44cbef3384397d9ee954dc1 in / 
# Tue, 05 Jun 2018 21:21:11 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:12 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:12 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:13 GMT
CMD ["/bin/bash"]
# Wed, 11 Jul 2018 00:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jul 2018 00:20:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jul 2018 00:22:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c0ca458ff045375fcdf9c3b2a3a21a6ab9296ef210aec29ad5be2db9bcdd670`  
		Last Modified: Tue, 05 Jun 2018 20:24:33 GMT  
		Size: 31.4 MB (31406074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de52c1a5aa543db4621dff125262d0794871f0cad9da0c6343f423185cf5f9`  
		Last Modified: Tue, 05 Jun 2018 21:23:30 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e1b2c9c16291d919092aafc17911b0543113a8fc23019296c55225b03185b7`  
		Last Modified: Tue, 05 Jun 2018 21:23:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab8dbe84d4909f2962932055ae971ba8c09de36e170009b27b99d757e2a688f`  
		Last Modified: Tue, 05 Jun 2018 21:23:31 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42d57ca5baa5ac106fc2f9dbbcdfccc58e36156336b775326d69aabfa4c0d5d`  
		Last Modified: Tue, 05 Jun 2018 21:23:30 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6edcee0f108af2b7fcb3ecda08a7b89f5bee178ab5d51a5df2c310eaacfdebb`  
		Last Modified: Wed, 11 Jul 2018 00:27:26 GMT  
		Size: 5.8 MB (5833437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfaf6c2931b17298faa06154a92f73a627d865751dc69dfc1e8851203d1e8c76`  
		Last Modified: Wed, 11 Jul 2018 00:27:24 GMT  
		Size: 3.2 MB (3195192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de77a5237f1716cb45e2eb729461a20c60c90a3e37c0e0588de7e12310e1db9`  
		Last Modified: Wed, 11 Jul 2018 00:28:17 GMT  
		Size: 50.7 MB (50708339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:cosmic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:78facdc9ba6df53a747d4c235ffacd5bd730618a5b18992b002ad01cd68a6adc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb76f4aa7f2f03f9379ba47ef984a1e4419236cdab2e59e4911a66d28f5efb97`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 06 Jun 2018 12:16:48 GMT
ADD file:261729513d1d4e0b8cfcf264cf094d330a9d8c103898e4a75b7da5516e5d544b in / 
# Wed, 06 Jun 2018 12:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 06 Jun 2018 12:17:10 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 12:17:11 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Wed, 06 Jun 2018 12:17:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 06 Jun 2018 12:17:12 GMT
CMD ["/bin/bash"]
# Wed, 11 Jul 2018 11:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jul 2018 11:58:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jul 2018 11:59:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:458499029c42367caba539c50c2e191936e4aad131a0c2ec80fc3e379ff43adb`  
		Last Modified: Wed, 06 Jun 2018 12:23:33 GMT  
		Size: 26.8 MB (26823415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951edb51922100fc354dfcc8ebb157d1b003c38ebdc7e2c4d85aad41865388ff`  
		Last Modified: Wed, 06 Jun 2018 12:23:26 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663f49360f77c6aeaf89cb6ec06854ba7854a5175ac05d678356431587c47db6`  
		Last Modified: Wed, 06 Jun 2018 12:23:26 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390108522fbcea5fc481a3e1583a3a5db3e4e632300abfa7226d1acc2c6c5e36`  
		Last Modified: Wed, 06 Jun 2018 12:23:26 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8768044cde9e389bc1efe15394485afb5db85f46d94ecb72d42fcc0463dca0a0`  
		Last Modified: Wed, 06 Jun 2018 12:23:26 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cc2a548aa559a954ddcf1401002cda9dea9cf96de26165f4981abe9e2cc7d2`  
		Last Modified: Wed, 11 Jul 2018 12:01:24 GMT  
		Size: 4.9 MB (4930460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64ec542c1b8cae571a786f0b09ac4d7e4033db9f7d67a20e928e7a1ea9c14ab`  
		Last Modified: Wed, 11 Jul 2018 12:01:24 GMT  
		Size: 2.7 MB (2718416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b74ffa7aaf2cc43cea319b0b24d7d1ca137fe33627c8d02fc7c54137581185`  
		Last Modified: Wed, 11 Jul 2018 12:02:02 GMT  
		Size: 45.6 MB (45558192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:cosmic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:138932ac5211c8ab15fb21260403bc2e0a1c096669c5b97f2415795d5b9e0ec1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.9 MB (84940117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68a477a27eb73b5af863ce25f747fd543bd2fd3a0f4a29545f1aae1ab1cccbaf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 06 Jun 2018 09:36:48 GMT
ADD file:5c5ae9859989b2106dc10823f3419d642755619e7eaa244c84c89a9678779971 in / 
# Wed, 06 Jun 2018 09:36:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 06 Jun 2018 09:36:52 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 09:36:55 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Wed, 06 Jun 2018 09:36:57 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 06 Jun 2018 09:36:58 GMT
CMD ["/bin/bash"]
# Wed, 11 Jul 2018 08:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jul 2018 08:41:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jul 2018 08:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1f48f4e125f7a97a6953ad4b266081f5e4c5acaf8d7fdc63a98e9a5f32384345`  
		Last Modified: Wed, 06 Jun 2018 09:41:15 GMT  
		Size: 28.3 MB (28300974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97ca4873890ac0a34725a3b48a2137e0fbc87756dae93365230db43342894e7`  
		Last Modified: Wed, 06 Jun 2018 09:41:05 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f8636160dd4576a5d2dd4b6806266cb97ff23597890ff00aba9f68aea406ee`  
		Last Modified: Wed, 06 Jun 2018 09:41:05 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143e26b0e6b3fe2008653142140e945e0225ea879acf1dde8459a84885d8c4ee`  
		Last Modified: Wed, 06 Jun 2018 09:41:05 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce0a40644cd0b897fc84184da0aa559416260983c291245750e8149bc08b67`  
		Last Modified: Wed, 06 Jun 2018 09:41:05 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28334ac0fa36aed07617176b1c919e8be7ebe6994de779220c6f9ed3cecad15`  
		Last Modified: Wed, 11 Jul 2018 08:54:11 GMT  
		Size: 5.3 MB (5298529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44da7f4bbf602f690b0c50b365d86ffc34c44c9ba6e4eb79cf63df0c72d8e2f`  
		Last Modified: Wed, 11 Jul 2018 08:54:10 GMT  
		Size: 2.9 MB (2936084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb581b79a37bc49a9309306d53ebf1a40dc1de6731b8033ac52e7e2914d19325`  
		Last Modified: Wed, 11 Jul 2018 08:55:10 GMT  
		Size: 48.4 MB (48402267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:cosmic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:34da897caac1c35f0863340c97cca9a4dbc3d3ace3ce7d3cb0a105c16305a48c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93779238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cb735f9981c8329fdd5038a1d3006d825562b65942f69bacb177325e83ebc68`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 06 Jun 2018 10:48:40 GMT
ADD file:50a73ee4973a0de02efa27ab556d8a092cc44562d04a1eccd459fba51bfe7b95 in / 
# Wed, 06 Jun 2018 10:48:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 06 Jun 2018 10:48:41 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 10:48:42 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Wed, 06 Jun 2018 10:48:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 06 Jun 2018 10:48:43 GMT
CMD ["/bin/bash"]
# Wed, 11 Jul 2018 10:39:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jul 2018 10:40:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jul 2018 10:42:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd2ca3cccfd99e68b8939d6848cb95fb6d76bbc3a218603e7bedd335386dcdf7`  
		Last Modified: Wed, 06 Jun 2018 10:51:30 GMT  
		Size: 31.8 MB (31837603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57957f423a7bcb2237b63ac6476e9e6f9103171d044fa6563ff883b76586381`  
		Last Modified: Wed, 06 Jun 2018 10:51:16 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b7a51423896486c245c91fba15bd1f503ebcd502a567f6b15750c55b29cc0d`  
		Last Modified: Wed, 06 Jun 2018 10:51:15 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4b55a21427ac12ee7f83d5e4f974453ee75838f96ee8ac3059d49c6c71eb35`  
		Last Modified: Wed, 06 Jun 2018 10:51:15 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9699b87fe9830e1c766cc00c1d08d0705128dbb3f0854770e8f307e307ebb3ea`  
		Last Modified: Wed, 06 Jun 2018 10:51:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c6031964dedae44e8da235def6e2a61da10e377938213bae5593886eba537b`  
		Last Modified: Wed, 11 Jul 2018 10:47:03 GMT  
		Size: 6.1 MB (6110435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4a695d7b6aebf633396918e9bd93a8a724f017b76c68aac5a3a74b1c956632`  
		Last Modified: Wed, 11 Jul 2018 10:47:01 GMT  
		Size: 3.5 MB (3453150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2a75f18093d3facf5f3aa7c5f4bc1779a3bd4fa27d28ca9baa3d36bdc0587e`  
		Last Modified: Wed, 11 Jul 2018 10:48:16 GMT  
		Size: 52.4 MB (52375783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:cosmic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3a1791a452f9692d4aa2441401d1a266063234be55c883fb1d0ac0acb33d95d2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104242459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf28cff40b361c76f47c4311e3c09648d5d8e4fa39e640ec7487bc240aa0b01`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 06 Jun 2018 09:04:09 GMT
ADD file:138ddc37989046fde5333917d43eeb91832677d0aa7e1b0da5429cb2535cbd0f in / 
# Wed, 06 Jun 2018 09:04:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 06 Jun 2018 09:04:50 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 09:05:16 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Wed, 06 Jun 2018 09:05:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 06 Jun 2018 09:05:49 GMT
CMD ["/bin/bash"]
# Wed, 11 Jul 2018 08:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jul 2018 08:25:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jul 2018 08:27:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1b6dc1b5f6bee1a19ad52f65522b00db78e8803876125fe69660a3358d965554`  
		Last Modified: Wed, 06 Jun 2018 09:09:21 GMT  
		Size: 35.1 MB (35111382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e30a53e6751fd7c669aa90c5fd40012c2624c06800772602203f5a4958f01b`  
		Last Modified: Wed, 06 Jun 2018 09:09:11 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d08951a6f22d8a76e6e679c022faa5dd73cc11a9edbf30ec942f1cbf0a8709`  
		Last Modified: Wed, 06 Jun 2018 09:09:11 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616df9d91dc7edc318a8446af565aa6a5863b7bca4821a1f6aa46d2f72fd021b`  
		Last Modified: Wed, 06 Jun 2018 09:09:11 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2bedc19d562cb9f9e3cac1b3226551fdf2307f737bc971422fb8e069062e11`  
		Last Modified: Wed, 06 Jun 2018 09:09:11 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c2f07a21f627164d59bfb8ca1393933af425d6dc4bcc6b7c8472b5a62215b9`  
		Last Modified: Wed, 11 Jul 2018 08:42:16 GMT  
		Size: 6.1 MB (6051652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9196d6c478d19f2fe85c8b0757ea60fa89fb0231562b7ebc3a4e1a566cc4dc4`  
		Last Modified: Wed, 11 Jul 2018 08:42:15 GMT  
		Size: 4.0 MB (3971876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbe130f3ed7a22afe007ca6b1c9cd62eca048131de0d5f728fbd8f2d177e32b`  
		Last Modified: Wed, 11 Jul 2018 08:43:02 GMT  
		Size: 59.1 MB (59105257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:cosmic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fd85258262c9348935323f9c2baaebe5eaea15f6bb90321a8945b11d8c8aa997
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88868136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:196cdbada3f035dd22e8b897510c1c8d7c4a228aef7ffe987b0264fda779bb0e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 06 Jun 2018 12:07:12 GMT
ADD file:086f1f65d3c68b3a21e090d1ab0eac2c12ae8977fdcf6229432366789e933df5 in / 
# Wed, 06 Jun 2018 12:07:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 06 Jun 2018 12:07:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 12:07:14 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Wed, 06 Jun 2018 12:07:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 06 Jun 2018 12:07:15 GMT
CMD ["/bin/bash"]
# Wed, 11 Jul 2018 11:41:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jul 2018 11:42:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jul 2018 11:42:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af51a2b27d132be0acffe9578890f5b427cefa535e1f31eb10c1fa46e31fe694`  
		Last Modified: Wed, 06 Jun 2018 12:09:13 GMT  
		Size: 30.0 MB (29983732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9c958ca09c91a5fe01ee1ffe4157b1ac68d25552185ea02fdc698430a2d746`  
		Last Modified: Wed, 06 Jun 2018 12:09:07 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd4bad1a62deea9d560eb0ab7a0f1c2807c66f1b6ef8af13160d63800b9f7b8`  
		Last Modified: Wed, 06 Jun 2018 12:09:07 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e952b03cebd8f29d98759fcda4a188181d20f6d238ea7ecb47047c32dadc75`  
		Last Modified: Wed, 06 Jun 2018 12:09:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684a30e9baefa1dbf0dfb09f80ecdb1bcd36dfc71e526b4effe6943178be99e1`  
		Last Modified: Wed, 06 Jun 2018 12:09:07 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa4428bebfb05a2554901ba7fae9f0562863beec4450d49054c8f726b277d52`  
		Last Modified: Wed, 11 Jul 2018 11:44:43 GMT  
		Size: 5.5 MB (5519510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d684ae94d9107b14fdf879eff147e568e69ae7124d3c8fa2be540198837e99`  
		Last Modified: Wed, 11 Jul 2018 11:44:42 GMT  
		Size: 3.1 MB (3142021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db94858196472dd8fe29e29af6106695e897b76836d46ad600e44e44b641fa17`  
		Last Modified: Wed, 11 Jul 2018 11:45:16 GMT  
		Size: 50.2 MB (50220611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip