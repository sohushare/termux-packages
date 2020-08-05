./scripts/run-docker.sh
CONTAINER_NAME=termux_builder_6 ./scripts/run-docker.sh

------------------------------------------------------------------------
BUILD
------------------------------------------------------------------------
./build-package.sh bash bzip2 command-not-found coreutils dash diffutils findutils gawk grep gzip less procps psmisc sed tar termux-exec termux-tools util-linux libc++ python yarn git

./build-package.sh -a arm bash bzip2 command-not-found coreutils dash diffutils findutils gawk grep gzip less procps psmisc sed tar termux-exec termux-tools util-linux libc++ python yarn git

./build-package.sh -a i686 bash bzip2 command-not-found coreutils dash diffutils findutils gawk grep gzip less procps psmisc sed tar termux-exec termux-tools util-linux libc++ python yarn git

./build-package.sh -a x86_64 bash bzip2 command-not-found coreutils dash diffutils findutils gawk grep gzip less procps psmisc sed tar termux-exec termux-tools util-linux libc++ python yarn git
------------------------------------------------------------------------
UPLOAD
------------------------------------------------------------------------
./scripts/package_uploader.sh -p ./debs bash ....

ncurses libandroid-support libiconv readline libgmp libnghttp2 libssh2 openssl ca-certificates zlib libmpfr pcre termux-am libcrypt xz-utils dialog libc++

curl --> libcurl
bzip2 --> libbz2
xz-utils --> liblzma

For nodejs: c-ares libicu

For apt: dpkg gpgv libgcrypt

gpgv -> gnupg