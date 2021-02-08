# ffmpeg-v4-for-kernel-v2.6
YEP
```
PATH="$HOME/bin:$PATH" PKG_CONFIG_PATH="$HOME/ffmpeg_build/lib/pkgconfig" ./configure \
  --prefix="$HOME/ffmpeg_build" \
  --pkg-config-flags="--static" \
  --extra-cflags="-I$HOME/ffmpeg_build/include" \
  --extra-ldflags="-L$HOME/ffmpeg_build/lib" \
  --extra-libs=-lpthread \
  --extra-libs=-lm \
  --bindir="$HOME/bin" \
  --enable-gpl \
  --enable-libfdk_aac \
  --enable-libfreetype \
  --enable-libmp3lame \
  --enable-libopus \
  --enable-libvorbis \
  --enable-libx264 \
  --enable-libx265 \
  --enable-nonfree \
  --enable-openssl \
  --enable-muxer=segment \
  --enable-decoder=mjpeg,png \
  --enable-demuxer=image2 \
  --enable-zlib \
  --enable-protocol=file \
  --enable-decoder=png \
  --enable-encoder=png \
  --enable-muxer=stream_segment
```

**NO LIBVPX** sorry couldn't get it compiled :sadge:
