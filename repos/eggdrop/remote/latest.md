## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:1c5d2dd27b22ae1b06be91634c9468ed6383ad693d5a1b4559104abe1c04f2b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:0ea10c904adb22dc71f632d40309714cd0ad5e3d9174bf58fbab6408f1b5e898
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9553833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94e5180bdae50b62e7848650deafec75a8a10371dd2f9df6ec7f93f06d89983f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 11 Sep 2018 22:19:38 GMT
ADD file:49f9e47e678d868d5b023482aa8dded71276a241a665c4f8b55ca77269321b34 in / 
# Tue, 11 Sep 2018 22:19:39 GMT
CMD ["/bin/sh"]
# Tue, 11 Sep 2018 22:53:24 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 11 Sep 2018 22:53:25 GMT
RUN adduser -S eggdrop
# Tue, 11 Sep 2018 22:53:26 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 11 Sep 2018 22:55:01 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 11 Sep 2018 22:55:54 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.3.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.3.tar.gz.asc eggdrop-1.8.3.tar.gz   && rm eggdrop-1.8.3.tar.gz.asc   && tar -zxvf eggdrop-1.8.3.tar.gz   && rm eggdrop-1.8.3.tar.gz   && ( cd eggdrop-1.8.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 11 Sep 2018 22:55:55 GMT
ENV NICK=
# Tue, 11 Sep 2018 22:55:55 GMT
ENV SERVER=
# Tue, 11 Sep 2018 22:55:55 GMT
ENV LISTEN=3333
# Tue, 11 Sep 2018 22:55:55 GMT
ENV OWNER=
# Tue, 11 Sep 2018 22:55:55 GMT
ENV USERFILE=eggdrop.user
# Tue, 11 Sep 2018 22:55:56 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 11 Sep 2018 22:55:56 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 11 Sep 2018 22:55:56 GMT
EXPOSE 3333/tcp
# Tue, 11 Sep 2018 22:55:56 GMT
COPY file:d80744926cf822928c4fc2c3f9107364df320eecb3ae407a3a5419a43ae4b872 in /home/eggdrop/eggdrop 
# Tue, 11 Sep 2018 22:55:57 GMT
COPY file:919804e5ddd4c807c178caccfed03e9d75a459fe0f744c3a1ada109817cb44ec in /home/eggdrop/eggdrop/scripts/ 
# Tue, 11 Sep 2018 22:55:57 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 11 Sep 2018 22:55:57 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c67f3896b22c1378881cbbb9c9d1edfe881fd07f713371835ef46d93c649684d`  
		Last Modified: Tue, 11 Sep 2018 22:21:16 GMT  
		Size: 2.1 MB (2107175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926d70e02e336bd99f571b4dcb3559e271e8828692d98358bbe5356307e1a53e`  
		Last Modified: Tue, 11 Sep 2018 22:56:19 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce023cda4d8be9e674bd3470ea36deef2f550e397afa48daac7dba6486e38b49`  
		Last Modified: Tue, 11 Sep 2018 22:56:18 GMT  
		Size: 8.8 KB (8847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd304d072d64b77eece79d4e6ba5ee0025dbc4245ca82404ec242e5eed853df`  
		Last Modified: Tue, 11 Sep 2018 22:56:32 GMT  
		Size: 4.4 MB (4402002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a94b92e95299e2f347f97e27204f3430fa6148ae240f4c4eb0eba9a026d22`  
		Last Modified: Tue, 11 Sep 2018 22:56:32 GMT  
		Size: 3.0 MB (3031976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed04c83e8f88ba701cf88a5770c843abb5706303b7b4b82f3580e4bbd4f0cb76`  
		Last Modified: Tue, 11 Sep 2018 22:56:31 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0acbaf2291b10bbf28072e4e325676b061dcae94a85b81f19270994dc39699`  
		Last Modified: Tue, 11 Sep 2018 22:56:31 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
