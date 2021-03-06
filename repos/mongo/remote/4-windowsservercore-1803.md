## `mongo:4-windowsservercore-1803`

```console
$ docker pull mongo@sha256:2a88d52318bf9b890e50d09a7bc9d78d42a1ca8359ef9c75ca75d5c006eb14ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.285; amd64

### `mongo:4-windowsservercore-1803` - windows version 10.0.17134.285; amd64

```console
$ docker pull mongo@sha256:ff9d70e9ee3e349bca3d118dd198a0c1de83772c6589ce4af81adc5fde96e818
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2265353127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:521d670be8c965f8030b6462c1182d1ea32cfa463a30c07eb5d3f1e89d5ee0f0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 10.0.17134.1
# Sun, 09 Sep 2018 17:20:44 GMT
RUN Install update 10.0.17134.285
# Sat, 15 Sep 2018 09:39:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 04 Oct 2018 09:23:31 GMT
ENV MONGO_VERSION=4.0.3
# Thu, 04 Oct 2018 09:23:31 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.3-signed.msi
# Thu, 04 Oct 2018 09:23:32 GMT
ENV MONGO_DOWNLOAD_SHA256=0e53cfd224d27862c286b765b85d769b39e3518b2dc2704ff87bd8a565ea9b7f
# Thu, 04 Oct 2018 09:26:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 04 Oct 2018 09:26:25 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 04 Oct 2018 09:26:27 GMT
EXPOSE 27017/tcp
# Thu, 04 Oct 2018 09:26:28 GMT
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
	-	`sha256:f2d58fae32a7dd0e093ccaf525a643520fe24d0c579ff96d24df8a3c7995e39f`  
		Last Modified: Thu, 04 Oct 2018 09:28:29 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e9ad12e4e0c7aeb9753b7959414d0e9dc9b496d20e89b4591a84d4d2d953ab`  
		Last Modified: Thu, 04 Oct 2018 09:28:29 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da10e3ea9988868e3cc1f397767ffd3e7035a9f6b31e4a5113346361456bb122`  
		Last Modified: Thu, 04 Oct 2018 09:28:27 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713ac5302bf688490c9d49321b866050b6bb13af8043a5373b3237f12edc0192`  
		Last Modified: Thu, 04 Oct 2018 09:28:40 GMT  
		Size: 58.4 MB (58430691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f976c21079e627b1b068df97b15a439dc65475b151b55350c7483713546c46f5`  
		Last Modified: Thu, 04 Oct 2018 09:28:27 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952c17aa0e5cc4de89afad1b3af498e6378aa2c3cafed7e197be4501f4240fe8`  
		Last Modified: Thu, 04 Oct 2018 09:28:27 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fcb17ad0a0eb4b32163d89feb2bb54d96ff664a8cf055c95547d3758df61c1`  
		Last Modified: Thu, 04 Oct 2018 09:28:27 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
