## `ruby:rc-alpine`

```console
$ docker pull ruby@sha256:33bbc7d8cfc98c821148273a16edb6a890117ce1cfdc46bd6d2fadb42428a5f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ruby:rc-alpine` - linux; amd64

```console
$ docker pull ruby@sha256:93fa4969a2ade38492a44cf742e0fbbbe70896e2c6af9f95a122464477113bb3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23872774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8210a0c92dc8eddbd99a3e9933594a222d5da56bfe60a1f6225116f4682b0ef`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 11 Sep 2018 22:19:50 GMT
ADD file:25c10b1d1b41d46a1827ad0b0d2389c24df6d31430005ff4e9a2d84ea23ebd42 in / 
# Tue, 11 Sep 2018 22:19:50 GMT
CMD ["/bin/sh"]
# Sat, 15 Sep 2018 01:53:44 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 15 Sep 2018 01:53:45 GMT
ENV RUBY_MAJOR=2.6-rc
# Sat, 15 Sep 2018 01:53:45 GMT
ENV RUBY_VERSION=2.6.0-preview2
# Sat, 15 Sep 2018 01:53:45 GMT
ENV RUBY_DOWNLOAD_SHA256=00ddfb5e33dee24469dd0b203597f7ecee66522ebb496f620f5815372ea2d3ec
# Sat, 15 Sep 2018 01:53:45 GMT
ENV RUBYGEMS_VERSION=2.7.7
# Fri, 05 Oct 2018 21:31:56 GMT
ENV BUNDLER_VERSION=1.16.6
# Fri, 05 Oct 2018 21:35:01 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch' 	&& echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum -c - 	&& patch -p1 -i thread-stack-fix.patch 	&& rm thread-stack-fix.patch 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del --no-network .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force 	&& rm -r /root/.gem/
# Fri, 05 Oct 2018 21:35:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 05 Oct 2018 21:35:02 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 05 Oct 2018 21:35:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Oct 2018 21:35:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 05 Oct 2018 21:35:03 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:4fe2ade4980c2dda4fc95858ebb981489baec8c1e4bd282ab1c3560be8ff9bde`  
		Last Modified: Tue, 11 Sep 2018 22:21:23 GMT  
		Size: 2.2 MB (2206931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5149ad82623a4772956c45af25639934cb0bf1f670750f37145db638b0c35b`  
		Last Modified: Sat, 15 Sep 2018 02:26:54 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56294417b3c504130fd02cdb79d508178624ba5d5a83102f2dbe0f6b8784d318`  
		Last Modified: Fri, 05 Oct 2018 22:27:52 GMT  
		Size: 21.7 MB (21665504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3ecd2fbe522c4284b81e409a737dd4f5ee37297244bdd4c14904343269935e`  
		Last Modified: Fri, 05 Oct 2018 22:27:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:rc-alpine` - linux; arm variant v6

```console
$ docker pull ruby@sha256:5cd4c09a89a2322116dde2966feca2f541cde0b444b6428108093cd437d6ad81
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23193541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5e6b3f2bfa4feed79f9001b195d036173480c92a377ef0ca1c514f1481cdf3`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 12 Sep 2018 07:49:40 GMT
ADD file:9c713f2312a88f19529816851673353155f329a4b024d62b03f656b0ce32f2a6 in / 
# Wed, 12 Sep 2018 07:49:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 07:49:40 GMT
CMD ["/bin/sh"]
# Sat, 15 Sep 2018 09:13:08 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 15 Sep 2018 09:13:08 GMT
ENV RUBY_MAJOR=2.6-rc
# Sat, 15 Sep 2018 09:13:08 GMT
ENV RUBY_VERSION=2.6.0-preview2
# Sat, 15 Sep 2018 09:13:09 GMT
ENV RUBY_DOWNLOAD_SHA256=00ddfb5e33dee24469dd0b203597f7ecee66522ebb496f620f5815372ea2d3ec
# Sat, 15 Sep 2018 09:13:09 GMT
ENV RUBYGEMS_VERSION=2.7.7
# Sat, 06 Oct 2018 07:49:50 GMT
ENV BUNDLER_VERSION=1.16.6
# Sat, 06 Oct 2018 07:52:37 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch' 	&& echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum -c - 	&& patch -p1 -i thread-stack-fix.patch 	&& rm thread-stack-fix.patch 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del --no-network .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force 	&& rm -r /root/.gem/
# Sat, 06 Oct 2018 07:52:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 06 Oct 2018 07:52:42 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 06 Oct 2018 07:52:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 06 Oct 2018 07:52:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 06 Oct 2018 07:52:47 GMT
CMD ["irb"]
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
	-	`sha256:0088c676e10e2c3dbb18edd0d4b1a4173eb744e4c2729b71310665a30e656ec9`  
		Last Modified: Sat, 15 Sep 2018 09:41:58 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4053fb18910c8d31d5ce3c31760a78964a761bc54157621776a409d0a96fe7c9`  
		Last Modified: Sat, 06 Oct 2018 08:16:58 GMT  
		Size: 21.0 MB (21046514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8536cbe5eb784b25756a4b6a56bbd71e856d2fd7d689a1f773904b38a7530bb`  
		Last Modified: Sat, 06 Oct 2018 08:16:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:rc-alpine` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:a175e6d2e3f186011f6cf95af2ff30c66bfbf6f0bb9201b7882acd4d0964a658
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23507382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e502fb030c456ea2bd5bdd5420499542c38515d409f59693bf4e81049ada6a`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 12 Sep 2018 08:42:24 GMT
ADD file:a4b53e2a2e207c5107a76c16d91b99cb1ed4ecb90b363913798e663426137d45 in / 
# Wed, 12 Sep 2018 08:42:24 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 08:42:25 GMT
CMD ["/bin/sh"]
# Sat, 15 Sep 2018 13:29:50 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 15 Sep 2018 13:29:51 GMT
ENV RUBY_MAJOR=2.6-rc
# Sat, 15 Sep 2018 13:29:52 GMT
ENV RUBY_VERSION=2.6.0-preview2
# Sat, 15 Sep 2018 13:29:52 GMT
ENV RUBY_DOWNLOAD_SHA256=00ddfb5e33dee24469dd0b203597f7ecee66522ebb496f620f5815372ea2d3ec
# Sat, 15 Sep 2018 13:29:53 GMT
ENV RUBYGEMS_VERSION=2.7.7
# Sat, 06 Oct 2018 09:11:34 GMT
ENV BUNDLER_VERSION=1.16.6
# Sat, 06 Oct 2018 09:15:48 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch' 	&& echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum -c - 	&& patch -p1 -i thread-stack-fix.patch 	&& rm thread-stack-fix.patch 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del --no-network .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force 	&& rm -r /root/.gem/
# Sat, 06 Oct 2018 09:15:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 06 Oct 2018 09:15:50 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 06 Oct 2018 09:15:51 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 06 Oct 2018 09:15:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 06 Oct 2018 09:16:03 GMT
CMD ["irb"]
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
	-	`sha256:607f3b2c08321d1069a4b670c7a5f9fe254abf239476a06e84eb6a3962bbd843`  
		Last Modified: Sat, 15 Sep 2018 14:24:58 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8775f9d58de45f6107758512dc7eb262413b015811a55bd6fac91e3f5c630f22`  
		Last Modified: Sat, 06 Oct 2018 10:40:41 GMT  
		Size: 21.4 MB (21407105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611a73e519814635f7636f8c44bb46e105f790921ffacf28c8f89f3dd0e6cd7`  
		Last Modified: Sat, 06 Oct 2018 10:40:33 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:rc-alpine` - linux; 386

```console
$ docker pull ruby@sha256:a7eb3d2e6d1d096f2c722b51fb2a75c00667afcea67acd13e38500e117e6b5c3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23422607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9963f563f7d5f05202679ba7a5249fa5962e0dd8f5bf6d09398769945e6255`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 12 Sep 2018 10:38:54 GMT
ADD file:b789aca08d6985c0bf373a2ca5f2a263d45e3a789aa6bbcd1fe1d47133f985d2 in / 
# Wed, 12 Sep 2018 10:38:54 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 10:38:54 GMT
CMD ["/bin/sh"]
# Sat, 15 Sep 2018 16:58:36 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 15 Sep 2018 16:58:37 GMT
ENV RUBY_MAJOR=2.6-rc
# Sat, 15 Sep 2018 16:58:37 GMT
ENV RUBY_VERSION=2.6.0-preview2
# Sat, 15 Sep 2018 16:58:37 GMT
ENV RUBY_DOWNLOAD_SHA256=00ddfb5e33dee24469dd0b203597f7ecee66522ebb496f620f5815372ea2d3ec
# Sat, 15 Sep 2018 16:58:37 GMT
ENV RUBYGEMS_VERSION=2.7.7
# Sat, 06 Oct 2018 10:45:43 GMT
ENV BUNDLER_VERSION=1.16.6
# Sat, 06 Oct 2018 10:48:28 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch' 	&& echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum -c - 	&& patch -p1 -i thread-stack-fix.patch 	&& rm thread-stack-fix.patch 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del --no-network .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force 	&& rm -r /root/.gem/
# Sat, 06 Oct 2018 10:48:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 06 Oct 2018 10:48:28 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 06 Oct 2018 10:48:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 06 Oct 2018 10:48:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 06 Oct 2018 10:48:29 GMT
CMD ["irb"]
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
	-	`sha256:924206edc141fd398aae2a8d03461adec00a65c98b42bc139568901368051ee2`  
		Last Modified: Sat, 15 Sep 2018 17:22:29 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f1548a1a055b8cfaa333d75894e64395525884df8a6551d1a252300d0b9129`  
		Last Modified: Sat, 06 Oct 2018 11:46:42 GMT  
		Size: 21.2 MB (21150634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157593bc06ef3d9dd96f47e7beb4d91e06eb030f90b0c8c32e030697792bed13`  
		Last Modified: Sat, 06 Oct 2018 11:46:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:rc-alpine` - linux; ppc64le

```console
$ docker pull ruby@sha256:d597ad543f96ba7d3618056fe5aa608a63ba2676423c93b6dc6831d6eeae1238
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24070842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35538a603f0c559504daff983e886d2269090912958b4d7a67839b4cb37e34ca`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 12 Sep 2018 08:18:11 GMT
ADD file:0991fe2a00b8319ade0b97ea20b79708b45153da36419ca58378c8bece0f987c in / 
# Wed, 12 Sep 2018 08:18:13 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 08:18:14 GMT
CMD ["/bin/sh"]
# Sat, 15 Sep 2018 09:14:09 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 15 Sep 2018 09:14:11 GMT
ENV RUBY_MAJOR=2.6-rc
# Sat, 15 Sep 2018 09:14:14 GMT
ENV RUBY_VERSION=2.6.0-preview2
# Sat, 15 Sep 2018 09:14:15 GMT
ENV RUBY_DOWNLOAD_SHA256=00ddfb5e33dee24469dd0b203597f7ecee66522ebb496f620f5815372ea2d3ec
# Sat, 15 Sep 2018 09:14:16 GMT
ENV RUBYGEMS_VERSION=2.7.7
# Sat, 06 Oct 2018 08:50:04 GMT
ENV BUNDLER_VERSION=1.16.6
# Sat, 06 Oct 2018 08:52:27 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch' 	&& echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum -c - 	&& patch -p1 -i thread-stack-fix.patch 	&& rm thread-stack-fix.patch 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del --no-network .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force 	&& rm -r /root/.gem/
# Sat, 06 Oct 2018 08:52:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 06 Oct 2018 08:52:33 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 06 Oct 2018 08:52:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 06 Oct 2018 08:52:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 06 Oct 2018 08:52:41 GMT
CMD ["irb"]
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
	-	`sha256:a47f25fa5e78b093c101c34cdb3870ec0eb5b9c315e0ddda4068763eed4d2588`  
		Last Modified: Sat, 15 Sep 2018 10:03:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cb099beacde2368a59e26bb480d012f06b5d8ea97329477ce4f4420055ec9f`  
		Last Modified: Sat, 06 Oct 2018 10:16:49 GMT  
		Size: 21.9 MB (21875036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06006f881a56b5ab06a6c5fc20dc7f07d4d9a42059fafe1dcf9c9183eb060dac`  
		Last Modified: Sat, 06 Oct 2018 10:16:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:rc-alpine` - linux; s390x

```console
$ docker pull ruby@sha256:1311072f9a2cedabd23a5eefd487af4d732d7805be1be24c09a3c62c0d085392
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24313640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f820141d10ffc1af9640f752d62ae6e337a1bd860fb05ce79b324673b3f442cc`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 12 Sep 2018 11:42:25 GMT
ADD file:532f451315fcf5c4077ef91f62d9838cf5681b4a348af2d78f6edd825146612c in / 
# Wed, 12 Sep 2018 11:42:25 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 12 Sep 2018 11:42:25 GMT
CMD ["/bin/sh"]
# Sat, 15 Sep 2018 12:00:52 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 15 Sep 2018 12:00:52 GMT
ENV RUBY_MAJOR=2.6-rc
# Sat, 15 Sep 2018 12:00:52 GMT
ENV RUBY_VERSION=2.6.0-preview2
# Sat, 15 Sep 2018 12:00:52 GMT
ENV RUBY_DOWNLOAD_SHA256=00ddfb5e33dee24469dd0b203597f7ecee66522ebb496f620f5815372ea2d3ec
# Sat, 15 Sep 2018 12:00:52 GMT
ENV RUBYGEMS_VERSION=2.7.7
# Sat, 06 Oct 2018 11:58:39 GMT
ENV BUNDLER_VERSION=1.16.6
# Sat, 06 Oct 2018 12:01:25 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch' 	&& echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum -c - 	&& patch -p1 -i thread-stack-fix.patch 	&& rm thread-stack-fix.patch 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del --no-network .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force 	&& rm -r /root/.gem/
# Sat, 06 Oct 2018 12:01:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 06 Oct 2018 12:01:26 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 06 Oct 2018 12:01:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 06 Oct 2018 12:01:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 06 Oct 2018 12:01:28 GMT
CMD ["irb"]
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
	-	`sha256:f0c3c18867777f4e91cee8695e81e60b1e94bbce4598f873188718b72cbde319`  
		Last Modified: Sat, 15 Sep 2018 12:20:30 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfc71462d43629f841a7067bdf3a1fb1e273bbb73421e6f58b0169915f730af`  
		Last Modified: Sat, 06 Oct 2018 12:50:25 GMT  
		Size: 22.0 MB (22005377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8637695bbc6651ba311ebfb5b0d039f3e66e4475566016bde4eece8c0489126`  
		Last Modified: Sat, 06 Oct 2018 12:50:21 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
