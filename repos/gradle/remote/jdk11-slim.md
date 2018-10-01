## `gradle:jdk11-slim`

```console
$ docker pull gradle@sha256:65bc76c5a614961e5ae899117a2f5c9e442501fa8b21f382f15431d3c94a2eb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gradle:jdk11-slim` - linux; amd64

```console
$ docker pull gradle@sha256:167fb70338bf40069d8080df6cf01b384a4ece4dbd41e065d1a8d5fce99b16a2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.7 MB (401726958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b9f2f5344a8c9b2f6e539984253353d9f3ba29c72655de0d0069f845155cc5`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 04 Sep 2018 21:20:58 GMT
ADD file:a391d9232725a03d7b21f24be4d387c1d11f905c3ba448c0a3793745ca8cc6f3 in / 
# Tue, 04 Sep 2018 21:20:58 GMT
CMD ["bash"]
# Wed, 05 Sep 2018 01:15:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 01:15:51 GMT
ENV LANG=C.UTF-8
# Wed, 05 Sep 2018 01:15:52 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 05 Sep 2018 01:15:52 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 05 Sep 2018 01:15:52 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 28 Sep 2018 18:24:19 GMT
ENV JAVA_VERSION=11
# Fri, 28 Sep 2018 18:24:20 GMT
ENV JAVA_DEBIAN_VERSION=11~28-2
# Fri, 28 Sep 2018 18:25:01 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jdk-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Fri, 28 Sep 2018 18:25:05 GMT
CMD ["jshell"]
# Mon, 01 Oct 2018 20:23:10 GMT
CMD ["gradle"]
# Mon, 01 Oct 2018 20:23:11 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 01 Oct 2018 20:23:11 GMT
ENV GRADLE_VERSION=4.10.2
# Mon, 01 Oct 2018 20:23:16 GMT
RUN apt-get update && 	apt-get install -y --no-install-recommends 		unzip 		wget && 	rm -rf /var/lib/apt/lists/*
# Mon, 01 Oct 2018 20:23:19 GMT
ARG GRADLE_DOWNLOAD_SHA256=b49c6da1b2cb67a0caf6c7480630b51c70a11ca2016ff2f555eaeda863143a29
# Mon, 01 Oct 2018 20:23:22 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=b49c6da1b2cb67a0caf6c7480630b51c70a11ca2016ff2f555eaeda863143a29
RUN set -o errexit -o nounset 	&& echo "Downloading Gradle" 	&& wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip" 		&& echo "Checking download hash" 	&& echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check - 		&& echo "Installing Gradle" 	&& unzip gradle.zip 	&& rm gradle.zip 	&& mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/" 	&& ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle 		&& echo "Adding gradle user and group" 	&& groupadd --system --gid 1000 gradle 	&& useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle 	&& mkdir /home/gradle/.gradle 	&& chown --recursive gradle:gradle /home/gradle 		&& echo "Symlinking root Gradle cache to gradle Gradle cache" 	&& ln -s /home/gradle/.gradle /root/.gradle
# Mon, 01 Oct 2018 20:23:23 GMT
USER [gradle]
# Mon, 01 Oct 2018 20:23:23 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 01 Oct 2018 20:23:23 GMT
WORKDIR /home/gradle
# Mon, 01 Oct 2018 20:23:25 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=b49c6da1b2cb67a0caf6c7480630b51c70a11ca2016ff2f555eaeda863143a29
RUN set -o errexit -o nounset 	&& echo "Testing Gradle installation" 	&& gradle --version
```

-	Layers:
	-	`sha256:a7e1658cb0533dfcb5baa38a0ce3230fd3aea217be1a52d0b46f5521b305d608`  
		Last Modified: Tue, 04 Sep 2018 21:24:51 GMT  
		Size: 26.3 MB (26269506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826d7fab3f2f9f524ee8ab66d9bf80ff7ce89278ff495a4c665481d069832089`  
		Last Modified: Wed, 05 Sep 2018 01:32:25 GMT  
		Size: 460.8 KB (460788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7705f8b8f1de989ae8e63828bc91553d1aa32563ed57bd05b21828c0ef89920`  
		Last Modified: Wed, 05 Sep 2018 01:32:25 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346fb9b43905ab75618d23770204a6bc486e33867d3761b8a29e052036f87396`  
		Last Modified: Wed, 05 Sep 2018 01:32:24 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cfa073662b858a3db3c5d3d3edc0c964614822b28837eb916f7a17ad135785`  
		Last Modified: Fri, 28 Sep 2018 18:33:12 GMT  
		Size: 296.0 MB (295975808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b7b39d4d65d7fcdf0653b857c69c51d13587a1f2c620ac5a37d6f906219586`  
		Last Modified: Mon, 01 Oct 2018 20:25:16 GMT  
		Size: 614.3 KB (614338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cd750965a43626f4e66fca386fc28996bd5f7fbdfb12ce49a4373c62bb00f4`  
		Last Modified: Mon, 01 Oct 2018 20:25:23 GMT  
		Size: 78.4 MB (78406012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6622df60bdb657c70df0368a205330f2a1c5b93ddebe931a535288da20dc0ff3`  
		Last Modified: Mon, 01 Oct 2018 20:25:16 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip