<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haskell`

-	[`haskell:8`](#haskell8)
-	[`haskell:8.2`](#haskell82)
-	[`haskell:8.2.2`](#haskell822)
-	[`haskell:8.4`](#haskell84)
-	[`haskell:8.4.3`](#haskell843)
-	[`haskell:latest`](#haskelllatest)

## `haskell:8`

```console
$ docker pull haskell@sha256:a79bc276db7dfc764c8a3016f72e170ad5992d4aa3476468c2dd5ac9d91bf3a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:39083fd8b95f3c4d85dc4fc43be22b53404532da438627b013df56a95f81c34e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.1 MB (308118781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d7d0eab4c0bbc1ad706f6bc3a0e6bcccab5b2c062d2ddc8b1654489ca1c319c`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Sep 2018 21:21:24 GMT
ADD file:58d5c21fcabcf1eec94e8676a3b1e51c5fdc2db5c7b866a761f907fa30ede4d8 in / 
# Tue, 04 Sep 2018 21:21:24 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 23:51:02 GMT
ENV LANG=C.UTF-8
# Tue, 04 Sep 2018 23:52:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr curl git &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BA3CBA3FFE22B574 &&     apt-get update &&     apt-get install -y --no-install-recommends ghc-8.4.3 cabal-install-2.2         zlib1g-dev libtinfo-dev libsqlite3-dev g++ netbase xz-utils make &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     apt-get purge -y --auto-remove curl &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 04 Sep 2018 23:52:21 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/2.2/bin:/opt/ghc/8.4.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Sep 2018 23:52:21 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:05d1a5232b461a4b35424129580054caa878cd56f100e34282510bd4b4082e4d`  
		Last Modified: Tue, 04 Sep 2018 21:25:27 GMT  
		Size: 45.3 MB (45310060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bae1bf114c7fbc6828d64cd59ea2e7b5793364ee0614e467e53269dadfaefd`  
		Last Modified: Tue, 04 Sep 2018 23:55:13 GMT  
		Size: 262.8 MB (262808721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.2`

```console
$ docker pull haskell@sha256:9a72c0b1899dee95e7b0b635766d76a68f875c8853dabadca7aa75b493dec0af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.2` - linux; amd64

```console
$ docker pull haskell@sha256:20712595ef927c03bb47e9e649648a97ffdd4f0f856a39f5071744b31fb8c6cb
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.0 MB (286981635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7afb496fd11071541722ad71860aa03670b5678a2cc77e2f705aa6dfc3c1ef5`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Sep 2018 21:21:24 GMT
ADD file:58d5c21fcabcf1eec94e8676a3b1e51c5fdc2db5c7b866a761f907fa30ede4d8 in / 
# Tue, 04 Sep 2018 21:21:24 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 23:51:02 GMT
ENV LANG=C.UTF-8
# Tue, 04 Sep 2018 23:53:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr curl git &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BA3CBA3FFE22B574 &&     apt-get update &&     apt-get install -y --no-install-recommends ghc-8.2.2 cabal-install-2.2         zlib1g-dev libtinfo-dev libsqlite3-dev g++ netbase xz-utils make &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     apt-get purge -y --auto-remove curl &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 04 Sep 2018 23:53:41 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/2.2/bin:/opt/ghc/8.2.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Sep 2018 23:53:41 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:05d1a5232b461a4b35424129580054caa878cd56f100e34282510bd4b4082e4d`  
		Last Modified: Tue, 04 Sep 2018 21:25:27 GMT  
		Size: 45.3 MB (45310060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2822128f7bd2f18ad46295e992057a44b4bd72b32615275534103784a16bddd8`  
		Last Modified: Tue, 04 Sep 2018 23:56:39 GMT  
		Size: 241.7 MB (241671575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.2.2`

```console
$ docker pull haskell@sha256:9a72c0b1899dee95e7b0b635766d76a68f875c8853dabadca7aa75b493dec0af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.2.2` - linux; amd64

```console
$ docker pull haskell@sha256:20712595ef927c03bb47e9e649648a97ffdd4f0f856a39f5071744b31fb8c6cb
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.0 MB (286981635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7afb496fd11071541722ad71860aa03670b5678a2cc77e2f705aa6dfc3c1ef5`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Sep 2018 21:21:24 GMT
ADD file:58d5c21fcabcf1eec94e8676a3b1e51c5fdc2db5c7b866a761f907fa30ede4d8 in / 
# Tue, 04 Sep 2018 21:21:24 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 23:51:02 GMT
ENV LANG=C.UTF-8
# Tue, 04 Sep 2018 23:53:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr curl git &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BA3CBA3FFE22B574 &&     apt-get update &&     apt-get install -y --no-install-recommends ghc-8.2.2 cabal-install-2.2         zlib1g-dev libtinfo-dev libsqlite3-dev g++ netbase xz-utils make &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     apt-get purge -y --auto-remove curl &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 04 Sep 2018 23:53:41 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/2.2/bin:/opt/ghc/8.2.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Sep 2018 23:53:41 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:05d1a5232b461a4b35424129580054caa878cd56f100e34282510bd4b4082e4d`  
		Last Modified: Tue, 04 Sep 2018 21:25:27 GMT  
		Size: 45.3 MB (45310060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2822128f7bd2f18ad46295e992057a44b4bd72b32615275534103784a16bddd8`  
		Last Modified: Tue, 04 Sep 2018 23:56:39 GMT  
		Size: 241.7 MB (241671575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.4`

```console
$ docker pull haskell@sha256:a79bc276db7dfc764c8a3016f72e170ad5992d4aa3476468c2dd5ac9d91bf3a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.4` - linux; amd64

```console
$ docker pull haskell@sha256:39083fd8b95f3c4d85dc4fc43be22b53404532da438627b013df56a95f81c34e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.1 MB (308118781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d7d0eab4c0bbc1ad706f6bc3a0e6bcccab5b2c062d2ddc8b1654489ca1c319c`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Sep 2018 21:21:24 GMT
ADD file:58d5c21fcabcf1eec94e8676a3b1e51c5fdc2db5c7b866a761f907fa30ede4d8 in / 
# Tue, 04 Sep 2018 21:21:24 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 23:51:02 GMT
ENV LANG=C.UTF-8
# Tue, 04 Sep 2018 23:52:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr curl git &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BA3CBA3FFE22B574 &&     apt-get update &&     apt-get install -y --no-install-recommends ghc-8.4.3 cabal-install-2.2         zlib1g-dev libtinfo-dev libsqlite3-dev g++ netbase xz-utils make &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     apt-get purge -y --auto-remove curl &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 04 Sep 2018 23:52:21 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/2.2/bin:/opt/ghc/8.4.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Sep 2018 23:52:21 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:05d1a5232b461a4b35424129580054caa878cd56f100e34282510bd4b4082e4d`  
		Last Modified: Tue, 04 Sep 2018 21:25:27 GMT  
		Size: 45.3 MB (45310060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bae1bf114c7fbc6828d64cd59ea2e7b5793364ee0614e467e53269dadfaefd`  
		Last Modified: Tue, 04 Sep 2018 23:55:13 GMT  
		Size: 262.8 MB (262808721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.4.3`

```console
$ docker pull haskell@sha256:a79bc276db7dfc764c8a3016f72e170ad5992d4aa3476468c2dd5ac9d91bf3a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.4.3` - linux; amd64

```console
$ docker pull haskell@sha256:39083fd8b95f3c4d85dc4fc43be22b53404532da438627b013df56a95f81c34e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.1 MB (308118781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d7d0eab4c0bbc1ad706f6bc3a0e6bcccab5b2c062d2ddc8b1654489ca1c319c`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Sep 2018 21:21:24 GMT
ADD file:58d5c21fcabcf1eec94e8676a3b1e51c5fdc2db5c7b866a761f907fa30ede4d8 in / 
# Tue, 04 Sep 2018 21:21:24 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 23:51:02 GMT
ENV LANG=C.UTF-8
# Tue, 04 Sep 2018 23:52:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr curl git &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BA3CBA3FFE22B574 &&     apt-get update &&     apt-get install -y --no-install-recommends ghc-8.4.3 cabal-install-2.2         zlib1g-dev libtinfo-dev libsqlite3-dev g++ netbase xz-utils make &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     apt-get purge -y --auto-remove curl &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 04 Sep 2018 23:52:21 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/2.2/bin:/opt/ghc/8.4.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Sep 2018 23:52:21 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:05d1a5232b461a4b35424129580054caa878cd56f100e34282510bd4b4082e4d`  
		Last Modified: Tue, 04 Sep 2018 21:25:27 GMT  
		Size: 45.3 MB (45310060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bae1bf114c7fbc6828d64cd59ea2e7b5793364ee0614e467e53269dadfaefd`  
		Last Modified: Tue, 04 Sep 2018 23:55:13 GMT  
		Size: 262.8 MB (262808721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:a79bc276db7dfc764c8a3016f72e170ad5992d4aa3476468c2dd5ac9d91bf3a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:39083fd8b95f3c4d85dc4fc43be22b53404532da438627b013df56a95f81c34e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.1 MB (308118781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d7d0eab4c0bbc1ad706f6bc3a0e6bcccab5b2c062d2ddc8b1654489ca1c319c`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Sep 2018 21:21:24 GMT
ADD file:58d5c21fcabcf1eec94e8676a3b1e51c5fdc2db5c7b866a761f907fa30ede4d8 in / 
# Tue, 04 Sep 2018 21:21:24 GMT
CMD ["bash"]
# Tue, 04 Sep 2018 23:51:02 GMT
ENV LANG=C.UTF-8
# Tue, 04 Sep 2018 23:52:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr curl git &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BA3CBA3FFE22B574 &&     apt-get update &&     apt-get install -y --no-install-recommends ghc-8.4.3 cabal-install-2.2         zlib1g-dev libtinfo-dev libsqlite3-dev g++ netbase xz-utils make &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v1.7.1/stack-1.7.1-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     apt-get purge -y --auto-remove curl &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 04 Sep 2018 23:52:21 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/2.2/bin:/opt/ghc/8.4.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Sep 2018 23:52:21 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:05d1a5232b461a4b35424129580054caa878cd56f100e34282510bd4b4082e4d`  
		Last Modified: Tue, 04 Sep 2018 21:25:27 GMT  
		Size: 45.3 MB (45310060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bae1bf114c7fbc6828d64cd59ea2e7b5793364ee0614e467e53269dadfaefd`  
		Last Modified: Tue, 04 Sep 2018 23:55:13 GMT  
		Size: 262.8 MB (262808721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
