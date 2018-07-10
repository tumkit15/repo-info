## `traefik:maroilles`

```console
$ docker pull traefik@sha256:96fdda85a7d2b78f4e18b125766f6618e5db518c995dfe951ec116e9f0f5ae62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:691d7e42caa2acd9a5d345b184d520cb2c123c68cd305431cd3a05212a4a1712
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16065760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee9981468308bf3b226f09eb995b4cf7ccedbd95428fbef5ead93bbf68dd9dc3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Sat, 16 Jun 2018 06:01:27 GMT
COPY file:d8282341d1fb7d2cc3d5d3523d0d4126066cc1ba8abe3f0047a459b3a63a5653 in /etc/ssl/certs/ 
# Mon, 09 Jul 2018 20:27:44 GMT
COPY file:9b1408023ea2f3c134a52dd09288e3085e202068adee702a21097b1e2c671bc1 in / 
# Mon, 09 Jul 2018 20:27:44 GMT
EXPOSE 80/tcp
# Mon, 09 Jul 2018 20:27:44 GMT
ENTRYPOINT ["/traefik"]
# Mon, 09 Jul 2018 20:27:45 GMT
LABEL org.label-schema.vendor=Containous org.label-schema.url=https://traefik.io org.label-schema.name=Traefik org.label-schema.description=A modern reverse-proxy org.label-schema.version=v1.7.0-rc1 org.label-schema.docker.schema-version=1.0
```

-	Layers:
	-	`sha256:03732cc4924a93fcbcbed879c4c63aad534a63a64e9919eceddf48d7602407b5`  
		Last Modified: Sat, 16 Jun 2018 06:03:25 GMT  
		Size: 155.2 KB (155150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e40814c4f731dcedbdf25bcc7b0b556525c9dc46bacc8025bf0b78a827c33`  
		Last Modified: Mon, 09 Jul 2018 20:28:55 GMT  
		Size: 15.9 MB (15910610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ca85f5babca632760c09136c283548495d096c2639115e8ce0ee39aa17f657e5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15409504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba5fe7a70388ecbb3fa583491d2f63cded6198202bfce2bf648ee05306d9746a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Oct 2017 23:48:27 GMT
COPY file:d8282341d1fb7d2cc3d5d3523d0d4126066cc1ba8abe3f0047a459b3a63a5653 in /etc/ssl/certs/ 
# Mon, 09 Jul 2018 21:43:24 GMT
COPY file:71383cd05a0ee9f71305cbd667ce6edac2a194ce64677a0e8ef68097fcd9e181 in / 
# Mon, 09 Jul 2018 21:43:24 GMT
EXPOSE 80/tcp
# Mon, 09 Jul 2018 21:43:24 GMT
ENTRYPOINT ["/traefik"]
# Mon, 09 Jul 2018 21:43:25 GMT
LABEL org.label-schema.vendor=Containous org.label-schema.url=https://traefik.io org.label-schema.name=Traefik org.label-schema.description=A modern reverse-proxy org.label-schema.version=v1.7.0-rc1 org.label-schema.docker.schema-version=1.0
```

-	Layers:
	-	`sha256:8996ab8c9ae2c6afe7d318a3784c7ba1b1b72d4ae14cf515d4c1490aae91cab0`  
		Last Modified: Tue, 24 Oct 2017 23:48:35 GMT  
		Size: 155.2 KB (155184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c020c7b945f84af3e2a57af6da04a9806271c79777608b36bdc669f29bde271`  
		Last Modified: Mon, 09 Jul 2018 21:43:57 GMT  
		Size: 15.3 MB (15254320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6ae45c41cc0f5701b52764e90a2e6017610e9ecf20eef007136fd8ba174c353d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15122453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e2ae6097c86cec25a16d622b23f17fef6d87fc3c6cb104b746c17e5758a633`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 25 Oct 2017 04:54:39 GMT
COPY file:d8282341d1fb7d2cc3d5d3523d0d4126066cc1ba8abe3f0047a459b3a63a5653 in /etc/ssl/certs/ 
# Mon, 09 Jul 2018 21:43:06 GMT
COPY file:a74582378f872557ea509f8729ef17eeffee5ba69e9cb72544e48bf011e9f1ab in / 
# Mon, 09 Jul 2018 21:43:07 GMT
EXPOSE 80/tcp
# Mon, 09 Jul 2018 21:43:08 GMT
ENTRYPOINT ["/traefik"]
# Mon, 09 Jul 2018 21:43:08 GMT
LABEL org.label-schema.vendor=Containous org.label-schema.url=https://traefik.io org.label-schema.name=Traefik org.label-schema.description=A modern reverse-proxy org.label-schema.version=v1.7.0-rc1 org.label-schema.docker.schema-version=1.0
```

-	Layers:
	-	`sha256:78fe135ba97a13abc86dbe373975f0d0712d8aa6e540e09824b715a55d7e2ed3`  
		Last Modified: Wed, 25 Oct 2017 04:55:01 GMT  
		Size: 155.2 KB (155151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc33a79bee9249a4f3e4c16ec38b1b5bed8835b2b59902697f16b4908f9a0fa`  
		Last Modified: Mon, 09 Jul 2018 21:44:19 GMT  
		Size: 15.0 MB (14967302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip