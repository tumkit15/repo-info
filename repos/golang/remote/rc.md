## `golang:rc`

```console
$ docker pull golang@sha256:6e4185a2e6e74cb8059ecb6d30f8b16b9e1d8c604a83e10116a7c3c2e8a94522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.14393.2312; amd64
	-	windows version 10.0.16299.492; amd64

### `golang:rc` - linux; amd64

```console
$ docker pull golang@sha256:3e90d12c0512b7daecc3bde25dfa2311fb90e8b1929085af8463978cbeee07c7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.4 MB (337375888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f1aa64fd70186d8e976f5134659b04b7bc184bfe425f8396f5195621a0cf9c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Jun 2018 21:24:58 GMT
ADD file:f21d7c14104d5d9fa99f271177e765a3472f5a69398bb78f34f7401e9b2df837 in / 
# Tue, 26 Jun 2018 21:24:58 GMT
CMD ["bash"]
# Tue, 26 Jun 2018 22:16:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 26 Jun 2018 22:16:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jun 2018 22:17:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 22:20:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 22:20:11 GMT
ENV GOLANG_VERSION=1.11beta1
# Wed, 27 Jun 2018 22:20:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='df7fe096ffab5d331d35c6d038d2ec0426b45ce17f55a93037e371d3af9d4e6d' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='844ed9e34b118a9c2b069a18924a7879236929e08c887a92e5be1af5d701fb90' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='9c1795148e777c81ac3cb381e3ea970eea60f5db2323658c061e5c4382125dd4' ;; 		i386) goRelArch='linux-386'; goRelSha256='a6e804652f58785b3dfe272d96b8206250210e7ba7bdcb1ffb726ab3753db4af' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='66529a525c0369d2b79ecd19f6d16444ed162c9bf88f7b37715520841c36de65' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='731b9e6ac0d4c9709297f0efc1a6455589b978d2ecc207184d3e5be07a130c9c' ;; 		*) goRelArch='src'; goRelSha256='5955eeb8f45e02aa5357fc18e62f1fe6c1b19e0c50aba93b8b9d9ef13b862dda'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 27 Jun 2018 22:20:30 GMT
ENV GOPATH=/go
# Wed, 27 Jun 2018 22:20:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jun 2018 22:20:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 27 Jun 2018 22:20:31 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0bd44ff9c2cf1129ef8cea689b3e10e6498f64d2f8d5532caae55841b474bf3a`  
		Last Modified: Tue, 26 Jun 2018 21:36:36 GMT  
		Size: 45.3 MB (45319224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047670ddbd2a37cb7940be99332555b0a9f4f2531802e50c06128c340ccd0c0d`  
		Last Modified: Tue, 26 Jun 2018 22:30:05 GMT  
		Size: 10.8 MB (10774053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7d5dc8943870545f4eecc6b06b3fd6b12b987dc99f0bbcfee8f132044fc9e2`  
		Last Modified: Tue, 26 Jun 2018 22:30:03 GMT  
		Size: 4.3 MB (4336270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ad5906a7580677bdf8a8d57749814520c2c6a2054604c115ba6e8646363aa`  
		Last Modified: Tue, 26 Jun 2018 22:30:55 GMT  
		Size: 50.1 MB (50062264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f6351ddb3796295061478a28f09752a99b61fdb5160e0456b687f3dd52e04a`  
		Last Modified: Wed, 27 Jun 2018 22:29:30 GMT  
		Size: 57.6 MB (57565582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d930c1545f5f8dd60d33f27b95cc6f26f9f30759d37264ef84a1f9081014e7`  
		Last Modified: Wed, 27 Jun 2018 22:29:50 GMT  
		Size: 169.3 MB (169318369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e30fc2f13a0a23db1d40bbddb264db6de62b51920c5f6aeaa143a34e144ac00`  
		Last Modified: Wed, 27 Jun 2018 22:29:09 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; arm variant v7

```console
$ docker pull golang@sha256:b3c43aa08b9ce5b24b91d222b87c83913895efd06c05db3790a1549eafd90997
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.4 MB (291393867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040666997a7227ed83c1ea77073172ff604085109cec247eaf165c993abea665`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Jun 2018 12:03:26 GMT
ADD file:b928e6adeb71af1928fc7b8e0ff4770e5521eebf544a3b27f9736ac86e7a0ffa in / 
# Wed, 27 Jun 2018 12:03:27 GMT
CMD ["bash"]
# Wed, 27 Jun 2018 12:47:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 12:47:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 27 Jun 2018 12:48:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 15:48:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jun 2018 11:57:30 GMT
ENV GOLANG_VERSION=1.11beta1
# Thu, 28 Jun 2018 11:57:50 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='df7fe096ffab5d331d35c6d038d2ec0426b45ce17f55a93037e371d3af9d4e6d' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='844ed9e34b118a9c2b069a18924a7879236929e08c887a92e5be1af5d701fb90' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='9c1795148e777c81ac3cb381e3ea970eea60f5db2323658c061e5c4382125dd4' ;; 		i386) goRelArch='linux-386'; goRelSha256='a6e804652f58785b3dfe272d96b8206250210e7ba7bdcb1ffb726ab3753db4af' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='66529a525c0369d2b79ecd19f6d16444ed162c9bf88f7b37715520841c36de65' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='731b9e6ac0d4c9709297f0efc1a6455589b978d2ecc207184d3e5be07a130c9c' ;; 		*) goRelArch='src'; goRelSha256='5955eeb8f45e02aa5357fc18e62f1fe6c1b19e0c50aba93b8b9d9ef13b862dda'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 28 Jun 2018 11:57:54 GMT
ENV GOPATH=/go
# Thu, 28 Jun 2018 11:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jun 2018 11:57:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jun 2018 11:57:56 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c675459249e5e2b5c2119c5965490fb00918a71cd19ba6a70e1c14ea0366cc9a`  
		Last Modified: Wed, 27 Jun 2018 12:12:46 GMT  
		Size: 42.1 MB (42062253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87675d75ec387a55e1b055dfadf15fd7137586ee9acf9be9b2a4840e4001b2a`  
		Last Modified: Wed, 27 Jun 2018 12:58:52 GMT  
		Size: 9.5 MB (9472634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55e83b4f681428c2fb1542a44d864d0d2f78d235199a33824985049fd42bb5`  
		Last Modified: Wed, 27 Jun 2018 12:58:50 GMT  
		Size: 3.9 MB (3913173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf79f9923b0cece59f9957dddd92e7c5cd6c8c3311984ae5249217f97be3d0f`  
		Last Modified: Wed, 27 Jun 2018 12:59:26 GMT  
		Size: 46.4 MB (46382240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91904e79c32d2fea51aa29f9e3b8f4dad43884af7ce77c6b01c3c5e334a1c2bf`  
		Last Modified: Wed, 27 Jun 2018 15:49:59 GMT  
		Size: 45.9 MB (45906205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adacd16ea4fb01632a667101f07200853f476df3201ae0d0899350f0a06b8095`  
		Last Modified: Thu, 28 Jun 2018 11:58:56 GMT  
		Size: 143.7 MB (143657206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468a66405f9e651a6ae18a1a96719c5ad6805061994b670cb701837f4be10e9`  
		Last Modified: Thu, 28 Jun 2018 11:58:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:839b97ed642a60174ff4a5e8795b4103cb0c311f4aa4344d40eef71f8d52726b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297446243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e789c7e021c8e525c92d5cb3c3290dfa6461205ba10ad4e7968fed08c7f1fee3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Jun 2018 08:47:01 GMT
ADD file:0f69db95e9a06ee21c38014c8bc6c142be97ec4d5127ba83f1d0ef48806f7415 in / 
# Wed, 27 Jun 2018 08:47:02 GMT
CMD ["bash"]
# Wed, 27 Jun 2018 10:46:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 10:47:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 27 Jun 2018 10:48:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 21:54:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jun 2018 08:45:52 GMT
ENV GOLANG_VERSION=1.11beta1
# Thu, 28 Jun 2018 08:46:18 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='df7fe096ffab5d331d35c6d038d2ec0426b45ce17f55a93037e371d3af9d4e6d' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='844ed9e34b118a9c2b069a18924a7879236929e08c887a92e5be1af5d701fb90' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='9c1795148e777c81ac3cb381e3ea970eea60f5db2323658c061e5c4382125dd4' ;; 		i386) goRelArch='linux-386'; goRelSha256='a6e804652f58785b3dfe272d96b8206250210e7ba7bdcb1ffb726ab3753db4af' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='66529a525c0369d2b79ecd19f6d16444ed162c9bf88f7b37715520841c36de65' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='731b9e6ac0d4c9709297f0efc1a6455589b978d2ecc207184d3e5be07a130c9c' ;; 		*) goRelArch='src'; goRelSha256='5955eeb8f45e02aa5357fc18e62f1fe6c1b19e0c50aba93b8b9d9ef13b862dda'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 28 Jun 2018 08:46:19 GMT
ENV GOPATH=/go
# Thu, 28 Jun 2018 08:46:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jun 2018 08:46:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jun 2018 08:46:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6054c6775a4e4515d2365ad9337e322dd5c6ad0e0bc8e5bb6b0252461e71afc4`  
		Last Modified: Wed, 27 Jun 2018 08:57:38 GMT  
		Size: 43.1 MB (43115791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d57f1ab872b53f8ac8eff946226a3ff9d5fb929656964b75dae06303e9c8ef4`  
		Last Modified: Wed, 27 Jun 2018 11:06:29 GMT  
		Size: 9.7 MB (9722190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e63f6b578575fadc2ae00bf10794a2a45166c03105d940c919da9f78c1c43`  
		Last Modified: Wed, 27 Jun 2018 11:06:28 GMT  
		Size: 4.1 MB (4088526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242c1552cb593c1f860dd482a21f1607a2965ef9ac5b5a29aad2a768ce9d699a`  
		Last Modified: Wed, 27 Jun 2018 11:07:20 GMT  
		Size: 48.0 MB (48002203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5fcd394e27d6088067f637bd3c0755a34ef456e102c0fad7bd17ef33cd7e14`  
		Last Modified: Wed, 27 Jun 2018 21:56:34 GMT  
		Size: 49.0 MB (48970237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f265b2dad76b328044beb0165c04a7b94af2775cbce766a278227ed5fa51e5ca`  
		Last Modified: Thu, 28 Jun 2018 08:51:39 GMT  
		Size: 143.5 MB (143547170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3efe661769a2cb034dcb26c3d34aa68cfe0f0f63d096ebbb3ffb5474941ec`  
		Last Modified: Thu, 28 Jun 2018 08:50:53 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; 386

```console
$ docker pull golang@sha256:9a2ca1f2c46757fa766256d659451665a336c83b6cdbcb864b7f0d185480cbc9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328038391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f28a8183271eb727bbcfc5004b2756734324ded2ca3423292792bc96153c7f6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 10:41:35 GMT
ADD file:df99f919c7f5a407abee5c74ea019e497e559a75bdd21b36ae581e81230884c3 in / 
# Sat, 28 Apr 2018 10:41:36 GMT
CMD ["bash"]
# Wed, 06 Jun 2018 11:41:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 11:42:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Jun 2018 11:42:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 12:42:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jun 2018 10:38:54 GMT
ENV GOLANG_VERSION=1.11beta1
# Thu, 28 Jun 2018 10:39:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='df7fe096ffab5d331d35c6d038d2ec0426b45ce17f55a93037e371d3af9d4e6d' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='844ed9e34b118a9c2b069a18924a7879236929e08c887a92e5be1af5d701fb90' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='9c1795148e777c81ac3cb381e3ea970eea60f5db2323658c061e5c4382125dd4' ;; 		i386) goRelArch='linux-386'; goRelSha256='a6e804652f58785b3dfe272d96b8206250210e7ba7bdcb1ffb726ab3753db4af' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='66529a525c0369d2b79ecd19f6d16444ed162c9bf88f7b37715520841c36de65' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='731b9e6ac0d4c9709297f0efc1a6455589b978d2ecc207184d3e5be07a130c9c' ;; 		*) goRelArch='src'; goRelSha256='5955eeb8f45e02aa5357fc18e62f1fe6c1b19e0c50aba93b8b9d9ef13b862dda'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 28 Jun 2018 10:39:18 GMT
ENV GOPATH=/go
# Thu, 28 Jun 2018 10:39:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jun 2018 10:39:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jun 2018 10:39:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5b858ae16eb844c6834e74a5c76644142d36957121de3f9bccf66d4c10b18816`  
		Last Modified: Sat, 28 Apr 2018 10:48:56 GMT  
		Size: 46.0 MB (46044885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fb0be3608d00a27aadd5246acebfa684875786308e5e07bd72ecedb1ea550e`  
		Last Modified: Wed, 06 Jun 2018 12:17:46 GMT  
		Size: 10.8 MB (10784612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109b3030038f2425d43d6f1796554d59323fd256fe621bd3a73249279da3a2e7`  
		Last Modified: Wed, 06 Jun 2018 12:17:44 GMT  
		Size: 4.6 MB (4555092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af01b2a73367b29b158a599b31f1a8d0e0e964f8ba899158fe801dca9aa54f`  
		Last Modified: Wed, 06 Jun 2018 12:18:38 GMT  
		Size: 51.6 MB (51593154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1180ff77f44b4c76845b640e811eb8ab26f087d893e0d368fc331c0ba05766bc`  
		Last Modified: Wed, 06 Jun 2018 12:53:25 GMT  
		Size: 62.1 MB (62091972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb454ca45fda579f08c1ec08af62fdfd24c3de3710b75fa2ab330872f304653`  
		Last Modified: Thu, 28 Jun 2018 10:43:31 GMT  
		Size: 153.0 MB (152968550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e71dabc643d63bb3c653c40170b232533ba10326504974be07441edf3716727`  
		Last Modified: Thu, 28 Jun 2018 10:42:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; ppc64le

```console
$ docker pull golang@sha256:0c3db19b60d19bb2e697eba5e90457963e8a993d2f189888ae83a491c87ad7c8
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.8 MB (304803747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a35be15d8a7e7377927a88aba9f2b99662e6bbb323fe56e4d185af441b9fab9c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Jun 2018 08:21:02 GMT
ADD file:d33614b8c4f66955a915157517ae82c889e6367cfc17a0d89ff64b91c984d7ef in / 
# Wed, 27 Jun 2018 08:21:04 GMT
CMD ["bash"]
# Wed, 27 Jun 2018 10:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 10:15:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 27 Jun 2018 10:16:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 14:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jun 2018 08:16:48 GMT
ENV GOLANG_VERSION=1.11beta1
# Thu, 28 Jun 2018 08:17:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='df7fe096ffab5d331d35c6d038d2ec0426b45ce17f55a93037e371d3af9d4e6d' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='844ed9e34b118a9c2b069a18924a7879236929e08c887a92e5be1af5d701fb90' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='9c1795148e777c81ac3cb381e3ea970eea60f5db2323658c061e5c4382125dd4' ;; 		i386) goRelArch='linux-386'; goRelSha256='a6e804652f58785b3dfe272d96b8206250210e7ba7bdcb1ffb726ab3753db4af' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='66529a525c0369d2b79ecd19f6d16444ed162c9bf88f7b37715520841c36de65' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='731b9e6ac0d4c9709297f0efc1a6455589b978d2ecc207184d3e5be07a130c9c' ;; 		*) goRelArch='src'; goRelSha256='5955eeb8f45e02aa5357fc18e62f1fe6c1b19e0c50aba93b8b9d9ef13b862dda'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 28 Jun 2018 08:17:11 GMT
ENV GOPATH=/go
# Thu, 28 Jun 2018 08:17:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jun 2018 08:17:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jun 2018 08:17:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:80b856b58d8f74e5617ff0b59e5192bd26540b867890becb80ac3b1766e68d1d`  
		Last Modified: Wed, 27 Jun 2018 08:30:43 GMT  
		Size: 45.6 MB (45587028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a98fa77416c63ffab99d98aea7befc5a0d53ec23ebff6abaa40b528d9ca971`  
		Last Modified: Wed, 27 Jun 2018 10:28:49 GMT  
		Size: 10.0 MB (9976097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd479833a536a5f1d2afb81f4d98a720d841227f1a3e2345238f8f966ace8c59`  
		Last Modified: Wed, 27 Jun 2018 10:28:48 GMT  
		Size: 4.3 MB (4289938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4645fc917f498a9483cc812c5015aa0bcb956be63b25957067bc030e84289c`  
		Last Modified: Wed, 27 Jun 2018 10:29:34 GMT  
		Size: 50.1 MB (50059206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f874cd164630c460c93d7b387a05c7bc24f20f1a61d522cfbb2c7928ca28ab1`  
		Last Modified: Wed, 27 Jun 2018 14:43:54 GMT  
		Size: 52.7 MB (52737934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6857eace7b440d04f70e33517c397aa9a2fed6859b4f5b4f7e2ab2e0e6cf29`  
		Last Modified: Thu, 28 Jun 2018 08:21:39 GMT  
		Size: 142.2 MB (142153388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41047d18db461fd2f7daefbd5deab99771c56c4ea25300a06b1cc865b95472c9`  
		Last Modified: Thu, 28 Jun 2018 08:21:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; s390x

```console
$ docker pull golang@sha256:c973a5ff25e08427e7b08b157d29652441115e19ffd2120eaf049fd08724d5e4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.3 MB (298291498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ec9918da9f8dc5dda907f5d768fa3d0e3db890e5402ca5d1cbafafd9901a6a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Jun 2018 11:48:36 GMT
ADD file:75083687b6ec1b46a3ccf759184d7da7ea89555c516ec0b9fe7307869e6e068d in / 
# Wed, 27 Jun 2018 11:48:36 GMT
CMD ["bash"]
# Wed, 27 Jun 2018 12:20:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 12:20:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 27 Jun 2018 12:20:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 15:08:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jun 2018 11:43:54 GMT
ENV GOLANG_VERSION=1.11beta1
# Thu, 28 Jun 2018 11:44:05 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='df7fe096ffab5d331d35c6d038d2ec0426b45ce17f55a93037e371d3af9d4e6d' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='844ed9e34b118a9c2b069a18924a7879236929e08c887a92e5be1af5d701fb90' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='9c1795148e777c81ac3cb381e3ea970eea60f5db2323658c061e5c4382125dd4' ;; 		i386) goRelArch='linux-386'; goRelSha256='a6e804652f58785b3dfe272d96b8206250210e7ba7bdcb1ffb726ab3753db4af' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='66529a525c0369d2b79ecd19f6d16444ed162c9bf88f7b37715520841c36de65' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='731b9e6ac0d4c9709297f0efc1a6455589b978d2ecc207184d3e5be07a130c9c' ;; 		*) goRelArch='src'; goRelSha256='5955eeb8f45e02aa5357fc18e62f1fe6c1b19e0c50aba93b8b9d9ef13b862dda'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 28 Jun 2018 11:44:06 GMT
ENV GOPATH=/go
# Thu, 28 Jun 2018 11:44:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jun 2018 11:44:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jun 2018 11:44:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:879ec09c190353266c9e5cb180d35fce7e1d21e2ed3f577f2708dba824290cec`  
		Last Modified: Wed, 27 Jun 2018 11:53:15 GMT  
		Size: 45.2 MB (45181422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cd1564a39a86ccb42d24db5044f7c0fc4f4057eb7acae6f1b7b2e4c582cd5a`  
		Last Modified: Wed, 27 Jun 2018 12:25:12 GMT  
		Size: 10.3 MB (10301218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d677b03f5d7f43f597f3ca3119cce61767eafd68c1cd48fd083dc3eae703de`  
		Last Modified: Wed, 27 Jun 2018 12:25:11 GMT  
		Size: 4.4 MB (4367019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db908d0308fa64224122e4e37c21ce2473cb5be8b9ac64a32dd006a61e947783`  
		Last Modified: Wed, 27 Jun 2018 12:25:37 GMT  
		Size: 50.5 MB (50478409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e39745d356e34f6b9f83861a8c1868f5a2a49af7e2ca2d3fac679ad8da02ad`  
		Last Modified: Wed, 27 Jun 2018 15:09:43 GMT  
		Size: 45.8 MB (45846483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8d9ee9ffc5a0a9333dce9d7351bd2a6a3a98f1a1bddda4072265ca2bb069f3`  
		Last Modified: Thu, 28 Jun 2018 11:47:31 GMT  
		Size: 142.1 MB (142116821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bdb504878b64aa3e15a1ca2136d532d640b0042e0e9f49a18bfbdd510b12c2`  
		Last Modified: Thu, 28 Jun 2018 11:46:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - windows version 10.0.14393.2312; amd64

```console
$ docker pull golang@sha256:5b1119fc42d197c112590d629d9d687447cf6350fc51b26fc3399e94a774a1b5
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5700450351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294da10a0eaf0e448b27c83773759bff0fa2cfe2ff98f7190089665aae8e42c3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Wed, 13 Jun 2018 00:36:30 GMT
RUN Install update 10.0.14393.2312
# Tue, 03 Jul 2018 00:23:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 03 Jul 2018 00:23:43 GMT
ENV GIT_VERSION=2.11.1
# Tue, 03 Jul 2018 00:23:44 GMT
ENV GIT_TAG=v2.11.1.windows.1
# Tue, 03 Jul 2018 00:23:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.11.1.windows.1/MinGit-2.11.1-64-bit.zip
# Tue, 03 Jul 2018 00:23:45 GMT
ENV GIT_DOWNLOAD_SHA256=668d16a799dd721ed126cc91bed49eb2c072ba1b25b50048280a4e2c5ed56e59
# Tue, 03 Jul 2018 00:25:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 		Write-Host 'Complete.';
# Tue, 03 Jul 2018 00:25:34 GMT
ENV GOPATH=C:\gopath
# Tue, 03 Jul 2018 00:26:38 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 03 Jul 2018 00:26:39 GMT
ENV GOLANG_VERSION=1.11beta1
# Tue, 03 Jul 2018 00:32:27 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1eeb874a919143f3e62b641ccd5ebbfd1b3d4f2184de1d6497f7b2b6df996960'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 03 Jul 2018 00:32:29 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8e9da9bbe3af2118a0b5eef7a3d649367557d0d3992ed0213c79857b23b4140e`  
		Last Modified: Wed, 13 Jun 2018 00:36:30 GMT  
		Size: 1.4 GB (1414319443 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:650685bf03844147638a02f1b62114e24cf12bf85feb92b6e2273d551a54c647`  
		Last Modified: Tue, 03 Jul 2018 01:20:32 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a91cb469c7e359d741522bed0e10c649670cfb3641af9c3cac4d93f2423df`  
		Last Modified: Tue, 03 Jul 2018 01:20:27 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8620bdbf56ed7bd0c8b1631a4af59f14ac8b13b1a35a419effed5ec5833d81`  
		Last Modified: Tue, 03 Jul 2018 01:20:27 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f22b0f509ad85923738743a615bdea603c33c88950a9a98f767cab9388a3e8`  
		Last Modified: Tue, 03 Jul 2018 01:20:24 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df5f4eb693cb8a03451955a74621e10cccf27271739ccb347b2aba30e4ae776`  
		Last Modified: Tue, 03 Jul 2018 01:20:23 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b05ca26dfe593b9d3d71f88f926f989dde3098abf546ea352705a8d592ec535`  
		Last Modified: Tue, 03 Jul 2018 01:20:36 GMT  
		Size: 29.4 MB (29418486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226aa27d434e3715787b7423db91aa0b17f5935a306412dc1e9bdd0024426551`  
		Last Modified: Tue, 03 Jul 2018 01:20:20 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93a88f4c490a44ae518df594618c85ae0740b85bd552f597b1db11b9c80f3f3`  
		Last Modified: Tue, 03 Jul 2018 01:20:24 GMT  
		Size: 5.0 MB (4957116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd70231903598ec134898bdc51f4ce57174266a27c161d33ac11419c09219eb`  
		Last Modified: Tue, 03 Jul 2018 01:20:21 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbff30d3fa34e99fccc7fe6285c80073f46439c076fc69f9343a120efac001d4`  
		Last Modified: Tue, 03 Jul 2018 01:21:53 GMT  
		Size: 181.8 MB (181759695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac53ba20e8119f58b384b42fe6873b50dfdc468e47bda0c267c6a365c0df366`  
		Last Modified: Tue, 03 Jul 2018 01:20:20 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - windows version 10.0.16299.492; amd64

```console
$ docker pull golang@sha256:4b1d3787cb75ad4937b27d1b87bfe8b7d6d1e6576119a5a08aec66b47273842c
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3308699990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f0f7f9495eca9f828f49743a33ef0832acc7b62651b26ffe2d10324e4e714fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Mon, 11 Jun 2018 20:38:48 GMT
RUN Install update 10.0.16299.492
# Tue, 03 Jul 2018 00:32:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 03 Jul 2018 00:32:42 GMT
ENV GIT_VERSION=2.11.1
# Tue, 03 Jul 2018 00:32:43 GMT
ENV GIT_TAG=v2.11.1.windows.1
# Tue, 03 Jul 2018 00:32:44 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.11.1.windows.1/MinGit-2.11.1-64-bit.zip
# Tue, 03 Jul 2018 00:32:45 GMT
ENV GIT_DOWNLOAD_SHA256=668d16a799dd721ed126cc91bed49eb2c072ba1b25b50048280a4e2c5ed56e59
# Tue, 03 Jul 2018 00:34:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 		Write-Host 'Complete.';
# Tue, 03 Jul 2018 00:34:27 GMT
ENV GOPATH=C:\gopath
# Tue, 03 Jul 2018 00:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 03 Jul 2018 00:35:14 GMT
ENV GOLANG_VERSION=1.11beta1
# Tue, 03 Jul 2018 00:41:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1eeb874a919143f3e62b641ccd5ebbfd1b3d4f2184de1d6497f7b2b6df996960'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 03 Jul 2018 00:41:06 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b9c63e313c8b374d5767c602fd6f2b947a3f1df9a8f8c5fcecb2fa6b1cfa968`  
		Last Modified: Wed, 13 Jun 2018 01:11:53 GMT  
		Size: 823.6 MB (823576248 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3989f186f0fc841be4fd06c5f4d58afe814bf92ffa0940def6b8d21ea38c223f`  
		Last Modified: Tue, 03 Jul 2018 01:22:20 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be9b417a88820877751cabcf39e3146ad1ab906b2ea03a402fc2c8c80ac63cd`  
		Last Modified: Tue, 03 Jul 2018 01:22:19 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d322a253d4e6b1042c99e15204b98272914fc6a977cc8e43f561d36c409974`  
		Last Modified: Tue, 03 Jul 2018 01:22:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d26f8ebc8846286e8ec3c1ad0caef4f3efa36d801c44f4c85fe1974e4985f36`  
		Last Modified: Tue, 03 Jul 2018 01:22:16 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbdea9ee4b8bfb010cf3410f4bbb85103ff94d9ad96e1ebe5dd863be875fcbd`  
		Last Modified: Tue, 03 Jul 2018 01:22:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37b383766e6fa050f0826e2e271967cb531e76bf089bf4e2020960418b5b9eb`  
		Last Modified: Tue, 03 Jul 2018 01:22:28 GMT  
		Size: 29.1 MB (29120783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff7982cd7f2036cd30289e69b2b7962f4b78c90b20cf8fd8e5bae1dce935fed`  
		Last Modified: Tue, 03 Jul 2018 01:22:13 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6cab04e28059c3e43f99bb05d15d5f14e0cb87711a9d919f9ae954a8d275bd`  
		Last Modified: Tue, 03 Jul 2018 01:22:14 GMT  
		Size: 4.7 MB (4681808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6644ea707dec024576ed8e38597235be44c073b2ff7919a6d30e043fee7a76a3`  
		Last Modified: Tue, 03 Jul 2018 01:22:13 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a1244190b0c56890a07c01d745c4544773dd3723b91a5044211201610cece6`  
		Last Modified: Tue, 03 Jul 2018 01:23:45 GMT  
		Size: 177.0 MB (177010890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47907aba4a4e458591b5f1a69b7d0401268ec667572e11cceeea180b737cbcbb`  
		Last Modified: Tue, 03 Jul 2018 01:22:13 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip