## `gradle:jdk11`

```console
$ docker pull gradle@sha256:84c2cde409d2d4d95004b195ffe2b9ce4f65d34ed53f13e39c9091fea671774e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gradle:jdk11` - linux; amd64

```console
$ docker pull gradle@sha256:e5ad544e45d622b0e8779d5fefdd57771001c7c0e9e4fb7ec8e2dea2c632a1a4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.5 MB (588493347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a1b8d55d2e0f06778bbc901e2b11fc58a81025a084e78dfd71297b538062a6`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 04 Sep 2018 21:20:51 GMT
ADD file:6b6ece05e75fbdccfdd76433844e066f0ec636fb62e74326f1747ccde948c381 in / 
# Tue, 04 Sep 2018 21:20:52 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 22:31:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Sep 2018 22:31:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Sep 2018 22:31:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 01:14:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 01:14:23 GMT
ENV LANG=C.UTF-8
# Wed, 05 Sep 2018 01:14:23 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 05 Sep 2018 01:14:24 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 05 Sep 2018 01:14:24 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 28 Sep 2018 18:22:40 GMT
ENV JAVA_VERSION=11
# Fri, 28 Sep 2018 18:22:40 GMT
ENV JAVA_DEBIAN_VERSION=11~28-2
# Fri, 28 Sep 2018 18:23:58 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Fri, 28 Sep 2018 18:24:03 GMT
CMD ["jshell"]
# Mon, 01 Oct 2018 20:22:40 GMT
CMD ["gradle"]
# Mon, 01 Oct 2018 20:22:40 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 01 Oct 2018 20:22:40 GMT
ENV GRADLE_VERSION=4.10.2
# Mon, 01 Oct 2018 20:22:40 GMT
ARG GRADLE_DOWNLOAD_SHA256=b49c6da1b2cb67a0caf6c7480630b51c70a11ca2016ff2f555eaeda863143a29
# Mon, 01 Oct 2018 20:22:44 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=b49c6da1b2cb67a0caf6c7480630b51c70a11ca2016ff2f555eaeda863143a29
RUN set -o errexit -o nounset 	&& echo "Downloading Gradle" 	&& wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip" 		&& echo "Checking download hash" 	&& echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check - 		&& echo "Installing Gradle" 	&& unzip gradle.zip 	&& rm gradle.zip 	&& mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/" 	&& ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle 		&& echo "Adding gradle user and group" 	&& groupadd --system --gid 1000 gradle 	&& useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle 	&& mkdir /home/gradle/.gradle 	&& chown --recursive gradle:gradle /home/gradle 		&& echo "Symlinking root Gradle cache to gradle Gradle cache" 	&& ln -s /home/gradle/.gradle /root/.gradle
# Mon, 01 Oct 2018 20:22:48 GMT
USER [gradle]
# Mon, 01 Oct 2018 20:22:48 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 01 Oct 2018 20:22:48 GMT
WORKDIR /home/gradle
# Mon, 01 Oct 2018 20:22:51 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=b49c6da1b2cb67a0caf6c7480630b51c70a11ca2016ff2f555eaeda863143a29
RUN set -o errexit -o nounset 	&& echo "Testing Gradle installation" 	&& gradle --version
```

-	Layers:
	-	`sha256:5164339600396c4bdb97f111e5236c5fc64911bbd2bfe6d2343ce45fe79ea7d8`  
		Last Modified: Tue, 04 Sep 2018 21:24:41 GMT  
		Size: 49.1 MB (49071704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083ed1d8baf85dbda1151434e9afe28ad5efa36397cda6ff66cc5e7a888d2a4f`  
		Last Modified: Tue, 04 Sep 2018 22:51:37 GMT  
		Size: 7.4 MB (7350084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973ddf6ced7131822a05e3dd20803610fd06a8c695d3d814713f6ece58d616fd`  
		Last Modified: Tue, 04 Sep 2018 22:51:38 GMT  
		Size: 9.3 MB (9303992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb8320d7db45f4fea60cc567f2cf18032e0996273d8e63d6af5953f756d185`  
		Last Modified: Tue, 04 Sep 2018 22:51:55 GMT  
		Size: 51.4 MB (51443158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affad348605132419a057b8d81c7261439d651c1b2211d826c6bcc86ebb42bfe`  
		Last Modified: Wed, 05 Sep 2018 01:31:32 GMT  
		Size: 900.7 KB (900730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9702fa0409b03c3a115803227ac769d6850b2da7027a11757fc2241e47e130ce`  
		Last Modified: Wed, 05 Sep 2018 01:31:19 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd219431247b808000b0314fd0f997b7edba52854d82433060282024e3d86889`  
		Last Modified: Wed, 05 Sep 2018 01:31:20 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840183798047cf2309bb875bee6368097b9a0e26642116a5a1227a110823e525`  
		Last Modified: Fri, 28 Sep 2018 18:32:17 GMT  
		Size: 392.0 MB (392017269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4ed66537493da38bd4ca74985cb43d82bef2c626a83e062c6e228e25bc2bed`  
		Last Modified: Mon, 01 Oct 2018 20:24:39 GMT  
		Size: 78.4 MB (78405904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f769e99e7180484be0c13a2b4684bf3ea481a56cdcfb68e5c3d675e9ea3309b`  
		Last Modified: Mon, 01 Oct 2018 20:24:33 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip