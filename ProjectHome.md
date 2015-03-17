# gcsfs #

gcsfs is a FUSE (Filesystem in Userspace) driver for Google Cloud Storage and other cloud storage providers that permits the mounting of buckets locally.  It's based on [s3fuse](https://code.google.com/p/s3fuse).

## Features ##

  * Binaries for Debian 7, RHEL/CentOS 6, Ubuntu, and OS X 10.9.
  * Compatible with GCS web console.
  * Caches file/directory metadata for improved performance.
  * Verifies file consistency on upload/download.
  * Optional file content encryption.
  * Supports multi-part (resumable) uploads.
  * Allows setting Cache-Control header (via extended attributes on files).
  * Maps file extensions to known MIME types (to set Content-Type header).
  * (Mostly) POSIX compliant.

## What's New ##

_2013-11-24_: Version 0.15 released with minor updates:

  * Removed libxml++ dependency.
  * Fixed libcurl init/cleanup bug.
  * Removed known-issue notes on MIME mapping and Google Cloud Storage Manager folder representation incompatibility.

> Since [Google Code downloads are deprecated](http://google-opensource.blogspot.com/2013/05/a-change-to-google-code-download-service.html), this and future gcsfs releases will be hosted here:
> https://drive.google.com/folderview?id=0B071t7_clY1HU2RTT3BqT1dKQ0E&usp=sharing#list

> Ubuntu packages are here:
> https://launchpad.net/~gcsfs/+archive/stable