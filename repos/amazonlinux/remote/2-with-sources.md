## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:b1c3711b788e9988a33b5d25b10834e6820af5e8f1b3d7310e906e84fe85bf5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:99c07c7e493763233bf370f356483e7c87cf7227508b7bc3213ed73211e8562f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.1 MB (412118259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e87c4c9c98c86dfa25b38e1c80b5b4093d5bb31b136ed39852c4acf0702a66`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Aug 2018 21:43:19 GMT
ADD file:29628d035f4e1bda4091dd25aecb8910351a3cbb0b06215d1c61f0ba4028f4c8 in / 
# Thu, 30 Aug 2018 21:43:19 GMT
CMD ["/bin/bash"]
# Thu, 30 Aug 2018 21:43:31 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/amzn2/srpm-bundle.tar.gz?versionId=0KdltZx3MM5vxoNe2pcOqdYDebiCRhU0"  && echo "b6a703acc414a896f65edaa797ac89c90febc63e01a09b7f962e8ab64ed7d090 /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:9a9707b030c2d5858e197de8b01ec47adfdf2b7289ae25b73aa30091844491a8`  
		Last Modified: Thu, 30 Aug 2018 21:44:13 GMT  
		Size: 61.6 MB (61628165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205ad25884aa9db59eca275c02bced9023061bfb61bf3145d98faf1abaac7e4`  
		Last Modified: Thu, 30 Aug 2018 21:44:37 GMT  
		Size: 350.5 MB (350490094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
