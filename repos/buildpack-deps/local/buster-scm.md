# `buildpack-deps:buster-scm`

## Docker Metadata

- Image ID: `sha256:9e92bb03d1b1e82b2ed6314b7c63a03873f2d7ff1f86422e4fd055bd61e116e3`
- Created: `2018-09-04T22:21:29.916614569Z`
- Virtual Size: ~ 283.49 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-3`

Binary Packages:

- `libacl1:amd64=2.2.52-3+b1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-3
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-3.dsc' acl_2.2.52-3.dsc 2025 SHA256:82e344b9ab176559a85630b74ee5a68d678d7f24b6fe8139f2fd9fcf38a48095
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-3.debian.tar.xz' acl_2.2.52-3.debian.tar.xz 8740 SHA256:fc3f1178d18288993fc4ce4853b7f9dcdf0bd1fd26e4f69349a4e4e5916d1fa8
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.2.52-3/ (for browsing the source)
- https://sources.debian.net/src/acl/2.2.52-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.2.52-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `adduser=3.117`

Binary Packages:

- `adduser=3.117`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/adduser/3.117/


### `dpkg` source package: `apr-util=1.6.1-2`

Binary Packages:

- `libaprutil1:amd64=1.6.1-2`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apr-util/1.6.1-2/


### `dpkg` source package: `apr=1.6.3-3`

Binary Packages:

- `libapr1:amd64=1.6.3-3`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.3-3
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.6.3-3.dsc' apr_1.6.3-3.dsc 2296 SHA256:3c4d3351d64619ca032268d85e7b14a607f918df41c546c12ee0a594788920b4
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.6.3.orig.tar.bz2' apr_1.6.3.orig.tar.bz2 854100 SHA256:131f06d16d7aabd097fa992a33eec2b6af3962f93e6d570a9bd4d85e95993172
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.6.3.orig.tar.bz2.asc' apr_1.6.3.orig.tar.bz2.asc 801 SHA256:33db39162f7ca9acdccaa4f19630a67045542791b262116d3512c8b5d7c3fca1
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.6.3-3.debian.tar.xz' apr_1.6.3-3.debian.tar.xz 213292 SHA256:0966c89da8e186bafcd15aa65c77e153549025a1efbe1005ca9a54b77a0b7315
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr/1.6.3-3/ (for browsing the source)
- https://sources.debian.net/src/apr/1.6.3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr/1.6.3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=1.6.4`

Binary Packages:

- `apt=1.6.4`
- `libapt-pkg5.0:amd64=1.6.4`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/1.6.4/


### `dpkg` source package: `attr=1:2.4.47-2`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2+b2`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.47-2
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.47-2.dsc' attr_2.4.47-2.dsc 2027 SHA256:ee842d6d62d473acf02b494c432cf33128fa46455a09d3172c77c252449fa1a6
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.47.orig.tar.bz2' attr_2.4.47.orig.tar.bz2 281877 SHA256:6c1208035757f5ce9b516402dd45b8299a53ae4d69ad2c352116f9cb8d7bc274
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.47-2.debian.tar.xz' attr_2.4.47-2.debian.tar.xz 8096 SHA256:f65909562def601b1556393f5656032c058dc574ba622414ad3eb80c7b05a42a
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.4.47-2/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.4.47-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.4.47-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:2.8.3-1`

Binary Packages:

- `libaudit-common=1:2.8.3-1`
- `libaudit1:amd64=1:2.8.3-1+b1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.3-1
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.3-1.dsc' audit_2.8.3-1.dsc 2483 SHA256:ae5afc029ff8d5144fd141a29e602a8f92cc8da08174384cc1c614dd839a112d
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.3.orig.tar.gz' audit_2.8.3.orig.tar.gz 1107583 SHA256:744945caee27a472f0cc7ecb067f1f33d606e5aebcf9660e701a58f9d3668a1a
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.3-1.debian.tar.xz' audit_2.8.3-1.debian.tar.xz 15460 SHA256:b4502d3890042d5fee3fa5af61eecf66c537dbd80bc11c7878a53d242b95ef0a
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:2.8.3-1/ (for browsing the source)
- https://sources.debian.net/src/audit/1:2.8.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:2.8.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=10.1`

Binary Packages:

- `base-files=10.1`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=10.1
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_10.1.dsc' base-files_10.1.dsc 1071 SHA256:993f58ec810722bf0210e06e351d58f1a316827b0995ffd03edbd2c3dc406130
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_10.1.tar.xz' base-files_10.1.tar.xz 65064 SHA256:368d2c32572802838de1151be45e8964669d3901429856bee06d219f125801d3
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/10.1/ (for browsing the source)
- https://sources.debian.net/src/base-files/10.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/10.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.5.45`

Binary Packages:

- `base-passwd=3.5.45`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.45
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.45.dsc' base-passwd_3.5.45.dsc 1651 SHA256:c5702c8c0fd5f2240d0fad07f1c03cdff86ea9370e80129c7258c40fa12015b9
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.45.tar.xz' base-passwd_3.5.45.tar.xz 52748 SHA256:8cd6a713c400cf52f437e5cb14fcec59b0c77d4003a9a4f56526ef27f28ce1fe
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.45/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.45/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.45/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=4.4.18-3.1`

Binary Packages:

- `bash=4.4.18-3.1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.4.18-3.1
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.4.18-3.1.dsc' bash_4.4.18-3.1.dsc 2309 SHA256:67fc85e76d8901fa44342aa0c61722dbf0667eea8de240ba6067636ab07236f8
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.4.18.orig.tar.xz' bash_4.4.18.orig.tar.xz 5036272 SHA256:704143a7170041ac9f1025455d6d23ff0f353711a3dc557b47d6e6322f24cd02
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.4.18-3.1.debian.tar.xz' bash_4.4.18-3.1.debian.tar.xz 60632 SHA256:68a6aaaa16c0b975176d421f38e7c5fb746f7a3a262cb699bf5a92e4fbcfba39
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/4.4.18-3.1/ (for browsing the source)
- https://sources.debian.net/src/bash/4.4.18-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/4.4.18-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.6-9`

Binary Packages:

- `libbz2-1.0:amd64=1.0.6-9`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-9
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-9.dsc' bzip2_1.0.6-9.dsc 2185 SHA256:f27d7febca8dbc1519bdacac3ee0b5a2d9cf9845e50dbb7b13c0e6daa17ab28e
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-9.debian.tar.bz2' bzip2_1.0.6-9.debian.tar.bz2 25873 SHA256:d1a91bf31bc60384f56fa2dd55cfdc07e27dbbbf295db2248b65afed0ca141a2
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.6-9/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.6-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.6-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates=20170717`

Binary Packages:

- `ca-certificates=20170717`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20170717
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20170717.dsc' ca-certificates_20170717.dsc 1506 SHA256:da6268ff88e05c85c23c62add13d3d127087467d0c7e83974ca28db5543a252a
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20170717.tar.xz' ca-certificates_20170717.tar.xz 293028 SHA256:e487639b641fa75445174734dd6e9d600373e3248b3d86a7e3c6d0f6977decd2
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20170717/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20170717/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20170717/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cdebconf=0.244`

Binary Packages:

- `libdebconfclient0:amd64=0.244`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cdebconf/0.244/


### `dpkg` source package: `coreutils=8.28-1`

Binary Packages:

- `coreutils=8.28-1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/coreutils/8.28-1/


### `dpkg` source package: `curl=7.61.0-1`

Binary Packages:

- `curl=7.61.0-1`
- `libcurl3-gnutls:amd64=7.61.0-1`
- `libcurl4:amd64=7.61.0-1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.61.0-1
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.61.0-1.dsc' curl_7.61.0-1.dsc 2662 SHA256:f7a9c3d60f75ff16dae8bde2efc632d12b5d306d2dd2f0b7bad5ebc61c3f2830
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.61.0.orig.tar.gz' curl_7.61.0.orig.tar.gz 3964862 SHA256:64141f0db4945268a21b490d58806b97c615d3d0c75bf8c335bbe0efd13b45b5
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.61.0-1.debian.tar.xz' curl_7.61.0-1.debian.tar.xz 28348 SHA256:3bdcd5605cf1e7fdf10aa7009e55ae16fd518e6ae193e262ade19a1d24ce5134
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.61.0-1/ (for browsing the source)
- https://sources.debian.net/src/curl/7.61.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.61.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.27~101-g0780600+dfsg-3.1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27~101-g0780600+dfsg-3.1`
- `libsasl2-modules-db:amd64=2.1.27~101-g0780600+dfsg-3.1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27~101-g0780600+dfsg-3.1
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3.1.dsc' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3.1.dsc 3522 SHA256:dd620adc358eb9831e42291c3b10c1749a2f837cb4fcb7553709edbccd37a164
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz 1143888 SHA256:69f34971f768e7ee6a6b647ec2d16a5a72a854ecd4602b019d5f79ba61063fdc
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3.1.debian.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3.1.debian.tar.xz 94780 SHA256:f036ab5b68d4f24ccdba41ccb566f395e15a1374f0a0d67963989f829cca3b9d
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3.1/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.8-2.10`

Binary Packages:

- `dash=0.5.8-2.10`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/dash/0.5.8-2.10/


### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.1`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg1-0.1/


### `dpkg` source package: `debconf=1.5.69`

Binary Packages:

- `debconf=1.5.69`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.69
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.69.dsc' debconf_1.5.69.dsc 2047 SHA256:d1d83db20bac5c611fa9c74091d193f8d0e30cdf6afec9395354e6cc8ff8aac4
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.69.tar.xz' debconf_1.5.69.tar.xz 570688 SHA256:728b0df9ba36ee2e090b5be9a79ebb9ff55605e38bd6780b26462a8c8bd0f646
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.69/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.69/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.69/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debian-archive-keyring=2017.7`

Binary Packages:

- `debian-archive-keyring=2017.7`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2017.7
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2017.7.dsc' debian-archive-keyring_2017.7.dsc 1781 SHA256:58dfdb7c93c72804e43f40fa081e2ab4f895e9ea0a4c2df8f59a1cf26d5fd0e4
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2017.7.tar.xz' debian-archive-keyring_2017.7.tar.xz 79760 SHA256:8a91b68b51faf81fe15599f04af778c1897430cc0a71dae1d6c483e86e7cbcdd
```

Other potentially useful URLs:

- https://sources.debian.net/src/debian-archive-keyring/2017.7/ (for browsing the source)
- https://sources.debian.net/src/debian-archive-keyring/2017.7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debian-archive-keyring/2017.7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debianutils=4.8.6`

Binary Packages:

- `debianutils=4.8.6`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.8.6
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.8.6.dsc' debianutils_4.8.6.dsc 1739 SHA256:1b82e438469d8ffe18a2fc4747f24b8f0475ced12f23d952279579ce6b27b108
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.8.6.tar.xz' debianutils_4.8.6.tar.xz 156532 SHA256:db09047144dadf6a35d0f28977fbef83b0dd60ca32e6c8512cce2444a6423f73
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/4.8.6/ (for browsing the source)
- https://sources.debian.net/src/debianutils/4.8.6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/4.8.6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `diffutils=1:3.6-1`

Binary Packages:

- `diffutils=1:3.6-1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.6-1
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.6-1.dsc' diffutils_3.6-1.dsc 1453 SHA256:26fe7690b45748dc92cee6af224192e78db2ac574e16ae0aeb8ed6a472c883cd
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.6.orig.tar.xz' diffutils_3.6.orig.tar.xz 1398296 SHA256:d621e8bdd4b573918c8145f7ae61817d1be9deb4c8d2328a65cea8e11d783bd6
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.6-1.debian.tar.xz' diffutils_3.6-1.debian.tar.xz 10808 SHA256:f6ab546a134bde18a87ca8e3c98919680e79d81a65a24801ae06ef69b33f24d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.6-1/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dpkg=1.19.0.5`

Binary Packages:

- `dpkg=1.19.0.5+b1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.19.0.5
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.19.0.5.dsc' dpkg_1.19.0.5.dsc 1977 SHA256:e9b38875c17766fd6b55436233dc6c72658d0cd0c2e63b5ec1f1dc3afd8058bb
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.19.0.5.tar.xz' dpkg_1.19.0.5.tar.xz 4557428 SHA256:818046927a7f77c1bcbbad7d8dbc04cdf0f3e6ec4e1a4f9d313378ecc69d85b5
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.19.0.5/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.19.0.5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.19.0.5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.44.4-2`

Binary Packages:

- `e2fsprogs=1.44.4-2`
- `libcom-err2:amd64=1.44.4-2`
- `libext2fs2:amd64=1.44.4-2`
- `libss2:amd64=1.44.4-2`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.44.4-2
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.44.4-2.dsc' e2fsprogs_1.44.4-2.dsc 2494 SHA256:fd92d2d786434c29b07932ca3d4e778345f022aa4221c8c4387744e5723854ac
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.44.4.orig.tar.gz' e2fsprogs_1.44.4.orig.tar.gz 7596925 SHA256:dd707688f0fc353941931c20081f26ec8e54b0bc1ac3f7601f479f9c7675dcb2
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.44.4-2.debian.tar.xz' e2fsprogs_1.44.4-2.debian.tar.xz 80640 SHA256:b72fdfbda6b96338432222d25c9be639e0d800d50533fa345f32789925282d5c
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.44.4-2/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.44.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.44.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `elfutils=0.170-0.5`

Binary Packages:

- `libelf1:amd64=0.170-0.5`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.170-0.5
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.170-0.5.dsc' elfutils_0.170-0.5.dsc 2326 SHA256:cbf2af3a3d8c15152082137c3a7c624358d8a8fc0309075ca35509d7da276158
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.170.orig.tar.bz2' elfutils_0.170.orig.tar.bz2 8358001 SHA256:1f844775576b79bdc9f9c717a50058d08620323c1e935458223a12f249c9e066
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.170-0.5.debian.tar.xz' elfutils_0.170-0.5.debian.tar.xz 45260 SHA256:5e4a997475d568c5bd8bd128d71a277de07e9600fa7437fe2b511ee012e31767
```

Other potentially useful URLs:

- https://sources.debian.net/src/elfutils/0.170-0.5/ (for browsing the source)
- https://sources.debian.net/src/elfutils/0.170-0.5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/elfutils/0.170-0.5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.2.6-1`

Binary Packages:

- `libexpat1:amd64=2.2.6-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.6-1
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.6-1.dsc' expat_2.2.6-1.dsc 1949 SHA256:e14d5e6658592b65821e52371f5036f6a2bdac525ea95014ac99183106917395
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.6.orig.tar.gz' expat_2.2.6.orig.tar.gz 8275473 SHA256:574499cba22a599393e28d99ecfa1e7fc85be7d6651d543045244d5b561cb7ff
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.6-1.debian.tar.xz' expat_2.2.6-1.debian.tar.xz 10688 SHA256:f0bc55f93042b6f517c39b2757021e8f505e19583b1a9d5f11b224825be62037
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.2.6-1/ (for browsing the source)
- https://sources.debian.net/src/expat/2.2.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.2.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.6.0+git+20180808-2`

Binary Packages:

- `findutils=4.6.0+git+20180808-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20180808-2
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20180808-2.dsc' findutils_4.6.0+git+20180808-2.dsc 2137 SHA256:82c5bdd7618af85ec161a0b22297e9b486abf85282abe7e1acf255a254691009
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20180808.orig.tar.xz' findutils_4.6.0+git+20180808.orig.tar.xz 1875160 SHA256:daa434e95aef62a79d6e03cdea901564f01791cff24394285c86f4962b50a979
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20180808-2.debian.tar.xz' findutils_4.6.0+git+20180808-2.debian.tar.xz 26224 SHA256:6dfede94f210c40c46900262a0174c7fecaa79f675b738096543a054802cffdd
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.6.0+git+20180808-2/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.6.0+git+20180808-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.6.0+git+20180808-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-8=8.2.0-4`

Binary Packages:

- `gcc-8-base:amd64=8.2.0-4`
- `libgcc1:amd64=1:8.2.0-4`
- `libstdc++6:amd64=8.2.0-4`

Licenses: (parsed from: `/usr/share/doc/gcc-8-base/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gcc-8/8.2.0-4/


### `dpkg` source package: `gdbm=1.14.1-6`

Binary Packages:

- `libgdbm-compat4:amd64=1.14.1-6+b1`
- `libgdbm5:amd64=1.14.1-6+b1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm5/copyright`)

- `GFDL-1.3+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.14.1-6
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.14.1-6.dsc' gdbm_1.14.1-6.dsc 2293 SHA256:85fc353e81fc54b49d9c13c71f4247836fb1aac2693e98416a6821de8cfe7b41
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.14.1.orig.tar.gz' gdbm_1.14.1.orig.tar.gz 894412 SHA256:cdceff00ffe014495bed3aed71c7910aa88bf29379f795abc0f46d4ee5f8bc5f
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.14.1-6.debian.tar.xz' gdbm_1.14.1-6.debian.tar.xz 27492 SHA256:c9da59f11d5e40ecd877f1256c53ea4750b9d614c7885800e42d0f1885996658
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdbm/1.14.1-6/ (for browsing the source)
- https://sources.debian.net/src/gdbm/1.14.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdbm/1.14.1-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.18.0-1`

Binary Packages:

- `git=1:2.18.0-1`
- `git-man=1:2.18.0-1`

Licenses: (parsed from: `/usr/share/doc/git/copyright`, `/usr/share/doc/git-man/copyright`)

- `Apache-2.0`
- `Artistic`
- `Artistic-1`
- `BSD-2-clause`
- `Boost`
- `EDL-1.0`
- `Expat`
- `GPL`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `dlmalloc`
- `mingw-runtime`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/git/1:2.18.0-1/


### `dpkg` source package: `glibc=2.27-5`

Binary Packages:

- `libc-bin=2.27-5`
- `libc6:amd64=2.27-5`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.27-5
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.27-5.dsc' glibc_2.27-5.dsc 8914 SHA256:7a2c8ed68349983a426a225b2ffb99e6ff609d97e441396c548ec1011b5a8827
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.27.orig.tar.xz' glibc_2.27.orig.tar.xz 15923832 SHA256:0e9826488e3ffedb4d14a426d741b7b1cf15f6973ab30762af9a188ad47633ed
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.27-5.debian.tar.xz' glibc_2.27-5.debian.tar.xz 1011540 SHA256:581372782407c4b138b9bf8c45d29f7513802b3a2e6bf544ea6aa8786081bca2
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.27-5/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.27-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.27-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.1.2+dfsg-3`

Binary Packages:

- `libgmp10:amd64=2:6.1.2+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.2+dfsg-3
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg-3.dsc' gmp_6.1.2+dfsg-3.dsc 2123 SHA256:1c918d2bf8a4fce98fc6bdcd752b36e1cd897114b9b9aeaf5dc661200bbcf9e2
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg.orig.tar.xz' gmp_6.1.2+dfsg.orig.tar.xz 1804424 SHA256:18016f718f621e7641ddd4e57f8e140391c5183252e5998263ffff59198a65b7
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg-3.debian.tar.xz' gmp_6.1.2+dfsg-3.debian.tar.xz 20824 SHA256:8c61aa9fcc1c90052c53bd723b1391acb4c9032bf90fcce27c6facfd8065bf5a
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.1.2+dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.1.2+dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.1.2+dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.10-1`

Binary Packages:

- `dirmngr=2.2.10-1`
- `gnupg=2.2.10-1`
- `gnupg-l10n=2.2.10-1`
- `gnupg-utils=2.2.10-1`
- `gpg=2.2.10-1`
- `gpg-agent=2.2.10-1`
- `gpg-wks-client=2.2.10-1`
- `gpg-wks-server=2.2.10-1`
- `gpgconf=2.2.10-1`
- `gpgsm=2.2.10-1`
- `gpgv=2.2.10-1`

Licenses: (parsed from: `/usr/share/doc/dirmngr/copyright`, `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gnupg-l10n/copyright`, `/usr/share/doc/gnupg-utils/copyright`, `/usr/share/doc/gpg/copyright`, `/usr/share/doc/gpg-agent/copyright`, `/usr/share/doc/gpg-wks-client/copyright`, `/usr/share/doc/gpg-wks-server/copyright`, `/usr/share/doc/gpgconf/copyright`, `/usr/share/doc/gpgsm/copyright`, `/usr/share/doc/gpgv/copyright`)

- `BSD-3-clause`
- `CC0-1.0`
- `Expat`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `RFC-Reference`
- `TinySCHEME`
- `permissive`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gnupg2/2.2.10-1/


### `dpkg` source package: `gnutls28=3.5.19-1`

Binary Packages:

- `libgnutls30:amd64=3.5.19-1`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `CC0 license`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `LGPL`
- `LGPL-3`
- `LGPL2.1`
- `The MIT License (MIT)`
- `The main library is licensed under GNU Lesser`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.5.19-1
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.19-1.dsc' gnutls28_3.5.19-1.dsc 3319 SHA256:2ff29427310d35523198e1c75e24128bf7abb514dd6dbb3e8f90a4b2f2b428d7
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.19.orig.tar.xz' gnutls28_3.5.19.orig.tar.xz 7239744 SHA256:1936eb64f03aaefd6eb16cef0567457777618573826b94d03376bb6a4afadc44
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.19.orig.tar.xz.asc' gnutls28_3.5.19.orig.tar.xz.asc 534 SHA256:8d46b9f0275f71d9c723523cbd9f59d245576df750cd219bc883455a9fc8cad6
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.19-1.debian.tar.xz' gnutls28_3.5.19-1.debian.tar.xz 60732 SHA256:3113ac77e75196fb173214d05510ff8f1dc954bc33d271a36f3cae7f31ce3e87
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.5.19-1/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.5.19-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.5.19-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=3.1-2`

Binary Packages:

- `grep=3.1-2`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.1-2
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.1-2.dsc' grep_3.1-2.dsc 2046 SHA256:b75ef8eb1399a49274bafe972679680b7add1500a4ee82eedaa0372f8ed744a0
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.1.orig.tar.xz' grep_3.1.orig.tar.xz 1370880 SHA256:db625c7ab3bb3ee757b3926a5cfa8d9e1c3991ad24707a83dde8a5ef2bf7a07e
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.1-2.debian.tar.bz2' grep_3.1-2.debian.tar.bz2 110067 SHA256:f09ce7a3c860a5de8939ebceb5fcd85d00d1537ad9f998dae5f623d9bcfe4e40
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/3.1-2/ (for browsing the source)
- https://sources.debian.net/src/grep/3.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/3.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gzip=1.9-2`

Binary Packages:

- `gzip=1.9-2`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.9-2
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.9-2.dsc' gzip_1.9-2.dsc 1879 SHA256:dadbf2ac52814fc8ecdd15ea2aca2f283c829cbf9144915666e715a0ed1c7fd5
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.9.orig.tar.gz' gzip_1.9.orig.tar.gz 1181937 SHA256:5d2d3a3432ef32f24cdb060d278834507b481a75adeca18850c73592f778f6ad
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.9-2.debian.tar.xz' gzip_1.9-2.debian.tar.xz 11684 SHA256:f431951eecbd5aa6b3a42b2fa490ad9a64a95dc9badc2522265efa9da6542dcb
```

Other potentially useful URLs:

- https://sources.debian.net/src/gzip/1.9-2/ (for browsing the source)
- https://sources.debian.net/src/gzip/1.9-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gzip/1.9-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hostname=3.20`

Binary Packages:

- `hostname=3.20`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/hostname/3.20/


### `dpkg` source package: `init-system-helpers=1.54`

Binary Packages:

- `init-system-helpers=1.54`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.54
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.54.dsc' init-system-helpers_1.54.dsc 2047 SHA256:5a648b6e85b64f4d353fc9f66a00bf31a2aa926f91ed6eecdb11a5e4ea464e5e
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.54.tar.xz' init-system-helpers_1.54.tar.xz 39848 SHA256:cce29b4889393ce9b614898bb423b2fd6fca79784c103990681947260cdc357a
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.54/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.54/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.54/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iproute2=4.17.0-2`

Binary Packages:

- `iproute2=4.17.0-2`

Licenses: (parsed from: `/usr/share/doc/iproute2/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/iproute2/4.17.0-2/


### `dpkg` source package: `iptables=1.6.2-1.1`

Binary Packages:

- `libxtables12:amd64=1.6.2-1.1`

Licenses: (parsed from: `/usr/share/doc/libxtables12/copyright`)

- `Artistic-2`
- `GPL-2`
- `GPL-2+`
- `custom`

Source:

```console
$ apt-get source -qq --print-uris iptables=1.6.2-1.1
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.6.2-1.1.dsc' iptables_1.6.2-1.1.dsc 2791 SHA256:d1e8a317abc6d3a9ecf3a87a6da251b5e585961e2e8363f316e72f9f3d41be0d
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.6.2.orig.tar.bz2' iptables_1.6.2.orig.tar.bz2 639785 SHA256:55d02dfa46263343a401f297d44190f2a3e5113c8933946f094ed40237053733
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.6.2-1.1.debian.tar.xz' iptables_1.6.2-1.1.debian.tar.xz 61192 SHA256:410b999709db3d319dcfa882adbc40c7b1cfe243ac9fa1527c3e24b60a02822f
```

Other potentially useful URLs:

- https://sources.debian.net/src/iptables/1.6.2-1.1/ (for browsing the source)
- https://sources.debian.net/src/iptables/1.6.2-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iptables/1.6.2-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iputils=3:20180629-2`

Binary Packages:

- `iputils-ping=3:20180629-2`

Licenses: (parsed from: `/usr/share/doc/iputils-ping/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris iputils=3:20180629-2
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20180629-2.dsc' iputils_20180629-2.dsc 2093 SHA256:c377186ea16ebeb404316f562857e2564e3346b7b0cfd9ef72d88498db6bf3b0
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20180629.orig.tar.bz2' iputils_20180629.orig.tar.bz2 157943 SHA256:1a54fe72d67ac00dae328ddb1952110ee5310ccecbfcb97cbb26d4dedc73fe6d
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20180629-2.debian.tar.xz' iputils_20180629-2.debian.tar.xz 10212 SHA256:bccf6d3819bbcea59ecade34872fb44f30495baa4878cc32b2ec32b973a7ac58
```

Other potentially useful URLs:

- https://sources.debian.net/src/iputils/3:20180629-2/ (for browsing the source)
- https://sources.debian.net/src/iputils/3:20180629-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iputils/3:20180629-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `keyutils=1.5.9-9.3`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-9.3`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-9.3
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-9.3.dsc' keyutils_1.5.9-9.3.dsc 2093 SHA256:65c003c2e0796a14f7dac94a3f3c8676e8a00a0c393136ae29a1e563a1aa5f42
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-9.3.debian.tar.xz' keyutils_1.5.9-9.3.debian.tar.xz 18236 SHA256:2d4d01cb07ac113341b33190a1eba6524768f575ea0c7309daa656a1f1305ac2
```

Other potentially useful URLs:

- https://sources.debian.net/src/keyutils/1.5.9-9.3/ (for browsing the source)
- https://sources.debian.net/src/keyutils/1.5.9-9.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/keyutils/1.5.9-9.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `krb5=1.16-2`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.16-2`
- `libk5crypto3:amd64=1.16-2`
- `libkrb5-3:amd64=1.16-2`
- `libkrb5support0:amd64=1.16-2`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.16-2
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.16-2.dsc' krb5_1.16-2.dsc 3358 SHA256:b854c4994e9f45b4e99498e5b8fbdda6ec4f5c06f697a7cfce3ab2a89cc8e60f
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.16.orig.tar.gz' krb5_1.16.orig.tar.gz 9474479 SHA256:faeb125f83b0fb4cdb2f99f088140631bb47d975982de0956d18c85842969e08
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.16-2.debian.tar.xz' krb5_1.16-2.debian.tar.xz 96272 SHA256:96c43881a8503b01c5025a4855de9261d0633200e15627d74f9717a0f971ac6c
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.16-2/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.16-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.16-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libassuan=2.5.1-2`

Binary Packages:

- `libassuan0:amd64=2.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libassuan0/copyright`)

- `GAP`
- `GAP~FSF`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with libtool exception`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libassuan=2.5.1-2
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.1-2.dsc' libassuan_2.5.1-2.dsc 2215 SHA256:e954a7ef30815e62832ca4a1d2959142e264795e7ec78ba369752353135beb68
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.1.orig.tar.bz2' libassuan_2.5.1.orig.tar.bz2 564857 SHA256:47f96c37b4f2aac289f0bc1bacfa8bd8b4b209a488d3d15e2229cb6cc9b26449
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.1-2.debian.tar.xz' libassuan_2.5.1-2.debian.tar.xz 15236 SHA256:4a67901dcb0e92cd40e0d5d7148ebe6f929378671df373eb68b48acb560d641f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.5.1-2/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.5.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.5.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.9.1-1`

Binary Packages:

- `libbsd0:amd64=0.9.1-1`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-John-Birrell`
- `BSD-3-clause-Regents`
- `BSD-3-clause-author`
- `BSD-4-clause-Christopher-G-Demetriou`
- `BSD-4-clause-Niels-Provos`
- `BSD-5-clause-Peter-Wemm`
- `Beerware`
- `Expat`
- `ISC`
- `ISC-Original`
- `public-domain`
- `public-domain-Colin-Plumb`

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.9.1-1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.9.1-1.dsc' libbsd_0.9.1-1.dsc 2181 SHA256:3082adfec10879cc623b8f714d16ba4b4533705f015bf96c971134c7896bd558
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.9.1.orig.tar.xz' libbsd_0.9.1.orig.tar.xz 387180 SHA256:56d835742327d69faccd16955a60b6dcf30684a8da518c4eca0ac713b9e0a7a4
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.9.1.orig.tar.xz.asc' libbsd_0.9.1.orig.tar.xz.asc 833 SHA256:a34a81f40bfef37242943cb1c4c446e75d57f31be3317c887d8a5f2cbfb5577d
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.9.1-1.debian.tar.xz' libbsd_0.9.1-1.debian.tar.xz 16372 SHA256:f71467eada3bca5bd3ba517dc69372ebc76df224b0e7ebc1761a856637c48c44
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.9.1-1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.9.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.9.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.7.9-1`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-1
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9-1.dsc' libcap-ng_0.7.9-1.dsc 1912 SHA256:99dbd0e464b4a8b60ba2afc03b5a8f96827ef51b334afffbfa96a9845c2e8346
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA256:4a1532bcf3731aade40936f6d6a586ed5a66ca4c7455e1338d1f6c3e09221328
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9-1.debian.tar.xz' libcap-ng_0.7.9-1.debian.tar.xz 5636 SHA256:fb67bc2baaa37e72767d5719917ac8087c6418a3469310b0f1f19d4d9a1a253c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap-ng/0.7.9-1/ (for browsing the source)
- https://sources.debian.net/src/libcap-ng/0.7.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap-ng/0.7.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap2=1:2.25-1.2`

Binary Packages:

- `libcap2:amd64=1:2.25-1.2`
- `libcap2-bin=1:2.25-1.2`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.25-1.2
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.25-1.2.dsc' libcap2_2.25-1.2.dsc 2230 SHA256:a492c5c61703dcd80e19ff408d8562671fbfe0a03dd93c3570ddf214ac06752b
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.25.orig.tar.xz' libcap2_2.25.orig.tar.xz 63672 SHA256:693c8ac51e983ee678205571ef272439d83afe62dd8e424ea14ad9790bc35162
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.25-1.2.debian.tar.xz' libcap2_2.25-1.2.debian.tar.xz 20912 SHA256:0088bcf76d6cdf1c242431b3b97e91e50120cc2fc2b938dbeb3606dece7d9870
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap2/1:2.25-1.2/ (for browsing the source)
- https://sources.debian.net/src/libcap2/1:2.25-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap2/1:2.25-1.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libedit=3.1-20180525-1`

Binary Packages:

- `libedit2:amd64=3.1-20180525-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20180525-1
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20180525-1.dsc' libedit_3.1-20180525-1.dsc 2219 SHA256:0680d068bbbad63ddbaaded2ea713f6807eec601715f7ddabbe9fb4b7aed5b9b
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20180525.orig.tar.gz' libedit_3.1-20180525.orig.tar.gz 521999 SHA256:c41bea8fd140fb57ba67a98ec1d8ae0b8ffa82f4aba9c35a87e5a9499e653116
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20180525-1.debian.tar.bz2' libedit_3.1-20180525-1.debian.tar.bz2 11444 SHA256:2bd107dbd9aff59d28314a55bbb74edbfd1eb969450223ca87127203ab001454
```

Other potentially useful URLs:

- https://sources.debian.net/src/libedit/3.1-20180525-1/ (for browsing the source)
- https://sources.debian.net/src/libedit/3.1-20180525-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libedit/3.1-20180525-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liberror-perl=0.17026-1`

Binary Packages:

- `liberror-perl=0.17026-1`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17026-1
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17026-1.dsc' liberror-perl_0.17026-1.dsc 2209 SHA256:6fe4e58ee63353bc35ad95bd7642f3c0ca07248221a69bcedb36a1592a4f285e
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17026.orig.tar.gz' liberror-perl_0.17026.orig.tar.gz 32988 SHA256:37590a962cd73ae03470e1ff16459a6cbc5273fc57626b8981dab9c2433155d9
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17026-1.debian.tar.xz' liberror-perl_0.17026-1.debian.tar.xz 4216 SHA256:45583961ac80fb63b8766b3c7d4157a9bb424e0cf25bc407b290b06f402324b4
```

Other potentially useful URLs:

- https://sources.debian.net/src/liberror-perl/0.17026-1/ (for browsing the source)
- https://sources.debian.net/src/liberror-perl/0.17026-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liberror-perl/0.17026-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.2.1-8`

Binary Packages:

- `libffi6:amd64=3.2.1-8`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-8
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1-8.dsc' libffi_3.2.1-8.dsc 1959 SHA256:a07201eb5374cfab35703a6f4c88a494bb23ece91da5481497bc25404c57eaf4
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1-8.debian.tar.xz' libffi_3.2.1-8.debian.tar.xz 11660 SHA256:1eb0b13e0c0fc989ed98011d18dcddf8a05af17380fe1258883761a8d16586b4
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.2.1-8/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.2.1-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.2.1-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.8.3-1`

Binary Packages:

- `libgcrypt20:amd64=1.8.3-1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.3-1
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.3-1.dsc' libgcrypt20_1.8.3-1.dsc 2863 SHA256:5ee11668e4deca5092c6f853a1ee82e8796415bd394cc63be429496640aa3b58
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.3.orig.tar.bz2' libgcrypt20_1.8.3.orig.tar.bz2 2989166 SHA256:66ec90be036747602f2b48f98312361a9180c97c68a690a5f376fa0f67d0af7c
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.3.orig.tar.bz2.asc' libgcrypt20_1.8.3.orig.tar.bz2.asc 534 SHA256:f3e70e2988f223dc2ac70ff51323fd8a99a5e32b9cc24ef193d347892c559f2c
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.3-1.debian.tar.xz' libgcrypt20_1.8.3-1.debian.tar.xz 28816 SHA256:46d0cf2e42621b8a9eee67d6f2249ea8efea33daa5a2411d15adca5cc4042933
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.8.3-1/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.8.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.8.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.32-1`

Binary Packages:

- `libgpg-error0:amd64=1.32-1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.32-1
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.32-1.dsc' libgpg-error_1.32-1.dsc 2060 SHA256:9f37f813495743bd528080ac9a4182ba36873bd1efbb4944bbe187637f02978e
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.32.orig.tar.bz2' libgpg-error_1.32.orig.tar.bz2 904382 SHA256:c345c5e73cc2332f8d50db84a2280abfb1d8f6d4f1858b9daa30404db44540ca
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.32.orig.tar.bz2.asc' libgpg-error_1.32.orig.tar.bz2.asc 534 SHA256:dbf20a0c4bbc4fccfe070c55959739e5bf4d1bec01f3c3cd46e262003685b466
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.32-1.debian.tar.xz' libgpg-error_1.32-1.debian.tar.xz 15296 SHA256:9c326726a4d979f6249d68c9a2b1cc1157eefd7c95b4d49c011e66dcd54ee3b0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.32-1/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.32-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.32-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn2=2.0.4-2.2`

Binary Packages:

- `libidn2-0:amd64=2.0.4-2.2`

Licenses: (parsed from: `/usr/share/doc/libidn2-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `Unicode`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libidn2/2.0.4-2.2/


### `dpkg` source package: `libksba=1.3.5-2`

Binary Packages:

- `libksba8:amd64=1.3.5-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.3.5-2
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.3.5-2.dsc' libksba_1.3.5-2.dsc 2526 SHA256:4fd08fd129f97ab1df86c220b88b7b2c6e4e04aa90bfd3ae364d18022256bef8
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2' libksba_1.3.5.orig.tar.bz2 620649 SHA256:41444fd7a6ff73a79ad9728f985e71c9ba8cd3e5e53358e70d5f066d35c1a340
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2.asc' libksba_1.3.5.orig.tar.bz2.asc 287 SHA256:a954b03144ee882c838853da24fd7b6868b78df72a18c71079217d968698a76f
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.3.5-2.debian.tar.xz' libksba_1.3.5-2.debian.tar.xz 13852 SHA256:98c985bff973be1aecc702fa15887ff1e5b8de481d1dc3e99423a587754eaabd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libksba/1.3.5-2/ (for browsing the source)
- https://sources.debian.net/src/libksba/1.3.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libksba/1.3.5-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmnl=1.0.4-2`

Binary Packages:

- `libmnl0:amd64=1.0.4-2`

Licenses: (parsed from: `/usr/share/doc/libmnl0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libmnl=1.0.4-2
'http://deb.debian.org/debian/pool/main/libm/libmnl/libmnl_1.0.4-2.dsc' libmnl_1.0.4-2.dsc 1994 SHA256:131106bb7eb4a94fa8e8c135f92c38068d0b42681f166eb159137f171c568630
'http://deb.debian.org/debian/pool/main/libm/libmnl/libmnl_1.0.4.orig.tar.bz2' libmnl_1.0.4.orig.tar.bz2 301270 SHA256:171f89699f286a5854b72b91d06e8f8e3683064c5901fb09d954a9ab6f551f81
'http://deb.debian.org/debian/pool/main/libm/libmnl/libmnl_1.0.4-2.debian.tar.xz' libmnl_1.0.4-2.debian.tar.xz 7512 SHA256:208d62777081ffe6d7dffde0d7370cefb03fe0a6a0486a1b50f6b7b8e9a5b068
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmnl/1.0.4-2/ (for browsing the source)
- https://sources.debian.net/src/libmnl/1.0.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmnl/1.0.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpsl=0.20.2-1`

Binary Packages:

- `libpsl5:amd64=0.20.2-1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.20.2-1
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.20.2-1.dsc' libpsl_0.20.2-1.dsc 1632 SHA256:6476accfce8dbaa9bbc1f4a8a8e2dcfc6c5f79b8e5f49f05678bdd541d087718
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.20.2.orig.tar.gz' libpsl_0.20.2.orig.tar.gz 8590430 SHA256:94d2b5e00e9aa761ae7efbaa67edc00d5298487ed9706eb4789e349012993c31
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.20.2-1.debian.tar.xz' libpsl_0.20.2-1.debian.tar.xz 9852 SHA256:e271054b304ea1b6f00bff46d4be75809a5b1427d99f2797d8aa856c8e12d91c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpsl/0.20.2-1/ (for browsing the source)
- https://sources.debian.net/src/libpsl/0.20.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpsl/0.20.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libseccomp=2.3.3-3`

Binary Packages:

- `libseccomp2:amd64=2.3.3-3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.3.3-3
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.3.3-3.dsc' libseccomp_2.3.3-3.dsc 2415 SHA256:2627e4d5c7386d839e7310d6aaf57292fedae5a9b123592a2550d6b88f884f8f
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.3.3.orig.tar.gz' libseccomp_2.3.3.orig.tar.gz 564546 SHA256:7fc28f4294cc72e61c529bedf97e705c3acf9c479a8f1a3028d4cd2ca9f3b155
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.3.3-3.debian.tar.xz' libseccomp_2.3.3-3.debian.tar.xz 11860 SHA256:46f218c83627571e7c28edcc351b15ad4a783f0cf92ca8a85f28e7dccaed6c22
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.3.3-3/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.3.3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.3.3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=2.8-1`

Binary Packages:

- `libselinux1:amd64=2.8-1+b1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.8-1
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.8-1.dsc' libselinux_2.8-1.dsc 2347 SHA256:0f08d64f4488312a8e8b7ffb12771cd385560752473a2e585449edc27223c129
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.8.orig.tar.gz' libselinux_2.8.orig.tar.gz 187759 SHA256:31db96ec7643ce10912b3c3f98506a08a9116dcfe151855fd349c3fda96187e1
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.8-1.debian.tar.xz' libselinux_2.8-1.debian.tar.xz 23052 SHA256:a0b150e870a3da7e1d7b0fec7c1a5ae6988a0985e545c69cfe8fe05363c5bf64
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/2.8-1/ (for browsing the source)
- https://sources.debian.net/src/libselinux/2.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/2.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=2.8-1`

Binary Packages:

- `libsemanage-common=2.8-1`
- `libsemanage1:amd64=2.8-1+b1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.8-1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.8-1.dsc' libsemanage_2.8-1.dsc 2434 SHA256:2e32bce21b51dd850ab11b10d59af5b781afdd4932b85c55b9fc27a3a3143757
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.8.orig.tar.gz' libsemanage_2.8.orig.tar.gz 154200 SHA256:1c0de8d2c51e5460926c21e371105c84a39087dfd8f8e9f0cc1d017e4cbea8e2
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.8-1.debian.tar.xz' libsemanage_2.8-1.debian.tar.xz 16964 SHA256:981fc945171e61c18af2e57a501cb1f26886b25a21daf3d8f9e1e25ddf07b722
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/2.8-1/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/2.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/2.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=2.8-1`

Binary Packages:

- `libsepol1:amd64=2.8-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.8-1
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.8-1.dsc' libsepol_2.8-1.dsc 1792 SHA256:37b0b79ab0f7533c194272809ccb3f3c5ff788536f66254c0d405e2e8b2b270e
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.8.orig.tar.gz' libsepol_2.8.orig.tar.gz 473384 SHA256:3ad6916a8352bef0bad49acc8037a5f5b48c56f94e4cb4e1959ca475fa9d24d6
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.8-1.debian.tar.xz' libsepol_2.8-1.debian.tar.xz 14076 SHA256:7b8d0b47396c96830754db2e5b679d294486aeffd93cfd21ac68202031374a00
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/2.8-1/ (for browsing the source)
- https://sources.debian.net/src/libsepol/2.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/2.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libssh2=1.8.0-2`

Binary Packages:

- `libssh2-1:amd64=1.8.0-2`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.8.0-2
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.8.0-2.dsc' libssh2_1.8.0-2.dsc 1447 SHA256:a3ab2120a472d0a886114ca62b44186550c060c82124616326ca8da11b2e8c7d
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.8.0.orig.tar.gz' libssh2_1.8.0.orig.tar.gz 846989 SHA256:4382d33de790b28f862e53ed59ffbd65f3def7a06e8b6e9ca1b6f70453b4d5e0
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.8.0-2.debian.tar.xz' libssh2_1.8.0-2.debian.tar.xz 7460 SHA256:2c9c438e77ed1bc84f4fc130a8018e935862a251b01749c8b79d89df655b5480
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh2/1.8.0-2/ (for browsing the source)
- https://sources.debian.net/src/libssh2/1.8.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh2/1.8.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.13-3`

Binary Packages:

- `libtasn1-6:amd64=4.13-3`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.13-3
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.13-3.dsc' libtasn1-6_4.13-3.dsc 2574 SHA256:15a984daba0bc64819a1203cd28a1e869a30e0edde227237e4cdcfbc86131227
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz' libtasn1-6_4.13.orig.tar.gz 1891703 SHA256:7e528e8c317ddd156230c4e31d082cd13e7ddeb7a54824be82632209550c8cca
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz.asc' libtasn1-6_4.13.orig.tar.gz.asc 774 SHA256:90261376528edf44831d1369847088cc2fb48669860d343961daca42e674b226
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.13-3.debian.tar.xz' libtasn1-6_4.13-3.debian.tar.xz 63384 SHA256:1428c31d3d900d8fa1946fc29d9d2839c73c7a4c0ebff7a2571c134aef53c310
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.13-3/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.13-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.13-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=0.9.10-1`

Binary Packages:

- `libunistring2:amd64=0.9.10-1`

Licenses: (parsed from: `/usr/share/doc/libunistring2/copyright`)

- `FreeSoftware`
- `GFDL-1.2`
- `GFDL-1.2+`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with distribution exception`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libunistring=0.9.10-1
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-1.dsc' libunistring_0.9.10-1.dsc 2206 SHA256:2118b96b1125399556bd95b8917cd559c4e9afe8d85861b01435f9635cefcdf2
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA256:eb8fb2c3e4b6e2d336608377050892b54c3c983b646c561836550863003c05d7
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA256:e1606f691034fa21b00e08269622743547c16d21cca6c8a64156b4774a49e78e
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-1.debian.tar.xz' libunistring_0.9.10-1.debian.tar.xz 40328 SHA256:dd4d07437e6332003e702aa2f56911a21091ac6f10d0cdc17aaaaa8e29ad63b7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/0.9.10-1/ (for browsing the source)
- https://sources.debian.net/src/libunistring/0.9.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/0.9.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzstd=1.3.5+dfsg-1`

Binary Packages:

- `libzstd1:amd64=1.3.5+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.3.5+dfsg-1
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.3.5+dfsg-1.dsc' libzstd_1.3.5+dfsg-1.dsc 2155 SHA256:a53d833a1b5c8412e30575452dbfc7c5e9ea85934557413f24d5ac9842c2f1db
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.3.5+dfsg.orig.tar.xz' libzstd_1.3.5+dfsg.orig.tar.xz 1185104 SHA256:c7517111ed4d4f1a6982ef8064dc311d9ff62a2f58059cae1a8ffa9743fafccd
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.3.5+dfsg-1.debian.tar.xz' libzstd_1.3.5+dfsg-1.debian.tar.xz 9940 SHA256:5217f4e433b5786363874a8c871373f761860fac04cf3a9cbbde0671fc5d603c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.3.5+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.3.5+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.3.5+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lsb=9.20170808`

Binary Packages:

- `lsb-base=9.20170808`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=9.20170808
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_9.20170808.dsc' lsb_9.20170808.dsc 1597 SHA256:d767e622530f73df4f041f7bace54412a6da3d66ddcc73df7913cdebdbf258a9
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_9.20170808.tar.xz' lsb_9.20170808.tar.xz 42120 SHA256:ec9cb022cedcdf34c5b8dc2dca530777ce3f491ad364222557691e87807729b1
```

Other potentially useful URLs:

- https://sources.debian.net/src/lsb/9.20170808/ (for browsing the source)
- https://sources.debian.net/src/lsb/9.20170808/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lsb/9.20170808/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lz4=1.8.2-1`

Binary Packages:

- `liblz4-1:amd64=1.8.2-1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.8.2-1
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.8.2-1.dsc' lz4_1.8.2-1.dsc 1932 SHA256:6a1c72b10315b91bf0a7ccd48097feb621f04a5c795b66d7d35fe05fc9d0b908
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.8.2.orig.tar.gz' lz4_1.8.2.orig.tar.gz 320742 SHA256:0963fbe9ee90acd1d15e9f09e826eaaf8ea0312e854803caf2db0a6dd40f4464
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.8.2-1.debian.tar.xz' lz4_1.8.2-1.debian.tar.xz 10948 SHA256:c3635bbb067b8544b29057dfc39d9f884ce06fd95afcf579d9b9f912a2765be4
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/1.8.2-1/ (for browsing the source)
- https://sources.debian.net/src/lz4/1.8.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/1.8.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mawk=1.3.3-17`

Binary Packages:

- `mawk=1.3.3-17+b3`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.3-17
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3-17.dsc' mawk_1.3.3-17.dsc 1801 SHA256:f98ce6e153e8ac1faf8165bbf77447a4279313f1c18f6bfeec0c5ce35e4b9c03
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3.orig.tar.gz' mawk_1.3.3.orig.tar.gz 209942 SHA256:32649c46063d4ef0777a12ae6e9a26bcc920833d54e1abca7edb8d37481e7485
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3-17.diff.gz' mawk_1.3.3-17.diff.gz 63506 SHA256:13cb66b6eb5ee654d5626621d5ef476ede6b0bebac18ce765516de810e58490c
```

Other potentially useful URLs:

- https://sources.debian.net/src/mawk/1.3.3-17/ (for browsing the source)
- https://sources.debian.net/src/mawk/1.3.3-17/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mawk/1.3.3-17/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mercurial=4.7-1`

Binary Packages:

- `mercurial=4.7-1`
- `mercurial-common=4.7-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/mercurial/4.7-1/


### `dpkg` source package: `mime-support=3.61`

Binary Packages:

- `mime-support=3.61`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.61
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.61.dsc' mime-support_3.61.dsc 1588 SHA256:a96dc8d9e5ac4e7b58b666606373b6fa9dde9c07eb049bb141d9c185dac50b80
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.61.tar.gz' mime-support_3.61.tar.gz 36436 SHA256:027fa5b709b3dabfb8dcdf68ab8c59e1f534a37eb1d1b5160ee1fd788103131d
```

Other potentially useful URLs:

- https://sources.debian.net/src/mime-support/3.61/ (for browsing the source)
- https://sources.debian.net/src/mime-support/3.61/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mime-support/3.61/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.1+20180714-1`

Binary Packages:

- `libncurses6:amd64=6.1+20180714-1`
- `libncursesw6:amd64=6.1+20180714-1`
- `libtinfo6:amd64=6.1+20180714-1`
- `ncurses-base=6.1+20180714-1`
- `ncurses-bin=6.1+20180714-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.1+20180714-1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20180714-1.dsc' ncurses_6.1+20180714-1.dsc 4147 SHA256:d4ee01fcada6e29bba632598e517fff5c48329c4191712f07311e3a21d36d4b9
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20180714.orig.tar.gz' ncurses_6.1+20180714.orig.tar.gz 3400860 SHA256:8e2d9ab51c54d5a5b78ca6d8e63200646202e91b152d9ea8ddbce86e6a32796d
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20180714.orig.tar.gz.asc' ncurses_6.1+20180714.orig.tar.gz.asc 251 SHA256:682fbba42d188d489b1cd457cce1285f0d9356fe8c45fdcd6e1c45e81e22d352
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20180714-1.debian.tar.xz' ncurses_6.1+20180714-1.debian.tar.xz 59968 SHA256:4160bcdae8e616c584317ae46ec8053709a4e640f9620621644f986c1b7e402f
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.1+20180714-1/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.1+20180714-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.1+20180714-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `netbase=5.4`

Binary Packages:

- `netbase=5.4`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=5.4
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.4.dsc' netbase_5.4.dsc 1326 SHA256:ebe29d45e65b661d64636cbce3840997d8079cf338efbfa347b4c73ed2831b7b
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.4.tar.xz' netbase_5.4.tar.xz 31524 SHA256:66ff73d2d162e2d49db43988d8b8cd328cf7fffca042db73397f14c71825e80d
```

Other potentially useful URLs:

- https://sources.debian.net/src/netbase/5.4/ (for browsing the source)
- https://sources.debian.net/src/netbase/5.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/netbase/5.4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=3.4-1`

Binary Packages:

- `libhogweed4:amd64=3.4-1`
- `libnettle6:amd64=3.4-1`

Licenses: (parsed from: `/usr/share/doc/libhogweed4/copyright`, `/usr/share/doc/libnettle6/copyright`)

- `GAP`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1+`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nettle=3.4-1
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.4-1.dsc' nettle_3.4-1.dsc 2238 SHA256:0ceb4600fdedf43916e95fb6b354ebb4038f00f5814433582d0481b510310e86
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.4.orig.tar.gz' nettle_3.4.orig.tar.gz 1935069 SHA256:ae7a42df026550b85daca8389b6a60ba6313b0567f374392e54918588a411e94
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.4.orig.tar.gz.asc' nettle_3.4.orig.tar.gz.asc 1238 SHA256:86d7441c7334dd95d16b1ca488fd94ec45ed6406714d4ed9887c7212e337eb2a
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.4-1.debian.tar.xz' nettle_3.4-1.debian.tar.xz 19884 SHA256:9bfc25562ed36449e75741b0473e0e558bc9ef5c20ca24e7c650fea87d631c03
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.4-1/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nghttp2=1.32.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.32.0-1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `SIL-OFL-1.1`
- `all-permissive`

Source:

```console
$ apt-get source -qq --print-uris nghttp2=1.32.0-1
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.32.0-1.dsc' nghttp2_1.32.0-1.dsc 2278 SHA256:8b4743acd51dd5609082d5e1f8f4a8dd744e11084858d5467e59b5460cabd126
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.32.0.orig.tar.bz2' nghttp2_1.32.0.orig.tar.bz2 1841198 SHA256:0660816fa83494471d7bff3c556d5a7c2ff07fb6ffa6b2d06bdbdb45ee6a964a
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.32.0-1.debian.tar.xz' nghttp2_1.32.0-1.debian.tar.xz 12444 SHA256:e4ce3e1115fb20b57d98e9dd1a6cdf25b5c0927d5cd27d1eb27538fad5a8b5d6
```

Other potentially useful URLs:

- https://sources.debian.net/src/nghttp2/1.32.0-1/ (for browsing the source)
- https://sources.debian.net/src/nghttp2/1.32.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nghttp2/1.32.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `npth=1.6-1`

Binary Packages:

- `libnpth0:amd64=1.6-1`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-1
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.6-1.dsc' npth_1.6-1.dsc 1925 SHA256:2c327ce494f702482e79ed620445cba303c4449dd0768fecee3ee7d5ade2544a
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA256:1393abd9adcf0762d34798dc34fdcf4d0d22a8410721e76f1e3afcd1daa4e2d1
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.6-1.debian.tar.xz' npth_1.6-1.debian.tar.xz 10532 SHA256:d312d4a3cf1d082e2f2cf3ea752c41d34f7e120f77a941c6c1680e6093834353
```

Other potentially useful URLs:

- https://sources.debian.net/src/npth/1.6-1/ (for browsing the source)
- https://sources.debian.net/src/npth/1.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/npth/1.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.4.46+dfsg-5`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.46+dfsg-5`
- `libldap-common=2.4.46+dfsg-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.46+dfsg-5
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.46+dfsg-5.dsc' openldap_2.4.46+dfsg-5.dsc 2711 SHA256:61354bc5ee694d39ad1046deb2aa3145cb52945ad6a0b26ce2837a0e2096a2af
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.46+dfsg.orig.tar.gz' openldap_2.4.46+dfsg.orig.tar.gz 4873832 SHA256:e93cb511f6bce162c27502d0d240e6410a8f14e72c47ddddb4e69b25b7c538e4
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.46+dfsg-5.debian.tar.xz' openldap_2.4.46+dfsg-5.debian.tar.xz 163000 SHA256:f07814e83627de02011f175d698e104bdd369b070d0a65f5db2a007c35a58232
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.46+dfsg-5/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.46+dfsg-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.46+dfsg-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:7.8p1-1`

Binary Packages:

- `openssh-client=1:7.8p1-1`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Beer-ware`
- `Expat-with-advertising-restriction`
- `Mazieres-BSD-style`
- `OpenSSH`
- `Powell-BSD-style`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:7.8p1-1
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.8p1-1.dsc' openssh_7.8p1-1.dsc 3121 SHA256:8ec0c6c21c59e00899e1102b2641ddfea63b1ca3aade5865db6c5aa6a628e266
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.8p1.orig.tar.gz' openssh_7.8p1.orig.tar.gz 1548026 SHA256:1a484bb15152c183bb2514e112aa30dd34138c3cfb032eee5490a66c507144ca
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.8p1.orig.tar.gz.asc' openssh_7.8p1.orig.tar.gz.asc 683 SHA256:01649b5f618d9f19c861a038b981db456778dd7b38a20d039513e2639a022fe4
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.8p1-1.debian.tar.xz' openssh_7.8p1-1.debian.tar.xz 161912 SHA256:e9c101ac6c8123a8148702585c67880229a8d472fb74d4a9ad3767a72b3e7592
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:7.8p1-1/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:7.8p1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:7.8p1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl1.0=1.0.2o-1`

Binary Packages:

- `libssl1.0.2:amd64=1.0.2o-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl1.0=1.0.2o-1
'http://deb.debian.org/debian/pool/main/o/openssl1.0/openssl1.0_1.0.2o-1.dsc' openssl1.0_1.0.2o-1.dsc 2529 SHA256:2539e065ea0c6eb9e8c0c5e6f0464c9cc0c45c6e4d565297564463ab37a5f978
'http://deb.debian.org/debian/pool/main/o/openssl1.0/openssl1.0_1.0.2o.orig.tar.gz' openssl1.0_1.0.2o.orig.tar.gz 5329472 SHA256:ec3f5c9714ba0fd45cb4e087301eb1336c317e0d20b575a125050470e8089e4d
'http://deb.debian.org/debian/pool/main/o/openssl1.0/openssl1.0_1.0.2o.orig.tar.gz.asc' openssl1.0_1.0.2o.orig.tar.gz.asc 455 SHA256:81321834f1809ecd52a624e68c4021b74aa453474ad8c7aaa56c58c1d4f20223
'http://deb.debian.org/debian/pool/main/o/openssl1.0/openssl1.0_1.0.2o-1.debian.tar.xz' openssl1.0_1.0.2o-1.debian.tar.xz 76764 SHA256:b4e0cc0186febfedd06859a71bf3ac24151fed0c8506d3e71634658b82b4948e
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl1.0/1.0.2o-1/ (for browsing the source)
- https://sources.debian.net/src/openssl1.0/1.0.2o-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl1.0/1.0.2o-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.1.0h-4`

Binary Packages:

- `libssl1.1:amd64=1.1.0h-4`
- `openssl=1.1.0h-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.0h-4
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0h-4.dsc' openssl_1.1.0h-4.dsc 2614 SHA256:85ebb39d96f5516bf12e1f61052034e4c80475088102b536ae8b8a1d2c04dd21
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0h.orig.tar.gz' openssl_1.1.0h.orig.tar.gz 5422717 SHA256:5835626cde9e99656585fc7aaa2302a73a7e1340bf8c14fd635a62c66802a517
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0h.orig.tar.gz.asc' openssl_1.1.0h.orig.tar.gz.asc 455 SHA256:5d01aeb02958dcf6e7d4a82d2ca61e9cbe5fd3b32c2bcad150469e29fbbfdccf
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0h-4.debian.tar.xz' openssl_1.1.0h-4.debian.tar.xz 85676 SHA256:94f04d08510f254e0392c8c8611eeb27fbf7df4f00caa42c72ed98f584c637a2
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.0h-4/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.0h-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.0h-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.23.13-2`

Binary Packages:

- `libp11-kit0:amd64=0.23.13-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/p11-kit/0.23.13-2/


### `dpkg` source package: `pam=1.1.8-3.8`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.8`
- `libpam-modules-bin=1.1.8-3.8`
- `libpam-runtime=1.1.8-3.8`
- `libpam0g:amd64=1.1.8-3.8`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.1.8-3.8
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.8.dsc' pam_1.1.8-3.8.dsc 2572 SHA256:1c53c38c71bdba71a5d1e5767cbae505e176b9220e0c07e078309493055c753f
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8.orig.tar.gz' pam_1.1.8.orig.tar.gz 1892765 SHA256:4183409a450708a976eca5af561dbf4f0490141a08e86e4a1e649c7c1b094876
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.8.diff.gz' pam_1.1.8-3.8.diff.gz 138822 SHA256:10e5623f5433460ea05da9cdcb604494a847b4b759102b83dc11e4cf43d59e48
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.1.8-3.8/ (for browsing the source)
- https://sources.debian.net/src/pam/1.1.8-3.8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.1.8-3.8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre2=10.31-3`

Binary Packages:

- `libpcre2-8-0:amd64=10.31-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.31-3
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.31-3.dsc' pcre2_10.31-3.dsc 2342 SHA256:ea30e310dda855534799c709a285864d2df7dc90249bf87334acab1430d1b975
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.31.orig.tar.gz' pcre2_10.31.orig.tar.gz 2130574 SHA256:e11ebd99dd23a7bccc9127d95d9978101b5f3cf0a6e7d25a1b1ca165a97166c4
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.31-3.diff.gz' pcre2_10.31-3.diff.gz 4668 SHA256:0552c9d58e142d8f2dc434d9c2d301fb6774828f611fd49c7b2fae34dfaaeba9
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.31-3/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.31-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.31-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre3=2:8.39-11`

Binary Packages:

- `libpcre3:amd64=2:8.39-11`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-11
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-11.dsc' pcre3_8.39-11.dsc 2226 SHA256:50738a8e55d4bdc10fd6eecc623170d0657bd15805e630d82bc90d722fcbc435
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-11.debian.tar.gz' pcre3_8.39-11.debian.tar.gz 26414 SHA256:de1f66246fe7b4e85fba0f9e3bac69bdf3271a9c5c6b7ac0661b20051c012883
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre3/2:8.39-11/ (for browsing the source)
- https://sources.debian.net/src/pcre3/2:8.39-11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre3/2:8.39-11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.26.2-7`

Binary Packages:

- `libperl5.26:amd64=5.26.2-7`
- `perl=5.26.2-7`
- `perl-base=5.26.2-7`
- `perl-modules-5.26=5.26.2-7`

Licenses: (parsed from: `/usr/share/doc/libperl5.26/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.26/copyright`)

- `Artistic`
- `Artistic,`
- `Artistic-2`
- `Artistic-dist`
- `BSD-3-clause`
- `BSD-3-clause-GENERIC`
- `BSD-3-clause-with-weird-numbering`
- `BSD-4-clause-POWERDOG`
- `BZIP`
- `CC0-1.0`
- `DONT-CHANGE-THE-GPL`
- `Expat`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `GPL-3+-WITH-BISON-EXCEPTION`
- `HSIEH-BSD`
- `HSIEH-DERIVATIVE`
- `LGPL-2.1`
- `REGCOMP`
- `REGCOMP,`
- `RRA-KEEP-THIS-NOTICE`
- `S2P`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.26.2-7
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.26.2-7.dsc' perl_5.26.2-7.dsc 2780 SHA256:5c385bc8c8d6ad08e1ed2942ba4e71dd684b81b744a219d0843b3d60dd50657d
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.26.2.orig-regen-configure.tar.gz' perl_5.26.2.orig-regen-configure.tar.gz 712883 SHA256:918f054a64b2835bc1c6ed79c1e082e7dcdb76735a95b54ee39c25ea9e245ca4
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.26.2.orig.tar.xz' perl_5.26.2.orig.tar.xz 11931624 SHA256:0f8c0fb1b0db4681adb75c3ba0dd77a0472b1b359b9e80efd79fc27b4352132c
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.26.2-7.debian.tar.xz' perl_5.26.2-7.debian.tar.xz 167472 SHA256:84223fbd68d617a2bf3734ebe622b381c74d435aec67c5e17cf60ecb5af6ecb1
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.26.2-7/ (for browsing the source)
- https://sources.debian.net/src/perl/5.26.2-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.26.2-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pinentry=1.1.0-1`

Binary Packages:

- `pinentry-curses=1.1.0-1+b1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-1
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0-1.dsc' pinentry_1.1.0-1.dsc 2910 SHA256:8cda3442923c0e18f9c3d5a2817a97a54db7447046b9c469e890abd19c680247
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2.asc' pinentry_1.1.0.orig.tar.bz2.asc 534 SHA256:0e3a7633b9fddf9c01c3dcf74aeb94888cc6d5d233f0b8357b0b9c1a1fed9a73
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0-1.debian.tar.xz' pinentry_1.1.0-1.debian.tar.xz 15408 SHA256:ddee92638e762f125ac09b86b4f3b31e2d240e8d2dcce940302293bb2ea0873e
```

Other potentially useful URLs:

- https://sources.debian.net/src/pinentry/1.1.0-1/ (for browsing the source)
- https://sources.debian.net/src/pinentry/1.1.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pinentry/1.1.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:3.3.15-2`

Binary Packages:

- `libprocps7:amd64=2:3.3.15-2`
- `procps=2:3.3.15-2`

Licenses: (parsed from: `/usr/share/doc/libprocps7/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.15-2
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.15-2.dsc' procps_3.3.15-2.dsc 2104 SHA256:c7f695ddba2fdf0c3b9de5c38de22713a7046dd9e4a141d59155f4dd62008b32
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.15.orig.tar.xz' procps_3.3.15.orig.tar.xz 903372 SHA256:82e8aa55b65eac116eee05f00d2a884a6374760d57100edd429d6e9b4953458d
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.15-2.debian.tar.xz' procps_3.3.15-2.debian.tar.xz 28060 SHA256:4e90c4129744b726929990239139fde29ab4e438d65d75f5d4c479ead2001aed
```

Other potentially useful URLs:

- https://sources.debian.net/src/procps/2:3.3.15-2/ (for browsing the source)
- https://sources.debian.net/src/procps/2:3.3.15-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/procps/2:3.3.15-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python-defaults=2.7.15-3`

Binary Packages:

- `libpython-stdlib:amd64=2.7.15-3`
- `libpython2-stdlib:amd64=2.7.15-3`
- `python=2.7.15-3`
- `python-minimal=2.7.15-3`
- `python2=2.7.15-3`
- `python2-minimal=2.7.15-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.15-3
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.15-3.dsc' python-defaults_2.7.15-3.dsc 2961 SHA256:a4072c1b0eb94df5516edf2de5faebcc15b8465dc42ed70ea810bddf28a6bb11
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.15-3.tar.gz' python-defaults_2.7.15-3.tar.gz 1398803 SHA256:beb52f958d2a17056e145083715fdb9ed4b3422051d9692243cdbb26798a0c8a
```

Other potentially useful URLs:

- https://sources.debian.net/src/python-defaults/2.7.15-3/ (for browsing the source)
- https://sources.debian.net/src/python-defaults/2.7.15-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python-defaults/2.7.15-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python2.7=2.7.15-4`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.15-4`
- `libpython2.7-stdlib:amd64=2.7.15-4`
- `python2.7=2.7.15-4`
- `python2.7-minimal=2.7.15-4`

Licenses: (parsed from: `/usr/share/doc/libpython2.7-minimal/copyright`, `/usr/share/doc/libpython2.7-stdlib/copyright`, `/usr/share/doc/python2.7/copyright`, `/usr/share/doc/python2.7-minimal/copyright`)

- `# Licensed to PSF under a Contributor Agreement`
- `* Permission to use this software in any way is granted without`
- `Apache`
- `Apache-2`
- `Apache-2.0`
- `Expat`
- `GPL-2`
- `ISC`
- `LGPL-2.1+`
- `PSF-2`
- `Permission is hereby granted, free of charge, to any person obtaining`
- `Python`
- `This software is provided 'as-is', without any express`
- `This software is provided as-is, without express`
- `implied`
- `see above, some license as Python`

Source:

```console
$ apt-get source -qq --print-uris python2.7=2.7.15-4
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.15-4.dsc' python2.7_2.7.15-4.dsc 3357 SHA256:86c6621118d37dcb4a9e10b98ea9a26d91309247dac6e356ad4a847bfc3a8975
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.15.orig.tar.gz' python2.7_2.7.15.orig.tar.gz 17496336 SHA256:18617d1f15a380a919d517630a9cd85ce17ea602f9bbdc58ddc672df4b0239db
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.15-4.diff.gz' python2.7_2.7.15-4.diff.gz 483036 SHA256:05ca1a74c8172f890e7dcfe920212b125b345b1d60c97ad5cbf0fd4ac28d0d7b
```

Other potentially useful URLs:

- https://sources.debian.net/src/python2.7/2.7.15-4/ (for browsing the source)
- https://sources.debian.net/src/python2.7/2.7.15-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python2.7/2.7.15-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=7.0-5`

Binary Packages:

- `libreadline7:amd64=7.0-5`
- `readline-common=7.0-5`

Licenses: (parsed from: `/usr/share/doc/libreadline7/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=7.0-5
'http://deb.debian.org/debian/pool/main/r/readline/readline_7.0-5.dsc' readline_7.0-5.dsc 2419 SHA256:4a804235e91ced3b957b0772101ca3992f5ad051e6540b8c41a1f98a06e84033
'http://deb.debian.org/debian/pool/main/r/readline/readline_7.0.orig.tar.gz' readline_7.0.orig.tar.gz 2910016 SHA256:750d437185286f40a369e1e4f4764eda932b9459b5ec9a731628393dd3d32334
'http://deb.debian.org/debian/pool/main/r/readline/readline_7.0-5.debian.tar.xz' readline_7.0-5.debian.tar.xz 29992 SHA256:5c1cc7396a670ce7e6e4c0bc36e8d3067b7642bea5b30fc3ff22bf8e65d2ee80
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline/7.0-5/ (for browsing the source)
- https://sources.debian.net/src/readline/7.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline/7.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc 2299 SHA256:a296819cd2ab5880b67ad963ef0867cb10e462f4403e52565aa863eb05bb1370
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz 8096 SHA256:26d47de07d16285e4ca55b0828cbbf1ba35e671f9b3500a87e301fe755d26882
```

Other potentially useful URLs:

- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-2/ (for browsing the source)
- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rtmpdump/2.4+20151223.gitfa8646d.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sed=4.5-1`

Binary Packages:

- `sed=4.5-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.5-1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.5-1.dsc' sed_4.5-1.dsc 2218 SHA256:9fba9d65b814cfbd7045fa5c4a3d2c33256542db8669cb3d9db63efd0ef24c66
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.5.orig.tar.xz' sed_4.5.orig.tar.xz 1274252 SHA256:7aad73c8839c2bdadca9476f884d2953cdace9567ecd0d90f9959f229d146b40
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.5.orig.tar.xz.asc' sed_4.5.orig.tar.xz.asc 1258 SHA256:d6a7f0df70447358fdc1eaea4bad77250b43c53df4938dae256006b7c6356141
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.5-1.debian.tar.xz' sed_4.5-1.debian.tar.xz 59764 SHA256:cb8e5d77782b088aca6b0205dee1ce86ffa97bf4bfcb01fee5e6affe8d08fc4c
```

Other potentially useful URLs:

- https://sources.debian.net/src/sed/4.5-1/ (for browsing the source)
- https://sources.debian.net/src/sed/4.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sed/4.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sensible-utils=0.0.12`

Binary Packages:

- `sensible-utils=0.0.12`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.12
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.12.dsc' sensible-utils_0.0.12.dsc 1732 SHA256:1b62cc5f7561b3f5692a6edaec942e2e97e8368dabff8c865867d428eecb1221
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.12.tar.xz' sensible-utils_0.0.12.tar.xz 62152 SHA256:99ba2ebf8c57447c69d426b99b84ff9dc817be0bc4988ec6890a14558c529e2e
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.12/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `serf=1.3.9-6`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-6`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-6/


### `dpkg` source package: `shadow=1:4.5-1.1`

Binary Packages:

- `login=1:4.5-1.1`
- `passwd=1:4.5-1.1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.5-1.1
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.5-1.1.dsc' shadow_4.5-1.1.dsc 2319 SHA256:75993dc19ccc4d5c404831d2dab021a03eaa39216b518d596b639d8f2ea4e98b
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.5.orig.tar.xz' shadow_4.5.orig.tar.xz 1344524 SHA256:22b0952dc944b163e2370bb911b11ca275fc80ad024267cf21e496b28c23d500
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.5-1.1.debian.tar.xz' shadow_4.5-1.1.debian.tar.xz 462960 SHA256:3bb16bbf5d9a255d7333932ae99815d65c1c8e86127e5016809d4ba55c499538
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.5-1.1/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.5-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.5-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sqlite3=3.24.0-1`

Binary Packages:

- `libsqlite3-0:amd64=3.24.0-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sqlite3/3.24.0-1/


### `dpkg` source package: `subversion=1.10.2-1`

Binary Packages:

- `libsvn1:amd64=1.10.2-1`
- `subversion=1.10.2-1`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris subversion=1.10.2-1
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.10.2-1.dsc' subversion_1.10.2-1.dsc 3516 SHA256:f086b629c60d8eae9c46d5b7f630e1ad3ebac78c192a21502016ac710a9724f7
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.10.2.orig.tar.gz' subversion_1.10.2.orig.tar.gz 11340555 SHA256:4f1be1bc26758c7c85c0ba6e7e8a90ce02e346607e84f44e018753f096f86577
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.10.2.orig.tar.gz.asc' subversion_1.10.2.orig.tar.gz.asc 2485 SHA256:3828cd55766859ec42374745f6ed0967b3c1dc85df8e770ceb07e4a265892ceb
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.10.2-1.debian.tar.xz' subversion_1.10.2-1.debian.tar.xz 2402840 SHA256:072ef649e862aedc919d9c2feab6c92ca57de14cfb25d50a734ae6ca6e4b5378
```

Other potentially useful URLs:

- https://sources.debian.net/src/subversion/1.10.2-1/ (for browsing the source)
- https://sources.debian.net/src/subversion/1.10.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/subversion/1.10.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=239-7`

Binary Packages:

- `libsystemd0:amd64=239-7`
- `libudev1:amd64=239-7`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`)

- `CC0-1.0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/systemd/239-7/


### `dpkg` source package: `sysvinit=2.88dsf-59.10`

Binary Packages:

- `sysvinit-utils=2.88dsf-59.10`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59.10
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10.dsc' sysvinit_2.88dsf-59.10.dsc 2353 SHA256:b25f6800b2c0f1cfd978979f25371a79493c81c6ad0815b541d12deaae75e319
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10.debian.tar.xz' sysvinit_2.88dsf-59.10.debian.tar.xz 132504 SHA256:3dd24f403de4565abe55181fbde15ac013e520bf65f159b875637f6c41972519
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/2.88dsf-59.10/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/2.88dsf-59.10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/2.88dsf-59.10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.30+dfsg-2`

Binary Packages:

- `tar=1.30+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.30+dfsg-2
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.30+dfsg-2.dsc' tar_1.30+dfsg-2.dsc 1951 SHA256:e06cc08da7db7e8a546a946c23d89042cf86c9e8ae3a5c2c4e0d585ad6f2039f
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.30+dfsg.orig.tar.xz' tar_1.30+dfsg.orig.tar.xz 1883220 SHA256:c02f3747ffe02017878303dde8b78e79cd220364c5e8048cf92320232e38912d
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.30+dfsg-2.debian.tar.xz' tar_1.30+dfsg-2.debian.tar.xz 17384 SHA256:7799136a18d6735463d421f5b48df900cd51ee7e89e3e6acc6c401bd903e4231
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.30+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/tar/1.30+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.30+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2018e-1`

Binary Packages:

- `tzdata=2018e-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2018e-1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2018e-1.dsc' tzdata_2018e-1.dsc 2232 SHA256:68552c028c1c8f2bec8ac786acf1afb9b38ba1f821a3f39da5ae6e3aee744f63
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2018e.orig.tar.gz' tzdata_2018e.orig.tar.gz 353953 SHA256:6b288e5926841a4cb490909fe822d85c36ae75538ad69baf20da9628b63b692e
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2018e.orig.tar.gz.asc' tzdata_2018e.orig.tar.gz.asc 819 SHA256:46812e7b7761bf4cbee7449a500cb0fba46912f99f6725b9437ab2f226e64753
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2018e-1.debian.tar.xz' tzdata_2018e-1.debian.tar.xz 104188 SHA256:2c8999456a1529a1e4abe42d5d97bbafe2eba0fa00f2a1a4140c0af74ed94750
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2018e-1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2018e-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2018e-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ucf=3.0038`

Binary Packages:

- `ucf=3.0038`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0038
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0038.dsc' ucf_3.0038.dsc 1445 SHA256:5fab6d0af664eac92b3404c6bb62d0a3ceb88cd21a1462b9a262d1292c77328f
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0038.tar.xz' ucf_3.0038.tar.xz 65416 SHA256:262ccd52637c869ac851838a176d76e90db8d3f12373e3b62eb89e217f93fe7e
```

Other potentially useful URLs:

- https://sources.debian.net/src/ucf/3.0038/ (for browsing the source)
- https://sources.debian.net/src/ucf/3.0038/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ucf/3.0038/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `utf8proc=2.2.0-1`

Binary Packages:

- `libutf8proc2:amd64=2.2.0-1`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.2.0-1
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.2.0-1.dsc' utf8proc_2.2.0-1.dsc 2094 SHA256:e410b68eeb6c16e7b9db86d654b1d96f561d94ecd0b72b3da615e2e1c0b7d611
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.2.0.orig.tar.gz' utf8proc_2.2.0.orig.tar.gz 156334 SHA256:3f8fd1dbdb057ee5ba584a539d5cd1b3952141c0338557cb0bdf8cb9cfed5dbf
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.2.0-1.debian.tar.xz' utf8proc_2.2.0-1.debian.tar.xz 4992 SHA256:7e4478c75cb1f04b23346d4485a64bd65d7ba8d52387d5fef55c4c4066a8eba0
```

Other potentially useful URLs:

- https://sources.debian.net/src/utf8proc/2.2.0-1/ (for browsing the source)
- https://sources.debian.net/src/utf8proc/2.2.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/utf8proc/2.2.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.32.1-0.1`

Binary Packages:

- `bsdutils=1:2.32.1-0.1`
- `fdisk=2.32.1-0.1`
- `libblkid1:amd64=2.32.1-0.1`
- `libfdisk1:amd64=2.32.1-0.1`
- `libmount1:amd64=2.32.1-0.1`
- `libsmartcols1:amd64=2.32.1-0.1`
- `libuuid1:amd64=2.32.1-0.1`
- `mount=2.32.1-0.1`
- `util-linux=2.32.1-0.1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/fdisk/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris util-linux=2.32.1-0.1
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.32.1-0.1.dsc' util-linux_2.32.1-0.1.dsc 4056 SHA256:a8a5e6b6e299ccdf262bc8966e8f7bc943194900aef5495b038d987458bd27d4
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.32.1.orig.tar.xz' util-linux_2.32.1.orig.tar.xz 4561088 SHA256:86e6707a379c7ff5489c218cfaf1e3464b0b95acf7817db0bc5f179e356a67b2
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.32.1-0.1.debian.tar.xz' util-linux_2.32.1-0.1.debian.tar.xz 82140 SHA256:dc787b94bbbef1ea0c8c1f647754312818d8b6b80cbc6ecad7b97ffedfb79804
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.32.1-0.1/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.32.1-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.32.1-0.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.19.5-1`

Binary Packages:

- `wget=1.19.5-1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.19.5-1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.19.5-1.dsc' wget_1.19.5-1.dsc 2155 SHA256:0171f759be8a7b460e4ee01e932a80dda40125780c73fba675be9959a0affe1e
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.19.5.orig.tar.gz' wget_1.19.5.orig.tar.gz 4455797 SHA256:b39212abe1a73f2b28f4c6cb223c738559caac91d6e416a6d91d4b9d55c9faee
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.19.5.orig.tar.gz.asc' wget_1.19.5.orig.tar.gz.asc 879 SHA256:f2058db1f155fc5564de797d11dc40f5fa721f35e36e02bf06332771db150ef7
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.19.5-1.debian.tar.xz' wget_1.19.5-1.debian.tar.xz 60208 SHA256:24e48282b093e87b1b90f5874ae7446386b13ffe61ad68e1681522f3576fd161
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.19.5-1/ (for browsing the source)
- https://sources.debian.net/src/wget/1.19.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.19.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.2.2-1.3`

Binary Packages:

- `liblzma5:amd64=5.2.2-1.3`

Licenses: (parsed from: `/usr/share/doc/liblzma5/copyright`)

- `Autoconf`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`
- `PD`
- `PD-debian`
- `config-h`
- `noderivs`
- `none`
- `permissive-fsf`
- `permissive-nowarranty`
- `probably-PD`

Source:

```console
$ apt-get source -qq --print-uris xz-utils=5.2.2-1.3
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.dsc' xz-utils_5.2.2-1.3.dsc 2575 SHA256:3ea4e6a32f6265b152f89ceafe78c8839e5f4bb1cad137b159fe2013817f9342
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz' xz-utils_5.2.2.orig.tar.xz 1016404 SHA256:f341b1906ebcdde291dd619399ae944600edc9193619dd0c0110a5f05bfcc89e
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz.asc' xz-utils_5.2.2.orig.tar.xz.asc 543 SHA256:2cc0575556e1331b3f468e6e7dca5969ce86efcc315d62672279b4e68b2e449f
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.debian.tar.xz' xz-utils_5.2.2-1.3.debian.tar.xz 108680 SHA256:d76c3acf39d0999c14384695394970e8f98853fd6736ba91972d3e67106bc6f6
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.2.2-1.3/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.2.2-1.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.2.2-1.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.11.dfsg-1`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-1`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-1
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-1.dsc' zlib_1.2.11.dfsg-1.dsc 2266 SHA256:bf21ab4d60cb836725162f5072884596e781a2f4974182af1868f546306eb8c8
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA256:80c481411a4fe8463aeb8270149a0e80bb9eaf7da44132b6e16f2b5af01bc899
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-1.debian.tar.xz' zlib_1.2.11.dfsg-1.debian.tar.xz 18956 SHA256:00b95b629fbe9a5181f8ba1ceddedf627aba1ab42e47f5916be8a41deb54098a
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.11.dfsg-1/ (for access to the source package after it no longer exists in the archive)
