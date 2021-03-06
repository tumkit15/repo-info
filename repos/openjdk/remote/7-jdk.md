## `openjdk:7-jdk`

```console
$ docker pull openjdk@sha256:27ca02ba3081b3eb9cf509ff1c9757257b4eb0d138bcdfa6f7c5a5f571bab1d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `openjdk:7-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:3229b39dd121d77539413ede533e5f7a779377bebb98fe8ad822ca49573a9443
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.7 MB (213729252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd6110589d1bab795c10081dbfde3889f9cdb085afe85fdcf985a6e3e7d06542`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Sep 2018 21:19:53 GMT
ADD file:8d73a09e59fe50289a6d0c019302aefe2e00ac6411e82404389c0c83f50cf08a in / 
# Tue, 04 Sep 2018 21:19:54 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 22:27:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Sep 2018 22:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Sep 2018 22:28:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 01:25:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 01:25:02 GMT
ENV LANG=C.UTF-8
# Wed, 05 Sep 2018 01:25:03 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 05 Sep 2018 01:25:04 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 05 Sep 2018 01:25:04 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 05 Sep 2018 01:25:04 GMT
ENV JAVA_VERSION=7u181
# Wed, 05 Sep 2018 01:25:04 GMT
ENV JAVA_DEBIAN_VERSION=7u181-2.6.14-1~deb8u1
# Wed, 05 Sep 2018 01:26:07 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:f189db1b88b3cab5fd17f74fee412610fe40d4b077e7882c1a50a8b6f4f0cea3`  
		Last Modified: Tue, 04 Sep 2018 21:23:11 GMT  
		Size: 54.3 MB (54252211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d06cf2f1b5e36347bb239d7ef7eb098e228d06a0a937e70798eb0dda459c61e`  
		Last Modified: Tue, 04 Sep 2018 22:50:42 GMT  
		Size: 17.5 MB (17538668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687ebdda822cb0f4af055462f887a7f76bc3f36d55161596fe93e45356dd45f0`  
		Last Modified: Tue, 04 Sep 2018 22:50:58 GMT  
		Size: 43.3 MB (43297955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4ab2fb905ca6c22240450bfe894880be6002348f782440c8401c755ca1dad5`  
		Last Modified: Wed, 05 Sep 2018 01:43:08 GMT  
		Size: 828.2 KB (828223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b6dc8bf2f2acb5e7855476df3eaa2d0755ef4721a283f6106ec1f953201fb4`  
		Last Modified: Wed, 05 Sep 2018 01:43:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b86af34285b6f5443cbf0bf7dd43c731f248e52d5d48ceb8d1b1884fa25370`  
		Last Modified: Wed, 05 Sep 2018 01:43:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab529fffea4c8d2178a260255e8887276b57461e8b6efeaf5472b72e8a5568`  
		Last Modified: Wed, 05 Sep 2018 01:43:28 GMT  
		Size: 97.8 MB (97811817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:7-jdk` - linux; arm variant v5

```console
$ docker pull openjdk@sha256:e60dfff38bdbf031d2f3d13b23ef5d935a9233a6001a74a8b86583a2f62f89e6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196380935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b83fadeb1666b7e3e3a8b20fed15554aa4020493c73d3b1a25cc3c2b291f923`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Sep 2018 08:50:01 GMT
ADD file:367230829937e3f959936d2c250983c5c63d8aff2e1987a1512c68d6b05ec2d9 in / 
# Wed, 05 Sep 2018 08:50:03 GMT
CMD ["bash"]
# Wed, 05 Sep 2018 09:51:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 09:51:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Sep 2018 09:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 14:29:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 14:29:05 GMT
ENV LANG=C.UTF-8
# Wed, 05 Sep 2018 14:29:06 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 05 Sep 2018 14:29:07 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 05 Sep 2018 14:29:07 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 05 Sep 2018 14:29:07 GMT
ENV JAVA_VERSION=7u181
# Wed, 05 Sep 2018 14:29:08 GMT
ENV JAVA_DEBIAN_VERSION=7u181-2.6.14-1~deb8u1
# Wed, 05 Sep 2018 14:30:25 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:e01fe8429ccebc46a010376112e864ce611e175d1f38e60e721840613bc3bc2a`  
		Last Modified: Wed, 05 Sep 2018 08:59:16 GMT  
		Size: 52.4 MB (52447943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6945911bf8713186fd7ee2c21f4ef1138adb8b200242ca929e7caab6978ff3a`  
		Last Modified: Wed, 05 Sep 2018 10:08:21 GMT  
		Size: 17.0 MB (17029456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a401183513e38faaa6c251a53174b409b087aeb9a040849500580106285c318`  
		Last Modified: Wed, 05 Sep 2018 10:08:50 GMT  
		Size: 41.1 MB (41141852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa51c9e15e98d67294aa44c71558aa6a991e2657d211dec1ceaeea4a2759bc`  
		Last Modified: Wed, 05 Sep 2018 14:42:41 GMT  
		Size: 821.4 KB (821427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6789df0668fab9d80b1f34a305d3e7771d9acde6ee87d4a26564b4d7350765`  
		Last Modified: Wed, 05 Sep 2018 14:42:41 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a813a2aea73adb5f787457f9e969aa8f0eff4c0ba63387d094b8f9b85ecb8fc6`  
		Last Modified: Wed, 05 Sep 2018 14:42:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc52689182f329952d12a68266de621ab31b719509438df3face8d5ee2852d2f`  
		Last Modified: Wed, 05 Sep 2018 14:42:59 GMT  
		Size: 84.9 MB (84939879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:7-jdk` - linux; arm variant v7

```console
$ docker pull openjdk@sha256:551ce9b8992d3374f4b46a52d392d6826c5a5cfb455840b0e4defc47aac07bf1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191052875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32a0b523b1eb1dca37f9539c605e7b954606b450c24474fecbca364846613404`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Sep 2018 11:59:11 GMT
ADD file:807e1499dd3578811c9df2630d381e29d52684675650039494a60eecfbbe9027 in / 
# Wed, 05 Sep 2018 11:59:12 GMT
CMD ["bash"]
# Wed, 05 Sep 2018 12:37:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 12:37:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Sep 2018 12:38:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 13:25:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 13:25:45 GMT
ENV LANG=C.UTF-8
# Wed, 05 Sep 2018 13:25:47 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 05 Sep 2018 13:25:48 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 05 Sep 2018 13:25:48 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 05 Sep 2018 13:25:48 GMT
ENV JAVA_VERSION=7u181
# Wed, 05 Sep 2018 13:25:48 GMT
ENV JAVA_DEBIAN_VERSION=7u181-2.6.14-1~deb8u1
# Wed, 05 Sep 2018 13:27:20 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:16b1b4bf69814b0a3f82bfd8b5c3117909ae89accabd8bee13a723080db56a75`  
		Last Modified: Wed, 05 Sep 2018 12:08:24 GMT  
		Size: 50.2 MB (50188388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002878cce7e14ca1293cd555eec033a6494913ae05e9b1b6a76701bb86dae153`  
		Last Modified: Wed, 05 Sep 2018 12:53:36 GMT  
		Size: 16.7 MB (16712872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a262dbf1b2c7fd841963ee65f24c265c5385068a36df528802e7ea0303aa0f`  
		Last Modified: Wed, 05 Sep 2018 12:54:08 GMT  
		Size: 39.8 MB (39764418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4490fe328aab7506ca28078302d84d7b34e2393d2ad8dfa97343b23a5668e2`  
		Last Modified: Wed, 05 Sep 2018 13:43:39 GMT  
		Size: 795.4 KB (795357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e863981e9ebc7e87ab350d5509fefb1248b77da0756591c2786ef65e7f55e5`  
		Last Modified: Wed, 05 Sep 2018 13:43:39 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74acde96147ace7f28c52e52829e6c5205928f264d98490dfd0673b30e6e8f0`  
		Last Modified: Wed, 05 Sep 2018 13:43:39 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0468380806091df36fb4ebc4ce32aad2a10a10a8c0463e29db054c7d93714bfd`  
		Last Modified: Wed, 05 Sep 2018 13:43:54 GMT  
		Size: 83.6 MB (83591461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:7-jdk` - linux; 386

```console
$ docker pull openjdk@sha256:24baf8acbbaab2e631a28eece6741b3bc5c657d33ed8b9f035e4414e76d6db59
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226639428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59907d42160c094fa5da7253cf7982a0334aaccdb35417e0facc045143a91735`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Sep 2018 10:39:51 GMT
ADD file:66e0b8b746f2f743e827a1adbb0d978b38dc00dab94077aa275e852073ea6beb in / 
# Wed, 05 Sep 2018 10:39:52 GMT
CMD ["bash"]
# Wed, 05 Sep 2018 11:28:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 11:28:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Sep 2018 11:30:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 13:03:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 13:03:48 GMT
ENV LANG=C.UTF-8
# Wed, 05 Sep 2018 13:03:49 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 05 Sep 2018 13:03:49 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 05 Sep 2018 13:03:50 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 05 Sep 2018 13:03:50 GMT
ENV JAVA_VERSION=7u181
# Wed, 05 Sep 2018 13:03:50 GMT
ENV JAVA_DEBIAN_VERSION=7u181-2.6.14-1~deb8u1
# Wed, 05 Sep 2018 13:05:47 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:8c6f9fc63ec81982d7b33596e2017e55287bdd085fd1c53fc5b439f51306efa5`  
		Last Modified: Wed, 05 Sep 2018 10:47:54 GMT  
		Size: 54.5 MB (54484051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912168c1f05e29e4f46f4cbc0e1aa3825348c0e9a19508d7658722848ddda877`  
		Last Modified: Wed, 05 Sep 2018 12:03:41 GMT  
		Size: 19.8 MB (19835822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e9187aeb009b949c7ae34ecf63d21f9c811f6f6bc2295738d4682eaba1f20e`  
		Last Modified: Wed, 05 Sep 2018 12:04:20 GMT  
		Size: 43.9 MB (43948373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339137fcf9b83c3b3f6a7b0d2e220dd7bfe5cb479bb0d0846563ffea90b92ff4`  
		Last Modified: Wed, 05 Sep 2018 13:28:53 GMT  
		Size: 831.3 KB (831257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b3172727a2bd95b368cced4daf7b768478c5bdc01788418ca68bfe36ab373a`  
		Last Modified: Wed, 05 Sep 2018 13:28:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3c2011ba703dfd9530a5d4fd4485e4b745a7fc111dfdfb41c5391f68cf396a`  
		Last Modified: Wed, 05 Sep 2018 13:28:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a12141ad64a4e238e63236835ef499d052036b48bb5d7a86d1c9669d07ac11d`  
		Last Modified: Wed, 05 Sep 2018 13:29:29 GMT  
		Size: 107.5 MB (107539547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
