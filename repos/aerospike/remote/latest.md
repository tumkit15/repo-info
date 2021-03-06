## `aerospike:latest`

```console
$ docker pull aerospike@sha256:f0416ac5cb39e30ca3eafa86252c9acfd7f5b9ecd9491ee12d3895796b6f676f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:23a968f692a1d39472d9e0a44975d517117b299bcf8e1492d12f2a65dc1db40b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48762581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06f614f5f50570ce3f0d252657a48dd8a9510308b468312569e32ba1130a4094`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 04 Sep 2018 21:21:34 GMT
ADD file:e6ca98733431f75e97eb09758ba64065d213d51bd2070a95cf15f2ff5adccfc4 in / 
# Tue, 04 Sep 2018 21:21:34 GMT
CMD ["bash"]
# Mon, 01 Oct 2018 23:19:28 GMT
ENV AEROSPIKE_VERSION=4.3.0.8
# Mon, 01 Oct 2018 23:19:28 GMT
ENV AEROSPIKE_SHA256=dbddf87e806355edcc47c809f21ee9d8d6313cb4be6c2c25c4b2ca50e9d7d426
# Mon, 01 Oct 2018 23:19:47 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 01 Oct 2018 23:19:47 GMT
COPY file:92f154ac5768cc66c29bd7ca3d00a0fe0ae8d08f1d309fdcda8bf66d4c73cadd in /etc/aerospike/aerospike.template.conf 
# Mon, 01 Oct 2018 23:19:47 GMT
COPY file:7eece3188902a85a78ecb96d2ec561fce45fa1728926bc66f3903d6955630907 in /entrypoint.sh 
# Mon, 01 Oct 2018 23:19:48 GMT
VOLUME [/opt/aerospike/data]
# Mon, 01 Oct 2018 23:19:48 GMT
EXPOSE 3000/tcp 3001/tcp 3002/tcp 3003/tcp
# Mon, 01 Oct 2018 23:19:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Oct 2018 23:19:48 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:802b00ed6f79f48e6a5f44ecbcaf43563d6077aaecb565eee1dfc615c0b18c00`  
		Last Modified: Tue, 04 Sep 2018 21:25:45 GMT  
		Size: 22.5 MB (22485965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb1451974cfed1a4ecc8fc3aba2c88fe44569de7d421dd72449cb6a8eafadb4`  
		Last Modified: Mon, 01 Oct 2018 23:20:05 GMT  
		Size: 26.3 MB (26274622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c437d5705993e43de9aea0a8e17cff5b7a9b8786815f0f0c78a62718e06f72f`  
		Last Modified: Mon, 01 Oct 2018 23:20:00 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417c8419823ad05751d5c4e2ee0fe8eafa0ea5ff0075e7365d1179d412230471`  
		Last Modified: Mon, 01 Oct 2018 23:20:00 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
