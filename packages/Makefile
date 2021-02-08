all: packages

BASE_PACKAGES = freeswitch spandsp tiff libjpeg-turbo sofia-sip check sqlite speex ldns libedit yasm libav lua opus postgresql tcl libks signalwire-client-c libsndfile libpng x264 nasm flac libogg libvorbis alsa-lib certbot firewall volatile-config

spandsp: tiff libjpeg-turbo
sofia-sip: check
x264: nasm
libav: libpng x264
postgresql: tcl
libsndfile: flac sqlite libvorbis libogg alsa-lib
flac: nasm libogg
freeswitch: spandsp sofia-sip sqlite speex ldns libedit yasm libav lua opus postgresql libks signalwire-client-c libsndfile

include Makefile.common
