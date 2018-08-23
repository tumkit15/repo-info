## `mongo:unstable-bionic`

```console
$ docker pull mongo@sha256:1b64fb84d1a07e944fbf4030e37cf7bfd0d8fbe1131f582831b541912c59b019
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:unstable-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:57da9feb1fe063bad72643f1872c765616178b2b354dd0beee2dae316dd2046f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125229991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2676c27f693513b846fa073c1e6c04fbf90820c3745462c33c666ccf3cf491c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 22 Aug 2018 17:28:39 GMT
ADD file:3df374a69ce696c21058366678c1ceb89e11349e52decfd35de0ee3bd8dc1162 in / 
# Wed, 22 Aug 2018 17:28:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 22 Aug 2018 17:28:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 22 Aug 2018 17:28:56 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Wed, 22 Aug 2018 17:28:57 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 22 Aug 2018 17:28:57 GMT
CMD ["/bin/bash"]
# Wed, 22 Aug 2018 22:54:13 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 22 Aug 2018 22:55:00 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		gnupg dirmngr 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Aug 2018 22:55:00 GMT
ENV GOSU_VERSION=1.10
# Wed, 22 Aug 2018 22:55:01 GMT
ENV JSYAML_VERSION=3.10.0
# Wed, 22 Aug 2018 22:55:14 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Wed, 22 Aug 2018 22:55:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 22 Aug 2018 22:56:30 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 22 Aug 2018 22:56:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	gpgconf --kill all; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 22 Aug 2018 22:56:32 GMT
ARG MONGO_PACKAGE=mongodb-org-unstable
# Wed, 22 Aug 2018 22:56:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 22 Aug 2018 22:56:32 GMT
ENV MONGO_PACKAGE=mongodb-org-unstable MONGO_REPO=repo.mongodb.org
# Wed, 22 Aug 2018 22:56:33 GMT
ENV MONGO_MAJOR=4.1
# Wed, 22 Aug 2018 22:56:33 GMT
ENV MONGO_VERSION=4.1.2
# Wed, 22 Aug 2018 22:56:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 22 Aug 2018 22:56:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 22 Aug 2018 22:57:00 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 22 Aug 2018 22:57:00 GMT
VOLUME [/data/db /data/configdb]
# Wed, 22 Aug 2018 22:57:01 GMT
COPY file:432f09fb61dea3ba52524ce5b165c30e7e96b5b711f3dc56c2c47cf8a79211d3 in /usr/local/bin/ 
# Wed, 22 Aug 2018 22:57:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Aug 2018 22:57:01 GMT
EXPOSE 27017/tcp
# Wed, 22 Aug 2018 22:57:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:124c757242f88002a858c23fc79f8262f9587fa30fd92507e586ad074afb42b6`  
		Last Modified: Wed, 22 Aug 2018 17:32:16 GMT  
		Size: 31.8 MB (31757372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebc019eb4e2bbd192e61bce91038048924216d72dfe6ac3255322caaeb70144`  
		Last Modified: Wed, 22 Aug 2018 17:32:06 GMT  
		Size: 837.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0825f7ffbea2ddf119026b0d6c4c453dfa38edb5c2abbe59bdba6ffdb3b9f`  
		Last Modified: Wed, 22 Aug 2018 17:32:06 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b0bb65d1bfb978cd646dcd653164f74b7e8656aa1b3a87657b8d244b56d324`  
		Last Modified: Wed, 22 Aug 2018 17:32:06 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3b655c7f887451d42e45a04c2d13478171e4d451419bc8cf76c635f509532f`  
		Last Modified: Wed, 22 Aug 2018 17:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7390dfec61b2668dd019074a86e41f3d8fbdd269329e8060e09c915bbf1b9841`  
		Last Modified: Wed, 22 Aug 2018 23:00:54 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d69d17b8aec7c7b82eb9e4835a46e50f0d5fc2ce28553acdd77f1abc876b25`  
		Last Modified: Wed, 22 Aug 2018 23:00:57 GMT  
		Size: 7.3 MB (7337391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1361c44993d16f9581ea06e61f361c2cafa8147a5e5a6cf1733080118f1951`  
		Last Modified: Wed, 22 Aug 2018 23:00:55 GMT  
		Size: 773.1 KB (773124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4803d25be6fa9ebd428665289ba3a24a09c7c346fa58164471ac63429f31aa5f`  
		Last Modified: Wed, 22 Aug 2018 23:00:54 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f350f2596b0b637f1533cd1160d66ef297bef2bb11418bf6bc02df35edc9733`  
		Last Modified: Wed, 22 Aug 2018 23:03:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a08784ed7496871da368491300e4ecc49b9c62a275ca0184f6f7eff73638f8`  
		Last Modified: Wed, 22 Aug 2018 23:03:07 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1e10c7f9d86a2783f7bc77503a0368a7300c4a6b30536448b1ff1d388b625c`  
		Last Modified: Wed, 22 Aug 2018 23:03:28 GMT  
		Size: 85.4 MB (85352276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a13a4867be883abed132024ca5cc4defd396a6d4b2e126c019ef79d14e6662c`  
		Last Modified: Wed, 22 Aug 2018 23:03:07 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4f2e03fe951cd7ea977c1c6e767a907da88ab96257150549b26d8aec65d83c`  
		Last Modified: Wed, 22 Aug 2018 23:03:07 GMT  
		Size: 3.7 KB (3708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip