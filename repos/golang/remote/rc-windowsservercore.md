## `golang:rc-windowsservercore`

```console
$ docker pull golang@sha256:6397056e9da35aebdb396a386adcc05fd4ae2275ae6ad9ea7b1e2e66332c64a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.2312; amd64
	-	windows version 10.0.16299.492; amd64

### `golang:rc-windowsservercore` - windows version 10.0.14393.2312; amd64

```console
$ docker pull golang@sha256:5b1119fc42d197c112590d629d9d687447cf6350fc51b26fc3399e94a774a1b5
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5700450351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294da10a0eaf0e448b27c83773759bff0fa2cfe2ff98f7190089665aae8e42c3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Wed, 13 Jun 2018 00:36:30 GMT
RUN Install update 10.0.14393.2312
# Tue, 03 Jul 2018 00:23:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 03 Jul 2018 00:23:43 GMT
ENV GIT_VERSION=2.11.1
# Tue, 03 Jul 2018 00:23:44 GMT
ENV GIT_TAG=v2.11.1.windows.1
# Tue, 03 Jul 2018 00:23:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.11.1.windows.1/MinGit-2.11.1-64-bit.zip
# Tue, 03 Jul 2018 00:23:45 GMT
ENV GIT_DOWNLOAD_SHA256=668d16a799dd721ed126cc91bed49eb2c072ba1b25b50048280a4e2c5ed56e59
# Tue, 03 Jul 2018 00:25:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 		Write-Host 'Complete.';
# Tue, 03 Jul 2018 00:25:34 GMT
ENV GOPATH=C:\gopath
# Tue, 03 Jul 2018 00:26:38 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 03 Jul 2018 00:26:39 GMT
ENV GOLANG_VERSION=1.11beta1
# Tue, 03 Jul 2018 00:32:27 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1eeb874a919143f3e62b641ccd5ebbfd1b3d4f2184de1d6497f7b2b6df996960'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 03 Jul 2018 00:32:29 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8e9da9bbe3af2118a0b5eef7a3d649367557d0d3992ed0213c79857b23b4140e`  
		Last Modified: Wed, 13 Jun 2018 00:36:30 GMT  
		Size: 1.4 GB (1414319443 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:650685bf03844147638a02f1b62114e24cf12bf85feb92b6e2273d551a54c647`  
		Last Modified: Tue, 03 Jul 2018 01:20:32 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a91cb469c7e359d741522bed0e10c649670cfb3641af9c3cac4d93f2423df`  
		Last Modified: Tue, 03 Jul 2018 01:20:27 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8620bdbf56ed7bd0c8b1631a4af59f14ac8b13b1a35a419effed5ec5833d81`  
		Last Modified: Tue, 03 Jul 2018 01:20:27 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f22b0f509ad85923738743a615bdea603c33c88950a9a98f767cab9388a3e8`  
		Last Modified: Tue, 03 Jul 2018 01:20:24 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df5f4eb693cb8a03451955a74621e10cccf27271739ccb347b2aba30e4ae776`  
		Last Modified: Tue, 03 Jul 2018 01:20:23 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b05ca26dfe593b9d3d71f88f926f989dde3098abf546ea352705a8d592ec535`  
		Last Modified: Tue, 03 Jul 2018 01:20:36 GMT  
		Size: 29.4 MB (29418486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226aa27d434e3715787b7423db91aa0b17f5935a306412dc1e9bdd0024426551`  
		Last Modified: Tue, 03 Jul 2018 01:20:20 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93a88f4c490a44ae518df594618c85ae0740b85bd552f597b1db11b9c80f3f3`  
		Last Modified: Tue, 03 Jul 2018 01:20:24 GMT  
		Size: 5.0 MB (4957116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd70231903598ec134898bdc51f4ce57174266a27c161d33ac11419c09219eb`  
		Last Modified: Tue, 03 Jul 2018 01:20:21 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbff30d3fa34e99fccc7fe6285c80073f46439c076fc69f9343a120efac001d4`  
		Last Modified: Tue, 03 Jul 2018 01:21:53 GMT  
		Size: 181.8 MB (181759695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac53ba20e8119f58b384b42fe6873b50dfdc468e47bda0c267c6a365c0df366`  
		Last Modified: Tue, 03 Jul 2018 01:20:20 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-windowsservercore` - windows version 10.0.16299.492; amd64

```console
$ docker pull golang@sha256:4b1d3787cb75ad4937b27d1b87bfe8b7d6d1e6576119a5a08aec66b47273842c
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3308699990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f0f7f9495eca9f828f49743a33ef0832acc7b62651b26ffe2d10324e4e714fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Mon, 11 Jun 2018 20:38:48 GMT
RUN Install update 10.0.16299.492
# Tue, 03 Jul 2018 00:32:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 03 Jul 2018 00:32:42 GMT
ENV GIT_VERSION=2.11.1
# Tue, 03 Jul 2018 00:32:43 GMT
ENV GIT_TAG=v2.11.1.windows.1
# Tue, 03 Jul 2018 00:32:44 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.11.1.windows.1/MinGit-2.11.1-64-bit.zip
# Tue, 03 Jul 2018 00:32:45 GMT
ENV GIT_DOWNLOAD_SHA256=668d16a799dd721ed126cc91bed49eb2c072ba1b25b50048280a4e2c5ed56e59
# Tue, 03 Jul 2018 00:34:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 		Write-Host 'Complete.';
# Tue, 03 Jul 2018 00:34:27 GMT
ENV GOPATH=C:\gopath
# Tue, 03 Jul 2018 00:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 03 Jul 2018 00:35:14 GMT
ENV GOLANG_VERSION=1.11beta1
# Tue, 03 Jul 2018 00:41:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1eeb874a919143f3e62b641ccd5ebbfd1b3d4f2184de1d6497f7b2b6df996960'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 03 Jul 2018 00:41:06 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b9c63e313c8b374d5767c602fd6f2b947a3f1df9a8f8c5fcecb2fa6b1cfa968`  
		Last Modified: Wed, 13 Jun 2018 01:11:53 GMT  
		Size: 823.6 MB (823576248 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3989f186f0fc841be4fd06c5f4d58afe814bf92ffa0940def6b8d21ea38c223f`  
		Last Modified: Tue, 03 Jul 2018 01:22:20 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be9b417a88820877751cabcf39e3146ad1ab906b2ea03a402fc2c8c80ac63cd`  
		Last Modified: Tue, 03 Jul 2018 01:22:19 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d322a253d4e6b1042c99e15204b98272914fc6a977cc8e43f561d36c409974`  
		Last Modified: Tue, 03 Jul 2018 01:22:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d26f8ebc8846286e8ec3c1ad0caef4f3efa36d801c44f4c85fe1974e4985f36`  
		Last Modified: Tue, 03 Jul 2018 01:22:16 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbdea9ee4b8bfb010cf3410f4bbb85103ff94d9ad96e1ebe5dd863be875fcbd`  
		Last Modified: Tue, 03 Jul 2018 01:22:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37b383766e6fa050f0826e2e271967cb531e76bf089bf4e2020960418b5b9eb`  
		Last Modified: Tue, 03 Jul 2018 01:22:28 GMT  
		Size: 29.1 MB (29120783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff7982cd7f2036cd30289e69b2b7962f4b78c90b20cf8fd8e5bae1dce935fed`  
		Last Modified: Tue, 03 Jul 2018 01:22:13 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6cab04e28059c3e43f99bb05d15d5f14e0cb87711a9d919f9ae954a8d275bd`  
		Last Modified: Tue, 03 Jul 2018 01:22:14 GMT  
		Size: 4.7 MB (4681808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6644ea707dec024576ed8e38597235be44c073b2ff7919a6d30e043fee7a76a3`  
		Last Modified: Tue, 03 Jul 2018 01:22:13 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a1244190b0c56890a07c01d745c4544773dd3723b91a5044211201610cece6`  
		Last Modified: Tue, 03 Jul 2018 01:23:45 GMT  
		Size: 177.0 MB (177010890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47907aba4a4e458591b5f1a69b7d0401268ec667572e11cceeea180b737cbcbb`  
		Last Modified: Tue, 03 Jul 2018 01:22:13 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip