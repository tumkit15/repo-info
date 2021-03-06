## `openjdk:11-windowsservercore`

```console
$ docker pull openjdk@sha256:4eaceb3f6e52250f05deaa74a3e7f6602673bfb7d12b00edb505c001bdf08d0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.2485; amd64
	-	windows version 10.0.16299.665; amd64
	-	windows version 10.0.17134.285; amd64

### `openjdk:11-windowsservercore` - windows version 10.0.14393.2485; amd64

```console
$ docker pull openjdk@sha256:ba435ad31ee2f1ea39fc6a58b82c65c7661aa6d02bc878c714dbef4864c3b529
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5778685207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4884c762b4f811319cebc58e4f9dcefe48a112dd017a76da8c82e102a63d1d6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Tue, 11 Sep 2018 16:53:50 GMT
RUN Install update 10.0.14393.2485
# Thu, 13 Sep 2018 09:42:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 03 Oct 2018 10:37:07 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 03 Oct 2018 10:38:27 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 03 Oct 2018 10:38:28 GMT
ENV JAVA_VERSION=11
# Wed, 03 Oct 2018 10:38:29 GMT
ENV JAVA_URL=https://download.java.net/java/ga/jdk11/openjdk-11_windows-x64_bin.zip
# Wed, 03 Oct 2018 10:38:30 GMT
ENV JAVA_SHA256=fde3b28ca31b86a889c37528f17411cd0b9651beb6fa76cac89a223417910f4b
# Wed, 03 Oct 2018 10:41:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 	Write-Host '  javac --version'; javac --version; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Complete.'
# Wed, 03 Oct 2018 10:41:04 GMT
CMD ["jshell"]
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
	-	`sha256:7aa2ad8eff720622c1b1f25bf31d2c32b588766208c093caef00e8b31961b74e`  
		Last Modified: Thu, 13 Sep 2018 10:24:13 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc3b246e6fc8f7357365b67034c119a2fd89685d8deb70b56b0de7b2292e73c`  
		Last Modified: Wed, 03 Oct 2018 11:08:50 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb40d60fad1387bf043f7eb020cb9e700680a2664f1a6f4ae0261330f69c78c0`  
		Last Modified: Wed, 03 Oct 2018 11:08:54 GMT  
		Size: 5.1 MB (5101896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2291c515b826ad4a93a0462ca4e0446535998f10699f888adbdefd9a91140e`  
		Last Modified: Wed, 03 Oct 2018 11:08:48 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285ac003cb1f9891c0e0da4b297d7fed6507868ba75e3a05b8db80ac38a7e921`  
		Last Modified: Wed, 03 Oct 2018 11:08:48 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10868e617c5f4d4701ebcd1a22cba2b324193beb4f1b4a6fa40b399182611ebf`  
		Last Modified: Wed, 03 Oct 2018 11:08:48 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e96dac622a05307bd19354d9e532f211495f4c663d05ebe943a6bb4d7613bf7`  
		Last Modified: Wed, 03 Oct 2018 11:09:31 GMT  
		Size: 187.7 MB (187719993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ad8eb0b34b0a7a993f2159bcc1ae6c5107c27a45aa8e934ff71916ed0e4c3`  
		Last Modified: Wed, 03 Oct 2018 11:08:48 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-windowsservercore` - windows version 10.0.16299.665; amd64

```console
$ docker pull openjdk@sha256:c6b6f029b7d6296ae55649b71f6a26ccda3072376d03ed60d9c9dde75c7f0d8f
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3324780506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183a825af28a12470c7f3e558bcdad7efa795847d3ad45b9bb51903581a697a8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sun, 09 Sep 2018 17:24:12 GMT
RUN Install update 10.0.16299.665
# Thu, 13 Sep 2018 09:47:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 03 Oct 2018 10:41:09 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 03 Oct 2018 10:42:02 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 03 Oct 2018 10:42:04 GMT
ENV JAVA_VERSION=11
# Wed, 03 Oct 2018 10:42:05 GMT
ENV JAVA_URL=https://download.java.net/java/ga/jdk11/openjdk-11_windows-x64_bin.zip
# Wed, 03 Oct 2018 10:42:06 GMT
ENV JAVA_SHA256=fde3b28ca31b86a889c37528f17411cd0b9651beb6fa76cac89a223417910f4b
# Wed, 03 Oct 2018 10:44:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 	Write-Host '  javac --version'; javac --version; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Complete.'
# Wed, 03 Oct 2018 10:44:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 18 Sep 2018 22:35:04 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5b83e25f92aef992a2827d664111b4726ada7d0b13d7af21882734cab96d8d0`  
		Last Modified: Tue, 11 Sep 2018 17:07:56 GMT  
		Size: 858.3 MB (858335510 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa61e3e01eeaa5482e77157970441ee8c2414720462e140b668a5b58902a78f5`  
		Last Modified: Thu, 13 Sep 2018 10:25:08 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:586217c4e250d3517218500cf05e01749f32c66086eedcb1c8325361bd93bf61`  
		Last Modified: Wed, 03 Oct 2018 11:09:49 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e583335e7bdeef62348f7a1fd384e5cd6cf6182e4275385221fa2e9b2e44ae4`  
		Last Modified: Wed, 03 Oct 2018 11:09:51 GMT  
		Size: 4.7 MB (4740426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbed90bdf52d95ab10a3abdaaddd89f5ec91e6fedaf072b22024f8bde035073`  
		Last Modified: Wed, 03 Oct 2018 11:09:47 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085a0a90ac87b415537129f51103e5a129cc2fce432916c66a5238755d5512dc`  
		Last Modified: Wed, 03 Oct 2018 11:09:47 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d7367487ff534c2d9a58e36d3b3f8e460acc7afacbc3476650c6984443cf3c`  
		Last Modified: Wed, 03 Oct 2018 11:09:46 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf89871bf1c88b00a70e03207a9718107f70f81b4d811ae95ccd732b3eab6b24`  
		Last Modified: Wed, 03 Oct 2018 11:10:13 GMT  
		Size: 187.4 MB (187396796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a162f0111f1569d308e44b677f0aa3bc0a575ce0f247ceefd16a90de7eb82c`  
		Last Modified: Wed, 03 Oct 2018 11:09:47 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-windowsservercore` - windows version 10.0.17134.285; amd64

```console
$ docker pull openjdk@sha256:8c52ae1d39cd868b6b1822a852354ff4eb0df86e665efd5d3ffc71c118041d09
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2394595463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57d44e82a6954becf1b00e0e16414d42ffa394d4bb3e4ab1f3ec1ed2bedf8ee`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 10.0.17134.1
# Sun, 09 Sep 2018 17:20:44 GMT
RUN Install update 10.0.17134.285
# Thu, 13 Sep 2018 09:50:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 03 Oct 2018 10:44:13 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 03 Oct 2018 10:45:03 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 03 Oct 2018 10:45:04 GMT
ENV JAVA_VERSION=11
# Wed, 03 Oct 2018 10:45:05 GMT
ENV JAVA_URL=https://download.java.net/java/ga/jdk11/openjdk-11_windows-x64_bin.zip
# Wed, 03 Oct 2018 10:45:06 GMT
ENV JAVA_SHA256=fde3b28ca31b86a889c37528f17411cd0b9651beb6fa76cac89a223417910f4b
# Wed, 03 Oct 2018 10:46:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 	Write-Host '  javac --version'; javac --version; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Complete.'
# Wed, 03 Oct 2018 10:46:58 GMT
CMD ["jshell"]
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
	-	`sha256:499c5d8410bcb30d8e576aa1248844529b2af7aff7307a4b79f366790c87756f`  
		Last Modified: Thu, 13 Sep 2018 10:26:08 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbedf3867f83e747f4d46d841c7ea751b8096686c02651c3dd7a250bdc3e68e5`  
		Last Modified: Wed, 03 Oct 2018 11:10:32 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64e6afc1d72115f82da84ef44286dd6f0336704f99c66cbe09679b4109a472e`  
		Last Modified: Wed, 03 Oct 2018 11:10:34 GMT  
		Size: 4.7 MB (4670527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5632ebcccbfacb40933469e0f86ec762c8cc489b1f76eccaaddc95aaee34ba18`  
		Last Modified: Wed, 03 Oct 2018 11:10:30 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185c19ef7c52223f74d4d2cb73d89cad4ec7b3894850b49dc894903490338d18`  
		Last Modified: Wed, 03 Oct 2018 11:10:29 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958b505c00908b3b8d17bcb1808f2c295bc1720361e6ff5988979b0258287936`  
		Last Modified: Wed, 03 Oct 2018 11:10:29 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52711d4ca783c468005b058f2865febeeef6d3afa07f7a78b5e76f6d819eb74`  
		Last Modified: Wed, 03 Oct 2018 11:11:05 GMT  
		Size: 183.0 MB (183003702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278468ad6e62e7cde6f2efb8648f2fb6aab8696becf0f84b3f088fc0ed1ac581`  
		Last Modified: Wed, 03 Oct 2018 11:10:29 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
