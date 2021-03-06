## `redmine:3-passenger`

```console
$ docker pull redmine@sha256:83d10668b9b2b9cb3fcdfa4a2568a55af2104f5f27206fe558feeb3a39b1535d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:3-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:89f2dd301ad2127889bd52cb592a19e1af6d30336f0a6cc4c96eab988c5fbad4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.5 MB (316460744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc9c6d5d6086c7a9706c6aade0da2ab13c908d74c1212e790f5dda4d1cf780d9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 04 Sep 2018 21:21:24 GMT
ADD file:58d5c21fcabcf1eec94e8676a3b1e51c5fdc2db5c7b866a761f907fa30ede4d8 in / 
# Tue, 04 Sep 2018 21:21:24 GMT
CMD ["bash"]
# Wed, 05 Sep 2018 05:34:49 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgdbm3 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Sep 2018 05:34:49 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 05 Sep 2018 06:00:33 GMT
ENV RUBY_MAJOR=2.4
# Wed, 05 Sep 2018 06:00:33 GMT
ENV RUBY_VERSION=2.4.4
# Wed, 05 Sep 2018 06:00:34 GMT
ENV RUBY_DOWNLOAD_SHA256=1d0034071d675193ca769f64c91827e5f54cb3a7962316a41d5217c7bc6949f0
# Wed, 05 Sep 2018 06:00:34 GMT
ENV RUBYGEMS_VERSION=2.7.7
# Fri, 05 Oct 2018 21:50:10 GMT
ENV BUNDLER_VERSION=1.16.6
# Fri, 05 Oct 2018 21:53:47 GMT
RUN set -ex 		&& buildDeps=' 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& dpkg-query --show --showformat '${package}\n' 		| grep -P '^libreadline\d+$' 		| xargs apt-mark manual 	&& apt-get purge -y --auto-remove $buildDeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force 	&& rm -r /root/.gem/
# Fri, 05 Oct 2018 21:53:47 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 05 Oct 2018 21:53:47 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 05 Oct 2018 21:53:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Oct 2018 21:53:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 05 Oct 2018 21:53:48 GMT
CMD ["irb"]
# Fri, 05 Oct 2018 22:54:28 GMT
RUN groupadd -r redmine && useradd -r -g redmine redmine
# Fri, 05 Oct 2018 22:54:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		imagemagick 		mercurial 		openssh-client 		subversion 	&& rm -rf /var/lib/apt/lists/*
# Fri, 05 Oct 2018 22:55:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.10'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 05 Oct 2018 22:55:09 GMT
ENV RAILS_ENV=production
# Fri, 05 Oct 2018 22:55:09 GMT
WORKDIR /usr/src/redmine
# Fri, 05 Oct 2018 22:55:10 GMT
ENV REDMINE_VERSION=3.4.6
# Fri, 05 Oct 2018 22:55:10 GMT
ENV REDMINE_DOWNLOAD_MD5=5f4993446ecf25782f469763c0d32ea1
# Fri, 05 Oct 2018 22:55:13 GMT
RUN wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz" 	&& echo "$REDMINE_DOWNLOAD_MD5 redmine.tar.gz" | md5sum -c - 	&& tar -xvf redmine.tar.gz --strip-components=1 	&& rm redmine.tar.gz files/delete.me log/delete.me 	&& mkdir -p tmp/pdf public/plugin_assets 	&& chown -R redmine:redmine ./
# Fri, 05 Oct 2018 22:58:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libmagickcore-dev 		libmagickwand-dev 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 				libssl1.0-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O freetds.tar.bz2 'http://www.freetds.org/files/stable/freetds-1.00.91.tar.bz2'; 	echo '8d71f9f29be0fe0637e443dd3807b3fd *freetds.tar.bz2' | md5sum -c -; 	mkdir freetds; 	tar -xf freetds.tar.bz2 -C freetds --strip-components=1; 	rm freetds.tar.bz2; 	( cd freetds && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" && ./configure --build="$gnuArch" --enable-silent-rules && make -j "$(nproc)" && make -C src install && make -C include install ); 	rm -rf freetds; 	bundle config build.tiny_tds --enable-system-freetds; 		bundle install --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		bundle install --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 05 Oct 2018 22:58:13 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 05 Oct 2018 22:58:13 GMT
COPY file:fc148119ccb9e484870c0b5926b68fb1ea903c3ded95d8f91ae4bd3783cd9d9a in / 
# Fri, 05 Oct 2018 22:58:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 05 Oct 2018 22:58:14 GMT
EXPOSE 3000/tcp
# Fri, 05 Oct 2018 22:58:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 05 Oct 2018 22:58:22 GMT
ENV PASSENGER_VERSION=5.3.5
# Fri, 05 Oct 2018 22:58:33 GMT
RUN buildDeps=' 		make 	' 	&& set -x 	&& apt-get update && apt-get install -y --no-install-recommends $buildDeps && rm -rf /var/lib/apt/lists/* 	&& gem install passenger --version "$PASSENGER_VERSION" 	&& apt-get purge -y --auto-remove $buildDeps
# Fri, 05 Oct 2018 22:58:34 GMT
RUN set -x 	&& passenger-config install-agent 	&& passenger-config download-nginx-engine
# Fri, 05 Oct 2018 22:58:34 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:05d1a5232b461a4b35424129580054caa878cd56f100e34282510bd4b4082e4d`  
		Last Modified: Tue, 04 Sep 2018 21:25:27 GMT  
		Size: 45.3 MB (45310060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4b62449fc8aef4ae6b5df70834999a86a052340178e5b9ee2df979c62a17d4`  
		Last Modified: Wed, 05 Sep 2018 06:49:54 GMT  
		Size: 12.8 MB (12811018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ae4c4adc599f2ab76d6eebe311daeca5cbf71756b6d181771c89b1618e855`  
		Last Modified: Wed, 05 Sep 2018 06:49:50 GMT  
		Size: 207.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f17b4afaac4eb22b0e70f4292d2260119a8ed2ab81285d199b6b0bb84ab63e`  
		Last Modified: Fri, 05 Oct 2018 22:33:19 GMT  
		Size: 21.8 MB (21753642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd96a6b3c421e27b93b2ac615efdb52d284d53ea7cd8506bef30bb0b01a44b8c`  
		Last Modified: Fri, 05 Oct 2018 22:33:16 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2077365091d83152dfe1e5bc07b5c42cba8be7bbf88a993d22892b3f636e44b9`  
		Last Modified: Fri, 05 Oct 2018 23:02:44 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dd687079de897cd32ac9c42e1b77a25154b3228fec4704d72398fa2707af2f`  
		Last Modified: Fri, 05 Oct 2018 23:02:59 GMT  
		Size: 84.6 MB (84635512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8580aed72357b9e88981c25ec22083a148dfafc5da0b14915eda1d93a6135d5`  
		Last Modified: Fri, 05 Oct 2018 23:02:42 GMT  
		Size: 904.1 KB (904132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dd091771dc100ae52341068183bde293375ce60ee370ebea4ef043240a968f`  
		Last Modified: Fri, 05 Oct 2018 23:02:42 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c7cf740aacbe0e0f9094936efce13c20c87060ddf261aef057414b3c7ed6ec`  
		Last Modified: Fri, 05 Oct 2018 23:02:43 GMT  
		Size: 2.5 MB (2456914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e39eb42c606339f3aa53038badcf1c04c118de0eb1df27f77aa8d0dc67eb03`  
		Last Modified: Fri, 05 Oct 2018 23:03:02 GMT  
		Size: 125.0 MB (125021842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c2babb9eb270cb8baed922270fa4bf8d122769a18406b14e036609bf08d8fa`  
		Last Modified: Fri, 05 Oct 2018 23:02:42 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f1ebf80f1f3204159eb71cbf96841ba11fa0781ad8f3ce65e34938e0250ed2`  
		Last Modified: Fri, 05 Oct 2018 23:03:39 GMT  
		Size: 19.1 MB (19116099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427030cee3939e081b3fd6863d101986522a28d278fd28f8607b3f8ee9da5236`  
		Last Modified: Fri, 05 Oct 2018 23:03:37 GMT  
		Size: 4.4 MB (4447460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
