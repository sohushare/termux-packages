------------------------------------------------------------------------
BUILD
------------------------------------------------------------------------
./build-package.sh bash bzip2 command-not-found coreutils dash diffutils findutils gawk grep gzip less procps psmisc sed tar termux-exec termux-tools util-linux libc++
------------------------------------------------------------------------
UPLOAD
------------------------------------------------------------------------
./scripts/package_uploader.sh -p ./debs bash ....

ncurses libandroid-support libiconv readline libgmp libnghttp2 libssh2 openssl ca-certificates zlib libmpfr pcre termux-am libcrypt xz-utils dialog

curl --> libcurl
bzip2 --> libbz2
xz-utils --> liblzma