## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:ecfc4bbc3baef7f054bd96e50194a25b0452a18010a2ba2008dc58404dacd4da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d1a8db20694b268db1043be3debe539444cdbef21299f0778f522c909fd0011c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28680299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e72aaf02ca523bc84d6822405dd5c639fda76bc219afa82836c8bcf09b22e31f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 11 Sep 2018 22:19:27 GMT
ADD file:ad486f580145bd2de2441f0846f0bfa62cd1f6d5cb374c28d29ef1ca785a0bbc in / 
# Tue, 11 Sep 2018 22:19:28 GMT
CMD ["/bin/sh"]
# Tue, 11 Sep 2018 22:45:27 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 11 Sep 2018 23:34:40 GMT
RUN apk add --no-cache tzdata bash
# Mon, 17 Sep 2018 20:23:52 GMT
ENV INFLUXDB_VERSION=1.6.3
# Mon, 17 Sep 2018 20:24:03 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar ca-certificates &&     update-ca-certificates &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 17 Sep 2018 20:24:03 GMT
COPY file:3ee2bc0321c2aa2451df7a508649c3a54f0eebc1ef9b8a24967c58105b4d3160 in /etc/influxdb/influxdb.conf 
# Mon, 17 Sep 2018 20:24:03 GMT
EXPOSE 8086/tcp
# Mon, 17 Sep 2018 20:24:04 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Sep 2018 20:24:04 GMT
COPY file:098affa3d1b749dacb263ddacfd86a5de1f598d6ba1f7c789ce482c66ee9c80b in /entrypoint.sh 
# Mon, 17 Sep 2018 20:24:04 GMT
COPY file:44e0050f3b04248a6900eace944c581b13b4ad9af1e5cfb91d837cb5e24356e6 in /init-influxdb.sh 
# Mon, 17 Sep 2018 20:24:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Sep 2018 20:24:05 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:3489d1c4660eacaadef3acfc3512c785acde2333b5e6e9387f43490a766382bf`  
		Last Modified: Tue, 11 Sep 2018 22:21:09 GMT  
		Size: 2.0 MB (2016693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad45804dc73d879f10b8bee29ee78a7554f30eda7a7a23fa9b5a98c6b7431397`  
		Last Modified: Tue, 11 Sep 2018 22:46:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ead0e4c75aae70ed9b7c002be7dd587da637e1a462bd7a5b7aff856884d2f6`  
		Last Modified: Tue, 11 Sep 2018 23:36:37 GMT  
		Size: 1.5 MB (1513052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c99d75756f20aa8188509bb03b615daa4ac39747935bfeacdbcf91aef8ecce1`  
		Last Modified: Mon, 17 Sep 2018 20:25:54 GMT  
		Size: 25.1 MB (25148804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533bcecd02135ee137d4e9a2a8079b0ba05b65cb6806ab094a935ca5d263e5aa`  
		Last Modified: Mon, 17 Sep 2018 20:25:48 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05ecfed1588bb3bcf0519524c704fe11af13eb7ec28a238fb95226ddb642409`  
		Last Modified: Mon, 17 Sep 2018 20:25:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c091c1cfe8e288c1fa4f058bb6305c9f593b7ae2e0360bca3dd558c4b4371491`  
		Last Modified: Mon, 17 Sep 2018 20:25:48 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
