## `mongo:unstable-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:83d7341587a6ea6afd8c1f245515d1af4ecd5ba640967cd93d16647e28e9f45d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.2485; amd64

### `mongo:unstable-windowsservercore-ltsc2016` - windows version 10.0.14393.2485; amd64

```console
$ docker pull mongo@sha256:fcbfafc989691c57a50bdbec130fab280f303614e2e143dae7de36126c7782b3
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5658464278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2fe3ef3b5d68962e9e80c2ecd8e750ea533059650a13bd592132894e152ed7d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Tue, 11 Sep 2018 16:53:50 GMT
RUN Install update 10.0.14393.2485
# Sat, 15 Sep 2018 09:16:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 15 Sep 2018 09:42:40 GMT
ENV MONGO_VERSION=4.1.3
# Sat, 15 Sep 2018 09:42:40 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.1.3-signed.msi
# Sat, 15 Sep 2018 09:42:41 GMT
ENV MONGO_DOWNLOAD_SHA256=58d1aced38f597dbbff4930a82f7b7fbe9affc00e837ae688790a3f3ed52250e
# Fri, 21 Sep 2018 10:12:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 21 Sep 2018 10:12:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 21 Sep 2018 10:12:30 GMT
EXPOSE 27017/tcp
# Fri, 21 Sep 2018 10:12:31 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e046b8e194c642cfc4d7dcaa12ec2f9359e1f54dbc7088ee9ca188416d5c553`  
		Last Modified: Tue, 11 Sep 2018 16:53:50 GMT  
		Size: 1.5 GB (1515870209 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f786254e0429ce7f1ddc69d592364c6179e4c72da867230a987eba95e7d61708`  
		Last Modified: Fri, 21 Sep 2018 10:20:04 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10aa54b7c6669c432ace49d98196d00032b4b1cbdc974368cad57ef75047837`  
		Last Modified: Fri, 21 Sep 2018 10:24:42 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c3ff5b982f152d75c5c790f51bf03bbf94cb440e6d68fb3e77cfe2c531b32`  
		Last Modified: Fri, 21 Sep 2018 10:24:42 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f7d621cf88cf58cb098dffab7125d9f4658477bafc2bd21459de965a0f0a0f`  
		Last Modified: Fri, 21 Sep 2018 10:24:40 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88b803189cea0aa66ea15779de326b029986c2515927329e17b49195c9e1570`  
		Last Modified: Fri, 21 Sep 2018 10:24:56 GMT  
		Size: 72.6 MB (72599795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c7b248aa662f6471be8d73467fd3f5455bcbbf89075ef114b8f9521502e664`  
		Last Modified: Fri, 21 Sep 2018 10:24:40 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a6250daa956ac0cbb2537977cdfd2c51b86e127cac428282bb97c8e0c9de52`  
		Last Modified: Fri, 21 Sep 2018 10:24:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824d528f5c1750f455948e5c224d36b022da848d99c716e3c119d5962d877ebb`  
		Last Modified: Fri, 21 Sep 2018 10:24:40 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
