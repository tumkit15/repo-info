## `mongo:unstable-windowsservercore-1803`

```console
$ docker pull mongo@sha256:462d01ce883fe9ce2c14a3c4a5fe1b22124d9d1daca2f3cbc8face9a508a6a64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.285; amd64

### `mongo:unstable-windowsservercore-1803` - windows version 10.0.17134.285; amd64

```console
$ docker pull mongo@sha256:d1a2c37a4d6c3b3416c391fddeacd937d0b634f966f7b156f0ede4b314a03b06
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2274351325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a807cbdd35830dc92cc493c9f87eb07b889153c8d4bc39ebe92f3fa706db70b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 10.0.17134.1
# Sun, 09 Sep 2018 17:20:44 GMT
RUN Install update 10.0.17134.285
# Sat, 15 Sep 2018 09:39:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 15 Sep 2018 09:48:19 GMT
ENV MONGO_VERSION=4.1.3
# Sat, 15 Sep 2018 09:48:20 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.1.3-signed.msi
# Sat, 15 Sep 2018 09:48:21 GMT
ENV MONGO_DOWNLOAD_SHA256=58d1aced38f597dbbff4930a82f7b7fbe9affc00e837ae688790a3f3ed52250e
# Fri, 21 Sep 2018 10:19:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 21 Sep 2018 10:19:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 21 Sep 2018 10:19:09 GMT
EXPOSE 27017/tcp
# Fri, 21 Sep 2018 10:19:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f036448990c273bb1accf8d436799639bbb644326ae47f30fe4faed21c8d8d9`  
		Last Modified: Tue, 11 Sep 2018 17:11:59 GMT  
		Size: 547.2 MB (547225773 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:72421b921bc76cd58967f35b89a741539cec39dab3ff330e790096ac6853216a`  
		Last Modified: Fri, 21 Sep 2018 10:24:09 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01874927ef78b40cc4812d0143cbe1a9aa289e8b836d7f80caec477e0eb88dc4`  
		Last Modified: Fri, 21 Sep 2018 10:25:47 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79be5af18f21c11fbee2bbdaa234d2a455fe62a5e99c4117e720245abb13492f`  
		Last Modified: Fri, 21 Sep 2018 10:25:46 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6117c24450ad288f5f838e4553e923e365862af30f823d6292d9f79a6dac1472`  
		Last Modified: Fri, 21 Sep 2018 10:25:43 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad6e20a9b78536e1767197a4ed7cbe0bbc21b5ae7bb84979476cdc3c30e408`  
		Last Modified: Fri, 21 Sep 2018 10:26:00 GMT  
		Size: 67.4 MB (67428885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4b7ca7cb1b88221d39fc758d723ac11176c8fc869e2e5b8dbbc9d9ae930e00`  
		Last Modified: Fri, 21 Sep 2018 10:25:43 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c7ab056c95598a7d83cf5339abf2dc992a42926d4b0c608cabca193196a891`  
		Last Modified: Fri, 21 Sep 2018 10:25:44 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf1d965e2250ae3e61c70c14f08735696b228467b5e413611bcc54ec9aa2219`  
		Last Modified: Fri, 21 Sep 2018 10:25:43 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
