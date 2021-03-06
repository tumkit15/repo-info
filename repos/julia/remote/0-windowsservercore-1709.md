## `julia:0-windowsservercore-1709`

```console
$ docker pull julia@sha256:e53431d46bdb556aa3b93bd5ade55868b3b57f3ea759bda38020b7d596047107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.665; amd64

### `julia:0-windowsservercore-1709` - windows version 10.0.16299.665; amd64

```console
$ docker pull julia@sha256:e81c03db78f7552de1f596c5045f1e4c19e02351fcbb873edd6457ee8d45d1eb
```

-	Docker Version: 17.06.2-ee-13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 GB (3245024941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317f7c2529904ecaaceccdc6c30941085c8c68e55cff91109cb8f63fe9260885`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sun, 09 Sep 2018 17:24:12 GMT
RUN Install update 10.0.16299.665
# Thu, 13 Sep 2018 09:47:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 03 Oct 2018 11:31:40 GMT
ENV JULIA_VERSION=0.7.0
# Wed, 03 Oct 2018 11:31:41 GMT
ENV JULIA_SHA256=a42d53d259d1f8f6feefac0da8352c19ca5d9da2303cf1595086867cfb1cd817
# Wed, 03 Oct 2018 11:34:33 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 03 Oct 2018 11:34:34 GMT
CMD ["julia"]
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
	-	`sha256:4fb86bf538a7672fc269d740738c9dea323819696c6a7cc356be061254654a3b`  
		Last Modified: Wed, 03 Oct 2018 11:38:15 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4193237f0b5eda8a72a608d40f1ed8b7e65556d0f112f1d3e107231f101ca28`  
		Last Modified: Wed, 03 Oct 2018 11:38:15 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3d585fa4bc4d7ad1ef717ce38a27ff930d4db51f296720b3f0589e0943f913`  
		Last Modified: Wed, 03 Oct 2018 11:38:46 GMT  
		Size: 112.4 MB (112384061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecd984d511cd7ab0064a0fa8836b6c655168d25191d1a434a270cc0c36b653e`  
		Last Modified: Wed, 03 Oct 2018 11:38:15 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
