<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rocket.chat`

-	[`rocket.chat:0`](#rocketchat0)
-	[`rocket.chat:0.70`](#rocketchat070)
-	[`rocket.chat:0.70.0`](#rocketchat0700)
-	[`rocket.chat:latest`](#rocketchatlatest)

## `rocket.chat:0`

```console
$ docker pull rocket.chat@sha256:233781e380555577e228688216af4ed3e3d900c0ceaf11b483efb95e3e963d61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:0` - linux; amd64

```console
$ docker pull rocket.chat@sha256:10323f439db22382b66e1376d0c31c49299c4a89a33a5c7756882f75797fb568
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227399724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184a3d858cf240ca0ace8be007407506adc3b14114f8ce427c666be3540c97ba`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 04 Sep 2018 21:20:04 GMT
ADD file:95eda454ef09779bfb9e8ba5744d0630fb6f59eb4c9174efa44804a756d15df3 in / 
# Tue, 04 Sep 2018 21:20:05 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 22:05:22 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 04 Sep 2018 22:05:23 GMT
RUN set -ex   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     56730D5401028683275BD23C23EFEFE93C4CFFFE     77984A986EBC2AA786BC0F66B01FBB92821C587A     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   ; do     gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Tue, 04 Sep 2018 22:05:23 GMT
ENV NODE_VERSION=8.11.4
# Tue, 04 Sep 2018 22:05:57 GMT
RUN buildDeps='xz-utils'     && ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -x     && apt-get update && apt-get install -y ca-certificates curl wget $buildDeps --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-get purge -y --auto-remove $buildDeps     && ln -s /usr/local/bin/node /usr/local/bin/nodejs
# Tue, 04 Sep 2018 22:05:58 GMT
ENV YARN_VERSION=1.6.0
# Tue, 04 Sep 2018 22:05:59 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz
# Tue, 04 Sep 2018 22:05:59 GMT
CMD ["node"]
# Wed, 05 Sep 2018 08:41:07 GMT
MAINTAINER buildmaster@rocket.chat
# Wed, 05 Sep 2018 08:41:08 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat.rocketchat /app/uploads
# Wed, 05 Sep 2018 08:41:08 GMT
VOLUME [/app/uploads]
# Wed, 05 Sep 2018 08:41:09 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Fri, 28 Sep 2018 18:26:54 GMT
ENV RC_VERSION=0.70.0
# Fri, 28 Sep 2018 18:26:54 GMT
WORKDIR /app
# Fri, 28 Sep 2018 18:27:51 GMT
RUN curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxvf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install
# Fri, 28 Sep 2018 18:27:54 GMT
USER [rocketchat]
# Fri, 28 Sep 2018 18:27:54 GMT
WORKDIR /app/bundle
# Fri, 28 Sep 2018 18:27:54 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Fri, 28 Sep 2018 18:27:54 GMT
EXPOSE 3000/tcp
# Fri, 28 Sep 2018 18:27:54 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:57936531d1eea907ae6c73ebe8f8b5dc71232f5a642db22e877a4f0fc6ff1516`  
		Last Modified: Tue, 04 Sep 2018 21:23:28 GMT  
		Size: 30.1 MB (30120564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b186cf19f9edbd5ee7b8f79fb5fa0a8a21c4f4119149d8f900b2f4f00b440815`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 4.4 KB (4400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadbf83122625b628be463f73c3c568462c43eaaeb284b83692ad754e5a126be`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 124.7 KB (124684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f59c2d471060372ce2f1ecadf6ebd0ef509c38ddbb741b103249574250fd725`  
		Last Modified: Tue, 04 Sep 2018 22:51:53 GMT  
		Size: 35.2 MB (35220388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ed7d64abe123ebfe43e3f2c3159f1bec4c06bbe96a66c961c0237f64470e89`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 1.1 MB (1073252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c605c1dcf6ea2ebe4f4a22935e4f9511178a8194dd6cbac794d155fdb4cf79`  
		Last Modified: Wed, 05 Sep 2018 08:42:27 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c374c906f2b065cb187f3dda90e3187e053a335d717ff3918db6a0ab01847e10`  
		Last Modified: Wed, 05 Sep 2018 08:42:27 GMT  
		Size: 138.1 KB (138136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcebf089bb2ec8afe6998793537600c083a0bf8d7ed9a6e64b666a8c60b8320`  
		Last Modified: Fri, 28 Sep 2018 18:29:46 GMT  
		Size: 160.7 MB (160716114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:0.70`

```console
$ docker pull rocket.chat@sha256:233781e380555577e228688216af4ed3e3d900c0ceaf11b483efb95e3e963d61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:0.70` - linux; amd64

```console
$ docker pull rocket.chat@sha256:10323f439db22382b66e1376d0c31c49299c4a89a33a5c7756882f75797fb568
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227399724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184a3d858cf240ca0ace8be007407506adc3b14114f8ce427c666be3540c97ba`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 04 Sep 2018 21:20:04 GMT
ADD file:95eda454ef09779bfb9e8ba5744d0630fb6f59eb4c9174efa44804a756d15df3 in / 
# Tue, 04 Sep 2018 21:20:05 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 22:05:22 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 04 Sep 2018 22:05:23 GMT
RUN set -ex   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     56730D5401028683275BD23C23EFEFE93C4CFFFE     77984A986EBC2AA786BC0F66B01FBB92821C587A     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   ; do     gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Tue, 04 Sep 2018 22:05:23 GMT
ENV NODE_VERSION=8.11.4
# Tue, 04 Sep 2018 22:05:57 GMT
RUN buildDeps='xz-utils'     && ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -x     && apt-get update && apt-get install -y ca-certificates curl wget $buildDeps --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-get purge -y --auto-remove $buildDeps     && ln -s /usr/local/bin/node /usr/local/bin/nodejs
# Tue, 04 Sep 2018 22:05:58 GMT
ENV YARN_VERSION=1.6.0
# Tue, 04 Sep 2018 22:05:59 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz
# Tue, 04 Sep 2018 22:05:59 GMT
CMD ["node"]
# Wed, 05 Sep 2018 08:41:07 GMT
MAINTAINER buildmaster@rocket.chat
# Wed, 05 Sep 2018 08:41:08 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat.rocketchat /app/uploads
# Wed, 05 Sep 2018 08:41:08 GMT
VOLUME [/app/uploads]
# Wed, 05 Sep 2018 08:41:09 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Fri, 28 Sep 2018 18:26:54 GMT
ENV RC_VERSION=0.70.0
# Fri, 28 Sep 2018 18:26:54 GMT
WORKDIR /app
# Fri, 28 Sep 2018 18:27:51 GMT
RUN curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxvf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install
# Fri, 28 Sep 2018 18:27:54 GMT
USER [rocketchat]
# Fri, 28 Sep 2018 18:27:54 GMT
WORKDIR /app/bundle
# Fri, 28 Sep 2018 18:27:54 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Fri, 28 Sep 2018 18:27:54 GMT
EXPOSE 3000/tcp
# Fri, 28 Sep 2018 18:27:54 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:57936531d1eea907ae6c73ebe8f8b5dc71232f5a642db22e877a4f0fc6ff1516`  
		Last Modified: Tue, 04 Sep 2018 21:23:28 GMT  
		Size: 30.1 MB (30120564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b186cf19f9edbd5ee7b8f79fb5fa0a8a21c4f4119149d8f900b2f4f00b440815`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 4.4 KB (4400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadbf83122625b628be463f73c3c568462c43eaaeb284b83692ad754e5a126be`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 124.7 KB (124684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f59c2d471060372ce2f1ecadf6ebd0ef509c38ddbb741b103249574250fd725`  
		Last Modified: Tue, 04 Sep 2018 22:51:53 GMT  
		Size: 35.2 MB (35220388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ed7d64abe123ebfe43e3f2c3159f1bec4c06bbe96a66c961c0237f64470e89`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 1.1 MB (1073252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c605c1dcf6ea2ebe4f4a22935e4f9511178a8194dd6cbac794d155fdb4cf79`  
		Last Modified: Wed, 05 Sep 2018 08:42:27 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c374c906f2b065cb187f3dda90e3187e053a335d717ff3918db6a0ab01847e10`  
		Last Modified: Wed, 05 Sep 2018 08:42:27 GMT  
		Size: 138.1 KB (138136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcebf089bb2ec8afe6998793537600c083a0bf8d7ed9a6e64b666a8c60b8320`  
		Last Modified: Fri, 28 Sep 2018 18:29:46 GMT  
		Size: 160.7 MB (160716114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:0.70.0`

```console
$ docker pull rocket.chat@sha256:233781e380555577e228688216af4ed3e3d900c0ceaf11b483efb95e3e963d61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:0.70.0` - linux; amd64

```console
$ docker pull rocket.chat@sha256:10323f439db22382b66e1376d0c31c49299c4a89a33a5c7756882f75797fb568
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227399724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184a3d858cf240ca0ace8be007407506adc3b14114f8ce427c666be3540c97ba`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 04 Sep 2018 21:20:04 GMT
ADD file:95eda454ef09779bfb9e8ba5744d0630fb6f59eb4c9174efa44804a756d15df3 in / 
# Tue, 04 Sep 2018 21:20:05 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 22:05:22 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 04 Sep 2018 22:05:23 GMT
RUN set -ex   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     56730D5401028683275BD23C23EFEFE93C4CFFFE     77984A986EBC2AA786BC0F66B01FBB92821C587A     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   ; do     gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Tue, 04 Sep 2018 22:05:23 GMT
ENV NODE_VERSION=8.11.4
# Tue, 04 Sep 2018 22:05:57 GMT
RUN buildDeps='xz-utils'     && ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -x     && apt-get update && apt-get install -y ca-certificates curl wget $buildDeps --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-get purge -y --auto-remove $buildDeps     && ln -s /usr/local/bin/node /usr/local/bin/nodejs
# Tue, 04 Sep 2018 22:05:58 GMT
ENV YARN_VERSION=1.6.0
# Tue, 04 Sep 2018 22:05:59 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz
# Tue, 04 Sep 2018 22:05:59 GMT
CMD ["node"]
# Wed, 05 Sep 2018 08:41:07 GMT
MAINTAINER buildmaster@rocket.chat
# Wed, 05 Sep 2018 08:41:08 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat.rocketchat /app/uploads
# Wed, 05 Sep 2018 08:41:08 GMT
VOLUME [/app/uploads]
# Wed, 05 Sep 2018 08:41:09 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Fri, 28 Sep 2018 18:26:54 GMT
ENV RC_VERSION=0.70.0
# Fri, 28 Sep 2018 18:26:54 GMT
WORKDIR /app
# Fri, 28 Sep 2018 18:27:51 GMT
RUN curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxvf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install
# Fri, 28 Sep 2018 18:27:54 GMT
USER [rocketchat]
# Fri, 28 Sep 2018 18:27:54 GMT
WORKDIR /app/bundle
# Fri, 28 Sep 2018 18:27:54 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Fri, 28 Sep 2018 18:27:54 GMT
EXPOSE 3000/tcp
# Fri, 28 Sep 2018 18:27:54 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:57936531d1eea907ae6c73ebe8f8b5dc71232f5a642db22e877a4f0fc6ff1516`  
		Last Modified: Tue, 04 Sep 2018 21:23:28 GMT  
		Size: 30.1 MB (30120564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b186cf19f9edbd5ee7b8f79fb5fa0a8a21c4f4119149d8f900b2f4f00b440815`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 4.4 KB (4400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadbf83122625b628be463f73c3c568462c43eaaeb284b83692ad754e5a126be`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 124.7 KB (124684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f59c2d471060372ce2f1ecadf6ebd0ef509c38ddbb741b103249574250fd725`  
		Last Modified: Tue, 04 Sep 2018 22:51:53 GMT  
		Size: 35.2 MB (35220388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ed7d64abe123ebfe43e3f2c3159f1bec4c06bbe96a66c961c0237f64470e89`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 1.1 MB (1073252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c605c1dcf6ea2ebe4f4a22935e4f9511178a8194dd6cbac794d155fdb4cf79`  
		Last Modified: Wed, 05 Sep 2018 08:42:27 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c374c906f2b065cb187f3dda90e3187e053a335d717ff3918db6a0ab01847e10`  
		Last Modified: Wed, 05 Sep 2018 08:42:27 GMT  
		Size: 138.1 KB (138136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcebf089bb2ec8afe6998793537600c083a0bf8d7ed9a6e64b666a8c60b8320`  
		Last Modified: Fri, 28 Sep 2018 18:29:46 GMT  
		Size: 160.7 MB (160716114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:233781e380555577e228688216af4ed3e3d900c0ceaf11b483efb95e3e963d61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:10323f439db22382b66e1376d0c31c49299c4a89a33a5c7756882f75797fb568
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227399724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184a3d858cf240ca0ace8be007407506adc3b14114f8ce427c666be3540c97ba`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 04 Sep 2018 21:20:04 GMT
ADD file:95eda454ef09779bfb9e8ba5744d0630fb6f59eb4c9174efa44804a756d15df3 in / 
# Tue, 04 Sep 2018 21:20:05 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 22:05:22 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 04 Sep 2018 22:05:23 GMT
RUN set -ex   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     56730D5401028683275BD23C23EFEFE93C4CFFFE     77984A986EBC2AA786BC0F66B01FBB92821C587A     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   ; do     gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Tue, 04 Sep 2018 22:05:23 GMT
ENV NODE_VERSION=8.11.4
# Tue, 04 Sep 2018 22:05:57 GMT
RUN buildDeps='xz-utils'     && ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -x     && apt-get update && apt-get install -y ca-certificates curl wget $buildDeps --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-get purge -y --auto-remove $buildDeps     && ln -s /usr/local/bin/node /usr/local/bin/nodejs
# Tue, 04 Sep 2018 22:05:58 GMT
ENV YARN_VERSION=1.6.0
# Tue, 04 Sep 2018 22:05:59 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz
# Tue, 04 Sep 2018 22:05:59 GMT
CMD ["node"]
# Wed, 05 Sep 2018 08:41:07 GMT
MAINTAINER buildmaster@rocket.chat
# Wed, 05 Sep 2018 08:41:08 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat.rocketchat /app/uploads
# Wed, 05 Sep 2018 08:41:08 GMT
VOLUME [/app/uploads]
# Wed, 05 Sep 2018 08:41:09 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Fri, 28 Sep 2018 18:26:54 GMT
ENV RC_VERSION=0.70.0
# Fri, 28 Sep 2018 18:26:54 GMT
WORKDIR /app
# Fri, 28 Sep 2018 18:27:51 GMT
RUN curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxvf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install
# Fri, 28 Sep 2018 18:27:54 GMT
USER [rocketchat]
# Fri, 28 Sep 2018 18:27:54 GMT
WORKDIR /app/bundle
# Fri, 28 Sep 2018 18:27:54 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Fri, 28 Sep 2018 18:27:54 GMT
EXPOSE 3000/tcp
# Fri, 28 Sep 2018 18:27:54 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:57936531d1eea907ae6c73ebe8f8b5dc71232f5a642db22e877a4f0fc6ff1516`  
		Last Modified: Tue, 04 Sep 2018 21:23:28 GMT  
		Size: 30.1 MB (30120564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b186cf19f9edbd5ee7b8f79fb5fa0a8a21c4f4119149d8f900b2f4f00b440815`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 4.4 KB (4400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadbf83122625b628be463f73c3c568462c43eaaeb284b83692ad754e5a126be`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 124.7 KB (124684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f59c2d471060372ce2f1ecadf6ebd0ef509c38ddbb741b103249574250fd725`  
		Last Modified: Tue, 04 Sep 2018 22:51:53 GMT  
		Size: 35.2 MB (35220388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ed7d64abe123ebfe43e3f2c3159f1bec4c06bbe96a66c961c0237f64470e89`  
		Last Modified: Tue, 04 Sep 2018 22:51:46 GMT  
		Size: 1.1 MB (1073252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c605c1dcf6ea2ebe4f4a22935e4f9511178a8194dd6cbac794d155fdb4cf79`  
		Last Modified: Wed, 05 Sep 2018 08:42:27 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c374c906f2b065cb187f3dda90e3187e053a335d717ff3918db6a0ab01847e10`  
		Last Modified: Wed, 05 Sep 2018 08:42:27 GMT  
		Size: 138.1 KB (138136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcebf089bb2ec8afe6998793537600c083a0bf8d7ed9a6e64b666a8c60b8320`  
		Last Modified: Fri, 28 Sep 2018 18:29:46 GMT  
		Size: 160.7 MB (160716114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
