## `redis:3-alpine`

```console
$ docker pull redis@sha256:e9083e10f5f81d350a3f687d582aefd06e114890b03e7f08a447fa1a1f66d967
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redis:3-alpine` - linux; amd64

```console
$ docker pull redis@sha256:359cfebb00bef01cda3bc1ca453e6455c770a246a06ad8df499a28118c144eda
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9417946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e94a98d3442e94970dde0013cae68240f025b63f0109cff422acf26d272d13b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 11 Sep 2018 22:19:50 GMT
ADD file:25c10b1d1b41d46a1827ad0b0d2389c24df6d31430005ff4e9a2d84ea23ebd42 in / 
# Tue, 11 Sep 2018 22:19:50 GMT
CMD ["/bin/sh"]
# Wed, 12 Sep 2018 03:26:27 GMT
RUN addgroup -S redis && adduser -S -G redis redis
# Wed, 12 Sep 2018 03:26:29 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 12 Sep 2018 03:29:53 GMT
ENV REDIS_VERSION=3.2.12
# Wed, 12 Sep 2018 03:29:53 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-3.2.12.tar.gz
# Wed, 12 Sep 2018 03:29:54 GMT
ENV REDIS_DOWNLOAD_SHA=98c4254ae1be4e452aa7884245471501c9aa657993e0318d88f048093e7f88fd
# Wed, 12 Sep 2018 03:30:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		jemalloc-dev 		linux-headers 		make 		musl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)"; 	make -C /usr/src/redis install; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .redis-rundeps $runDeps; 	apk del .build-deps; 		redis-server --version
# Wed, 12 Sep 2018 03:30:43 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 12 Sep 2018 03:30:43 GMT
VOLUME [/data]
# Wed, 12 Sep 2018 03:30:43 GMT
WORKDIR /data
# Tue, 02 Oct 2018 18:11:38 GMT
COPY file:592b00f2927fa2144858cc8c78ef610815375a7ed6046b2460776997a98d663a in /usr/local/bin/ 
# Tue, 02 Oct 2018 18:11:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Oct 2018 18:11:39 GMT
EXPOSE 6379/tcp
# Tue, 02 Oct 2018 18:11:39 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:4fe2ade4980c2dda4fc95858ebb981489baec8c1e4bd282ab1c3560be8ff9bde`  
		Last Modified: Tue, 11 Sep 2018 22:21:23 GMT  
		Size: 2.2 MB (2206931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb758dc2e0380088f86e84055736737a7147cc918d44dd7b9d6b3d10b8846478`  
		Last Modified: Wed, 12 Sep 2018 03:31:03 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989f7b0c858b7747b3a6dd43de74fe166d16abf090b2df6a51687fdf9ae27b2d`  
		Last Modified: Wed, 12 Sep 2018 03:31:02 GMT  
		Size: 402.1 KB (402130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b4b9f869ad95726b86b723cd8b11fb359f6ff5b0736518dc8dd47447aba9ab`  
		Last Modified: Wed, 12 Sep 2018 03:32:14 GMT  
		Size: 6.8 MB (6807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e06138ef2002928e21146e333e1fd766cb4d88742134b7bd0f8eeb715076d8`  
		Last Modified: Wed, 12 Sep 2018 03:32:12 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecd66db81e7cba225fcc892a9ec9fcd90ca71bea91e9e4bc7ad86d4573b80a`  
		Last Modified: Tue, 02 Oct 2018 18:20:34 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:3-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:cd99f95754854f4c5f0f3016abb9e74ce38cf1a9e7b6efff837f6803669dc1d1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9087360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d10efb8c57ec0bc4847da899471e5846ef9bb423df40e9d3cbf33994680954`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 12 Sep 2018 07:49:40 GMT
ADD file:9c713f2312a88f19529816851673353155f329a4b024d62b03f656b0ce32f2a6 in / 
# Wed, 12 Sep 2018 07:49:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 07:49:40 GMT
CMD ["/bin/sh"]
# Wed, 12 Sep 2018 13:48:17 GMT
RUN addgroup -S redis && adduser -S -G redis redis
# Wed, 12 Sep 2018 13:48:26 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 12 Sep 2018 13:57:17 GMT
ENV REDIS_VERSION=3.2.12
# Wed, 12 Sep 2018 13:57:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-3.2.12.tar.gz
# Wed, 12 Sep 2018 13:57:18 GMT
ENV REDIS_DOWNLOAD_SHA=98c4254ae1be4e452aa7884245471501c9aa657993e0318d88f048093e7f88fd
# Wed, 12 Sep 2018 14:02:24 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		jemalloc-dev 		linux-headers 		make 		musl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)"; 	make -C /usr/src/redis install; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .redis-rundeps $runDeps; 	apk del .build-deps; 		redis-server --version
# Wed, 12 Sep 2018 14:02:28 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 12 Sep 2018 14:02:28 GMT
VOLUME [/data]
# Wed, 12 Sep 2018 14:02:29 GMT
WORKDIR /data
# Wed, 03 Oct 2018 09:06:09 GMT
COPY file:592b00f2927fa2144858cc8c78ef610815375a7ed6046b2460776997a98d663a in /usr/local/bin/ 
# Wed, 03 Oct 2018 09:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Oct 2018 09:06:10 GMT
EXPOSE 6379/tcp
# Wed, 03 Oct 2018 09:06:11 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:905674ea9d9448b14f15ae82e3c34138680bac1ef4fc29088aae8c9639b502fe`  
		Last Modified: Wed, 12 Sep 2018 07:50:09 GMT  
		Size: 2.1 MB (2146453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91fe322e1690c8fb3f2b684fd85335d36a45e509b1568683232aede6d8a5e2b`  
		Last Modified: Wed, 12 Sep 2018 07:50:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0282f47fed57cf0edb74497b0117f3bda5406a7b722499f98cfd1cfe84071abd`  
		Last Modified: Wed, 12 Sep 2018 14:02:59 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f05f53c51b59f1cf2512bc366489d8279414dcfdf4d3a44d2b36b407f0d1179`  
		Last Modified: Wed, 12 Sep 2018 14:03:02 GMT  
		Size: 404.7 KB (404670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7b6b6cb7cd754c5204b987ba25e69799cbfa6133472a266d43f89d2f046829`  
		Last Modified: Wed, 12 Sep 2018 14:05:49 GMT  
		Size: 6.5 MB (6534233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ece8c35142b8abd29ac1e21e985b2e27ff0c0fd639d778ca32d1138c6fa40b5`  
		Last Modified: Wed, 12 Sep 2018 14:05:42 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc2af76283e2aad5a8ea62a0144843a831a410f3200cd68727d3e01a5be5be7`  
		Last Modified: Wed, 03 Oct 2018 09:08:58 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:3-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:e7e71971e9ac79ea76a1ce6f79470ec7762c4dde610c90cc268b1c46702ddf63
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9131715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a674704febf60f60c6e30ecdf0e6a620d575aad6b8a5253e8b1bf3137393c96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 12 Sep 2018 08:42:24 GMT
ADD file:a4b53e2a2e207c5107a76c16d91b99cb1ed4ecb90b363913798e663426137d45 in / 
# Wed, 12 Sep 2018 08:42:24 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 08:42:25 GMT
CMD ["/bin/sh"]
# Sat, 15 Sep 2018 11:24:22 GMT
RUN addgroup -S redis && adduser -S -G redis redis
# Sat, 15 Sep 2018 11:24:26 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 15 Sep 2018 11:29:12 GMT
ENV REDIS_VERSION=3.2.12
# Sat, 15 Sep 2018 11:29:14 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-3.2.12.tar.gz
# Sat, 15 Sep 2018 11:29:15 GMT
ENV REDIS_DOWNLOAD_SHA=98c4254ae1be4e452aa7884245471501c9aa657993e0318d88f048093e7f88fd
# Sat, 15 Sep 2018 11:30:29 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		jemalloc-dev 		linux-headers 		make 		musl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)"; 	make -C /usr/src/redis install; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .redis-rundeps $runDeps; 	apk del .build-deps; 		redis-server --version
# Sat, 15 Sep 2018 11:30:32 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 15 Sep 2018 11:30:33 GMT
VOLUME [/data]
# Sat, 15 Sep 2018 11:30:34 GMT
WORKDIR /data
# Wed, 03 Oct 2018 10:09:27 GMT
COPY file:592b00f2927fa2144858cc8c78ef610815375a7ed6046b2460776997a98d663a in /usr/local/bin/ 
# Wed, 03 Oct 2018 10:09:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Oct 2018 10:09:29 GMT
EXPOSE 6379/tcp
# Wed, 03 Oct 2018 10:09:30 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9941776d74c9129fd585b6f0434ba48bd3a7112d6736bc02e6d12f41153cab26`  
		Last Modified: Wed, 12 Sep 2018 08:44:55 GMT  
		Size: 2.1 MB (2099762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae94b3cb7a1b2cef0ceffe3303cd03f83434d283aab43389e586b42bea00b358`  
		Last Modified: Wed, 12 Sep 2018 08:44:55 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fbd813e350b4987a2ae8ea02e0a5e9f94bdf531dbd060fb3f9b48f75615e79`  
		Last Modified: Sat, 15 Sep 2018 11:32:25 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0c4e1e080718745f6953bd2c106b3a8f95d80969ae1170c532d005111bc038`  
		Last Modified: Sat, 15 Sep 2018 11:32:25 GMT  
		Size: 400.5 KB (400519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41468f81c7bee9dd3d7e0f866672320e52e1238d0b9dc0516e0ff3df6bffd3db`  
		Last Modified: Sat, 15 Sep 2018 11:34:38 GMT  
		Size: 6.6 MB (6629493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b21ca937eaf55bfcf6f9af44122c1d818863af9aabac5d23594226bf23b9e9`  
		Last Modified: Sat, 15 Sep 2018 11:34:35 GMT  
		Size: 101.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc321d3c0ce6c67ff94a5651a8ee07fa4c7e400c8ccc0e2e437913b6da4775f3`  
		Last Modified: Wed, 03 Oct 2018 10:18:13 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:3-alpine` - linux; 386

```console
$ docker pull redis@sha256:b5d3a8ea62abe72a1030d8a5bbd2740227d9961172aeb4762ddebe5387f92697
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9154068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806b2d540b7d806914919e0d24a919697b08bcf990273a52efe71bd26700e361`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 12 Sep 2018 10:38:54 GMT
ADD file:b789aca08d6985c0bf373a2ca5f2a263d45e3a789aa6bbcd1fe1d47133f985d2 in / 
# Wed, 12 Sep 2018 10:38:54 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 10:38:54 GMT
CMD ["/bin/sh"]
# Wed, 12 Sep 2018 17:19:49 GMT
RUN addgroup -S redis && adduser -S -G redis redis
# Wed, 12 Sep 2018 17:19:51 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 12 Sep 2018 17:21:53 GMT
ENV REDIS_VERSION=3.2.12
# Wed, 12 Sep 2018 17:21:53 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-3.2.12.tar.gz
# Wed, 12 Sep 2018 17:21:53 GMT
ENV REDIS_DOWNLOAD_SHA=98c4254ae1be4e452aa7884245471501c9aa657993e0318d88f048093e7f88fd
# Wed, 12 Sep 2018 17:22:21 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		jemalloc-dev 		linux-headers 		make 		musl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)"; 	make -C /usr/src/redis install; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .redis-rundeps $runDeps; 	apk del .build-deps; 		redis-server --version
# Wed, 12 Sep 2018 17:22:22 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 12 Sep 2018 17:22:22 GMT
VOLUME [/data]
# Wed, 12 Sep 2018 17:22:22 GMT
WORKDIR /data
# Wed, 03 Oct 2018 12:03:08 GMT
COPY file:592b00f2927fa2144858cc8c78ef610815375a7ed6046b2460776997a98d663a in /usr/local/bin/ 
# Wed, 03 Oct 2018 12:03:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Oct 2018 12:03:09 GMT
EXPOSE 6379/tcp
# Wed, 03 Oct 2018 12:03:09 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:6b5c2e9bbf9885ccefe772a5a1f471d7da4315b7bf43ec3b4c014a65d04073b1`  
		Last Modified: Wed, 12 Sep 2018 10:39:28 GMT  
		Size: 2.3 MB (2271460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d99e807699886f28203b3284584d7b093a61a84c40230f7094513bb2f84cd2`  
		Last Modified: Wed, 12 Sep 2018 10:39:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66f3eda904fd49ce410925fb7a9c881efd1a8963c0629d993094e288faa52b4`  
		Last Modified: Wed, 12 Sep 2018 17:22:41 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc8259a71237d638c384b24f5a1dceb2c11501d45c4f34bec4569a3a8ed464c`  
		Last Modified: Wed, 12 Sep 2018 17:22:42 GMT  
		Size: 406.6 KB (406559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31a1d7a2166ce374c3b016d4e10deecee77f0679224346fe96f9330de0d6e96`  
		Last Modified: Wed, 12 Sep 2018 17:23:46 GMT  
		Size: 6.5 MB (6474112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3a8217905e41892971abfab51d0fe3e25f104eef02f76f756ae8bc8d9c106a`  
		Last Modified: Wed, 12 Sep 2018 17:23:44 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4913c80e13aee3ca866f4b5cd950e3addf2a72b475371642835181d13f1c8024`  
		Last Modified: Wed, 03 Oct 2018 12:06:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:3-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:896c9b129a6800eb7bceb234525b856b212765dffc203c1c6c95c45432c271f4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9478026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b530eab5903a723371f536e9d37e034cf451418034fa5245cb6f688b9587fb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 12 Sep 2018 08:18:11 GMT
ADD file:0991fe2a00b8319ade0b97ea20b79708b45153da36419ca58378c8bece0f987c in / 
# Wed, 12 Sep 2018 08:18:13 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 08:18:14 GMT
CMD ["/bin/sh"]
# Wed, 12 Sep 2018 12:46:51 GMT
RUN addgroup -S redis && adduser -S -G redis redis
# Wed, 12 Sep 2018 12:46:56 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 12 Sep 2018 12:49:38 GMT
ENV REDIS_VERSION=3.2.12
# Wed, 12 Sep 2018 12:49:40 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-3.2.12.tar.gz
# Wed, 12 Sep 2018 12:49:41 GMT
ENV REDIS_DOWNLOAD_SHA=98c4254ae1be4e452aa7884245471501c9aa657993e0318d88f048093e7f88fd
# Wed, 12 Sep 2018 12:50:10 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		jemalloc-dev 		linux-headers 		make 		musl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)"; 	make -C /usr/src/redis install; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .redis-rundeps $runDeps; 	apk del .build-deps; 		redis-server --version
# Wed, 12 Sep 2018 12:50:13 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 12 Sep 2018 12:50:14 GMT
VOLUME [/data]
# Wed, 12 Sep 2018 12:50:15 GMT
WORKDIR /data
# Wed, 03 Oct 2018 10:27:15 GMT
COPY file:592b00f2927fa2144858cc8c78ef610815375a7ed6046b2460776997a98d663a in /usr/local/bin/ 
# Wed, 03 Oct 2018 10:27:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Oct 2018 10:27:17 GMT
EXPOSE 6379/tcp
# Wed, 03 Oct 2018 10:27:18 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d6201b52ea9b908d4d6e950e2a79ded27be48979d6f0f63bd3a57b16b621f188`  
		Last Modified: Wed, 12 Sep 2018 08:19:46 GMT  
		Size: 2.2 MB (2195226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5cedde51de1c8ffccd5521fd02fc1efc1cc44ece2d5dccb1e550a65366cd80`  
		Last Modified: Wed, 12 Sep 2018 08:19:44 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf7586f18b2066373cb5094be8898e1e33840c1f4cddee3e8f8b873075fb5ab`  
		Last Modified: Wed, 12 Sep 2018 12:50:56 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92415845fc066af3f720f0e6b9e348e4769da935329f65effd80736be62d1f91`  
		Last Modified: Wed, 12 Sep 2018 12:50:56 GMT  
		Size: 406.8 KB (406845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2721b6afd483e4f445f5ea752a9981c2ee3e0533bf19af6367e26a59b3cb314a`  
		Last Modified: Wed, 12 Sep 2018 12:53:28 GMT  
		Size: 6.9 MB (6873947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a86dafe109cdd333430821309c6391396d7670e213b729332ce59548acda2f`  
		Last Modified: Wed, 12 Sep 2018 12:53:25 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cdcb0a11df72e0e0b9bdddfe715f3c9a9ea49ed6e6ba2ea4018d6dbe94ab81`  
		Last Modified: Wed, 03 Oct 2018 10:38:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:3-alpine` - linux; s390x

```console
$ docker pull redis@sha256:a6ea3eae6800c7fb60bb7bc21143bf7174fd45342d1c93aa6ddf91f66a6e827c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9592669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d60e39bc4b1a15aa522fcc12156669e670a44ea15a0c47a4471ca1ac2095d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 12 Sep 2018 11:42:25 GMT
ADD file:532f451315fcf5c4077ef91f62d9838cf5681b4a348af2d78f6edd825146612c in / 
# Wed, 12 Sep 2018 11:42:25 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 11:42:25 GMT
CMD ["/bin/sh"]
# Wed, 12 Sep 2018 13:19:49 GMT
RUN addgroup -S redis && adduser -S -G redis redis
# Wed, 12 Sep 2018 13:19:50 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 12 Sep 2018 13:21:25 GMT
ENV REDIS_VERSION=3.2.12
# Wed, 12 Sep 2018 13:21:26 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-3.2.12.tar.gz
# Wed, 12 Sep 2018 13:21:26 GMT
ENV REDIS_DOWNLOAD_SHA=98c4254ae1be4e452aa7884245471501c9aa657993e0318d88f048093e7f88fd
# Wed, 12 Sep 2018 13:21:52 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		jemalloc-dev 		linux-headers 		make 		musl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)"; 	make -C /usr/src/redis install; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .redis-rundeps $runDeps; 	apk del .build-deps; 		redis-server --version
# Wed, 12 Sep 2018 13:21:53 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 12 Sep 2018 13:21:53 GMT
VOLUME [/data]
# Wed, 12 Sep 2018 13:21:53 GMT
WORKDIR /data
# Wed, 03 Oct 2018 12:25:46 GMT
COPY file:592b00f2927fa2144858cc8c78ef610815375a7ed6046b2460776997a98d663a in /usr/local/bin/ 
# Wed, 03 Oct 2018 12:25:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Oct 2018 12:25:46 GMT
EXPOSE 6379/tcp
# Wed, 03 Oct 2018 12:25:46 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:e5d7a290acc264d66e5c29923d4b8a79135ffd15887225581968bf7df22fb281`  
		Last Modified: Wed, 12 Sep 2018 11:43:25 GMT  
		Size: 2.3 MB (2307746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad01149bcd3bd207c03ab0c38897be9653222644a37b651c399c24f1e9170313`  
		Last Modified: Wed, 12 Sep 2018 11:43:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4783fcf5616fd256cd37b848c921a4c368fb868509715757477d1719e8ad5f`  
		Last Modified: Wed, 12 Sep 2018 13:22:18 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a126c000d8dae10977adebe9cfc4a4adf463db95e95f790eb271bd6b675c99de`  
		Last Modified: Wed, 12 Sep 2018 13:22:18 GMT  
		Size: 407.8 KB (407806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43336f15350cd5bb43b79e02d13654e0c092fe54f2d6cab2c1dfc9e38b59245`  
		Last Modified: Wed, 12 Sep 2018 13:23:57 GMT  
		Size: 6.9 MB (6875177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f584079375e63f716a364445b97e6a244c6a9f38ec25be1215b292fb00bf2897`  
		Last Modified: Wed, 12 Sep 2018 13:23:55 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b08289f952ff3896611c08a6bb8eaf7f356181eea619531e1facf00f9187e`  
		Last Modified: Wed, 03 Oct 2018 12:30:27 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
