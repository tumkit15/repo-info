## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:4a61f65a7d65bee92e6042c0760854af6f914112ffe6231b760f27cbe3242c8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.2485; amd64

### `golang:1-nanoserver` - windows version 10.0.14393.2485; amd64

```console
$ docker pull golang@sha256:9ca865f2b3cc262648ff0d5a0b979292cbed914dd8a312c304b96021b3e250fc
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.7 MB (565714237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea4c05f6dd74a648171018a1985aba76ca83d7edde7f279fbd0a4b8614a51644`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:47:17 GMT
RUN Apply image 10.0.14393.0
# Tue, 11 Sep 2018 16:53:25 GMT
RUN Install update 10.0.14393.2485
# Thu, 13 Sep 2018 10:13:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 03 Oct 2018 09:43:07 GMT
ENV GOPATH=C:\gopath
# Wed, 03 Oct 2018 09:43:53 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Wed, 03 Oct 2018 09:43:54 GMT
ENV GOLANG_VERSION=1.11.1
# Wed, 03 Oct 2018 09:49:44 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '230a08d4260ded9d769f072512a49bffe8bfaff8323e839c2db7cf7c9c788130'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Wed, 03 Oct 2018 09:49:45 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:bce2fbc256ea437a87dadac2f69aabd25bed4f56255549090056c1131fad0277`  
		Last Modified: Mon, 17 Sep 2018 20:04:15 GMT  
		Size: 252.7 MB (252691002 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b1b0c61be11f6d053756595f70211e6044137b150fc1cc23d52ee0852eaf9146`  
		Last Modified: Tue, 11 Sep 2018 16:53:25 GMT  
		Size: 180.5 MB (180533966 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d47ca3c2a708c20309f263de7441f23acb1e8b76c56c75bcc314d2af593e2d17`  
		Last Modified: Thu, 13 Sep 2018 10:33:11 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2beb060d746862a2aeaaeb2e761a5fe91f07420d6d296322f895a574e265d086`  
		Last Modified: Wed, 03 Oct 2018 10:17:47 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f865f947b98c9efc30d19e4f835306b3d3ba08dd6ce301f2cfb0b67ab93dd46c`  
		Last Modified: Wed, 03 Oct 2018 10:17:48 GMT  
		Size: 951.1 KB (951077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af742a096213a783479adf6650170a7cec386d135113f9b303bbc54d72d776b`  
		Last Modified: Wed, 03 Oct 2018 10:17:47 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c54bbb92ce1b8b4dacd7020fbe28d0952b6bbfe45d9bb85eb4b811cb22fde0d`  
		Last Modified: Wed, 03 Oct 2018 10:19:16 GMT  
		Size: 131.5 MB (131534190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beabe250dcbfb291c02ae1580c8c64e37d866bdf4be8bf213adb74c6e0edcd2f`  
		Last Modified: Wed, 03 Oct 2018 10:17:47 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
