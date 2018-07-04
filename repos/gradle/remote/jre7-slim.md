## `gradle:jre7-slim`

```console
$ docker pull gradle@sha256:bc49fa382904160d4e32e31d95c45802d1df5cce8fce2556fc20c275561ddfd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386

### `gradle:jre7-slim` - linux; amd64

```console
$ docker pull gradle@sha256:246f6a6fa4ab15ba88277585c1cfe1081a1e8fa3b05361d783c02caaabb3ab03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.5 MB (180521587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:236588fdda067aa74ed6ab4169f6634c6122c096722971e256e2a1878462041e`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 26 Jun 2018 21:21:17 GMT
ADD file:8108708c9ab961c9562c2171f4f594291dbaac0dc81dcb7bcbaf134f251f459e in / 
# Tue, 26 Jun 2018 21:21:18 GMT
CMD ["bash"]
# Tue, 26 Jun 2018 23:33:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 26 Jun 2018 23:33:58 GMT
ENV LANG=C.UTF-8
# Tue, 26 Jun 2018 23:33:59 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 26 Jun 2018 23:33:59 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 26 Jun 2018 23:37:09 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Tue, 26 Jun 2018 23:37:09 GMT
ENV JAVA_VERSION=7u181
# Tue, 26 Jun 2018 23:37:09 GMT
ENV JAVA_DEBIAN_VERSION=7u181-2.6.14-1~deb8u1
# Tue, 26 Jun 2018 23:38:08 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Fri, 29 Jun 2018 22:26:09 GMT
CMD ["gradle"]
# Fri, 29 Jun 2018 22:26:09 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 29 Jun 2018 22:26:09 GMT
ENV GRADLE_VERSION=4.8.1
# Fri, 29 Jun 2018 22:26:42 GMT
RUN apt-get update && 	apt-get install -y --no-install-recommends 		unzip 		wget && 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Jun 2018 22:26:42 GMT
ARG GRADLE_DOWNLOAD_SHA256=af334d994b5e69e439ab55b5d2b7d086da5ea6763d78054f49f147b06370ed71
# Fri, 29 Jun 2018 22:26:47 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=af334d994b5e69e439ab55b5d2b7d086da5ea6763d78054f49f147b06370ed71
RUN set -o errexit -o nounset 	&& echo "Downloading Gradle" 	&& wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip" 		&& echo "Checking download hash" 	&& echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check - 		&& echo "Installing Gradle" 	&& unzip gradle.zip 	&& rm gradle.zip 	&& mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/" 	&& ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle 		&& echo "Adding gradle user and group" 	&& groupadd --system --gid 1000 gradle 	&& useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle 	&& mkdir /home/gradle/.gradle 	&& chown --recursive gradle:gradle /home/gradle 		&& echo "Symlinking root Gradle cache to gradle Gradle cache" 	&& ln -s /home/gradle/.gradle /root/.gradle
# Fri, 29 Jun 2018 22:26:48 GMT
USER [gradle]
# Fri, 29 Jun 2018 22:26:48 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 29 Jun 2018 22:26:48 GMT
WORKDIR /home/gradle
# Fri, 29 Jun 2018 22:26:50 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=af334d994b5e69e439ab55b5d2b7d086da5ea6763d78054f49f147b06370ed71
RUN set -o errexit -o nounset 	&& echo "Testing Gradle installation" 	&& gradle --version
```

-	Layers:
	-	`sha256:2caa28db99eb312c788669036f0bf3914f73f5a27a30f69d2a7443fce10eb882`  
		Last Modified: Tue, 26 Jun 2018 21:31:00 GMT  
		Size: 30.1 MB (30119838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b466fd40b39060e96cf1326c3764f3186bb062bb692cf9f130d477fdccf9aaf1`  
		Last Modified: Tue, 26 Jun 2018 23:57:03 GMT  
		Size: 463.7 KB (463741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d0ac1dcec173c9698e3586eb1889ea24d359fbd1f735863f5742072496ece6`  
		Last Modified: Tue, 26 Jun 2018 23:57:03 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a711da6835f07d1b38e4677dafe89be66bb2a1de6dc07f652c470b58a22152ed`  
		Last Modified: Tue, 26 Jun 2018 23:57:02 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ad9a40fa41c09e5a8700cdd5a91bd8f2b80a8036f57db7cc357c09b15a37a2`  
		Last Modified: Tue, 26 Jun 2018 23:59:08 GMT  
		Size: 61.7 MB (61701012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a7ca1b2423113bc560e54f1405cb30956b25156c79c0901365c30ca797f64`  
		Last Modified: Fri, 29 Jun 2018 22:36:29 GMT  
		Size: 12.4 MB (12360651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1df66363c6bc627bbbd3be3a79d9ce3edbb4295f3d4668d6b15ef6bb6f9c94`  
		Last Modified: Fri, 29 Jun 2018 22:36:39 GMT  
		Size: 75.9 MB (75875830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cebea1026f1dc9409e2ca8b1dc0fd6e43dfa35358541e827b0c25400e0acf0`  
		Last Modified: Fri, 29 Jun 2018 22:36:25 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre7-slim` - linux; 386

```console
$ docker pull gradle@sha256:29827f1c1ac8061f1fbf9913527bd37aa5c96b9a9abd588e47105aeddb35ec7e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192395627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccea807c251a1a9f09d125f3ad6fb8cf7bd523a62f5cde87dc1e501b0f8da782`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 27 Jun 2018 10:40:54 GMT
ADD file:cd5600a909bc1ec399c2dd64e2e0f8383e1029c2169b56e923349fff08a544a6 in / 
# Wed, 27 Jun 2018 10:40:55 GMT
CMD ["bash"]
# Wed, 27 Jun 2018 15:20:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jun 2018 15:20:03 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jun 2018 15:20:04 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 27 Jun 2018 15:20:05 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 27 Jun 2018 15:24:35 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Wed, 27 Jun 2018 15:24:35 GMT
ENV JAVA_VERSION=7u181
# Wed, 27 Jun 2018 15:24:36 GMT
ENV JAVA_DEBIAN_VERSION=7u181-2.6.14-1~deb8u1
# Wed, 27 Jun 2018 15:25:40 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Sat, 30 Jun 2018 10:44:11 GMT
CMD ["gradle"]
# Sat, 30 Jun 2018 10:44:11 GMT
ENV GRADLE_HOME=/opt/gradle
# Sat, 30 Jun 2018 10:44:11 GMT
ENV GRADLE_VERSION=4.8.1
# Sat, 30 Jun 2018 10:45:03 GMT
RUN apt-get update && 	apt-get install -y --no-install-recommends 		unzip 		wget && 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Jun 2018 10:45:04 GMT
ARG GRADLE_DOWNLOAD_SHA256=af334d994b5e69e439ab55b5d2b7d086da5ea6763d78054f49f147b06370ed71
# Sat, 30 Jun 2018 10:45:11 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=af334d994b5e69e439ab55b5d2b7d086da5ea6763d78054f49f147b06370ed71
RUN set -o errexit -o nounset 	&& echo "Downloading Gradle" 	&& wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip" 		&& echo "Checking download hash" 	&& echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check - 		&& echo "Installing Gradle" 	&& unzip gradle.zip 	&& rm gradle.zip 	&& mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/" 	&& ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle 		&& echo "Adding gradle user and group" 	&& groupadd --system --gid 1000 gradle 	&& useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle 	&& mkdir /home/gradle/.gradle 	&& chown --recursive gradle:gradle /home/gradle 		&& echo "Symlinking root Gradle cache to gradle Gradle cache" 	&& ln -s /home/gradle/.gradle /root/.gradle
# Sat, 30 Jun 2018 10:45:11 GMT
USER [gradle]
# Sat, 30 Jun 2018 10:45:11 GMT
VOLUME [/home/gradle/.gradle]
# Sat, 30 Jun 2018 10:45:11 GMT
WORKDIR /home/gradle
# Sat, 30 Jun 2018 10:45:14 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=af334d994b5e69e439ab55b5d2b7d086da5ea6763d78054f49f147b06370ed71
RUN set -o errexit -o nounset 	&& echo "Testing Gradle installation" 	&& gradle --version
```

-	Layers:
	-	`sha256:754ff349eaaa3314a657ce6b24abe2a9d237430ab3b66d7bd2b21113499d68ff`  
		Last Modified: Wed, 27 Jun 2018 10:54:13 GMT  
		Size: 30.3 MB (30269679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ecc1d61c7e4f9d92c42aa04c2c34df4a177075b5e03757cd2e9763398cdfeb`  
		Last Modified: Wed, 27 Jun 2018 15:34:05 GMT  
		Size: 466.3 KB (466301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c7e2782264f446bd837b4d66b7a139ab8eaa08fc2cd1b899df57f6d2209fcd`  
		Last Modified: Wed, 27 Jun 2018 15:34:04 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104cf7f40f84e06d4be0be1bb678f84432eedb0d07eaab0f1e54bccfd21e2e40`  
		Last Modified: Wed, 27 Jun 2018 15:34:04 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2821d86a80de17c528d3a7ff0248c524ab79da82e3af7c78d7f0d60305625f53`  
		Last Modified: Wed, 27 Jun 2018 15:37:22 GMT  
		Size: 73.3 MB (73288198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764fc25b24afb6e6ed1f789c21343f59a1586a231e0009f3085deb19d28bfdd`  
		Last Modified: Sat, 30 Jun 2018 10:49:34 GMT  
		Size: 12.5 MB (12495123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6461afce9bafbd2f0c064a961b90f513eb11ed79d975bb75c0fe588893fb8757`  
		Last Modified: Sat, 30 Jun 2018 10:49:41 GMT  
		Size: 75.9 MB (75875810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b1659f29464a1aecf1fa055511c85f743c42ef6b877f947787b0c957a4aaa9`  
		Last Modified: Sat, 30 Jun 2018 10:49:29 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip