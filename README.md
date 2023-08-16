# ImageMagick packaged for Immich Distribution

[ImageMagick](https://imagemagick.org/) is a image processing tool that I use in [Immich Distribution](https://github.com/nsg/immich-distribution). This repo is used as a dependency of the Immich Distribution project and is not intended for direct consumption.

## Usage

```yaml
stage-snaps:
    - immich-distribution-imagemagick/latest/stable
```

## Contents
```
.
├── etc
│   └── fonts
│       ├── conf.avail
│       │   ├── 10-antialias.conf
│       │   ├── 10-autohint.conf
│       │   ├── 10-hinting-full.conf
│       │   ├── 10-hinting-medium.conf
│       │   ├── 10-hinting-none.conf
│       │   ├── 10-hinting-slight.conf
│       │   ├── 10-no-sub-pixel.conf
│       │   ├── 10-scale-bitmap-fonts.conf
│       │   ├── 10-sub-pixel-bgr.conf
│       │   ├── 10-sub-pixel-rgb.conf
│       │   ├── 10-sub-pixel-vbgr.conf
│       │   ├── 10-sub-pixel-vrgb.conf
│       │   ├── 10-unhinted.conf
│       │   ├── 11-lcdfilter-default.conf
│       │   ├── 11-lcdfilter-legacy.conf
│       │   ├── 11-lcdfilter-light.conf
│       │   ├── 20-unhint-small-dejavu-lgc-sans.conf
│       │   ├── 20-unhint-small-dejavu-lgc-sans-mono.conf
│       │   ├── 20-unhint-small-dejavu-lgc-serif.conf
│       │   ├── 20-unhint-small-dejavu-sans.conf
│       │   ├── 20-unhint-small-dejavu-sans-mono.conf
│       │   ├── 20-unhint-small-dejavu-serif.conf
│       │   ├── 20-unhint-small-vera.conf
│       │   ├── 25-unhint-nonlatin.conf
│       │   ├── 30-metric-aliases.conf
│       │   ├── 40-nonlatin.conf
│       │   ├── 45-generic.conf
│       │   ├── 45-latin.conf
│       │   ├── 49-sansserif.conf
│       │   ├── 50-user.conf
│       │   ├── 51-local.conf
│       │   ├── 53-monospace-lcd-filter.conf
│       │   ├── 57-dejavu-sans.conf
│       │   ├── 57-dejavu-sans-mono.conf
│       │   ├── 57-dejavu-serif.conf
│       │   ├── 58-dejavu-lgc-sans.conf
│       │   ├── 58-dejavu-lgc-sans-mono.conf
│       │   ├── 58-dejavu-lgc-serif.conf
│       │   ├── 60-generic.conf
│       │   ├── 60-latin.conf
│       │   ├── 65-fonts-persian.conf
│       │   ├── 65-khmer.conf
│       │   ├── 65-nonlatin.conf
│       │   ├── 69-unifont.conf
│       │   ├── 70-force-bitmaps.conf
│       │   ├── 70-no-bitmaps.conf
│       │   ├── 70-yes-bitmaps.conf
│       │   ├── 80-delicious.conf
│       │   └── 90-synthetic.conf
│       ├── conf.d
│       │   ├── 10-antialias.conf -> ../conf.avail/10-antialias.conf
│       │   ├── 10-hinting-slight.conf -> ../conf.avail/10-hinting-slight.conf
│       │   ├── 10-scale-bitmap-fonts.conf -> ../conf.avail/10-scale-bitmap-fonts.conf
│       │   ├── 11-lcdfilter-default.conf -> ../conf.avail/11-lcdfilter-default.conf
│       │   ├── 20-unhint-small-dejavu-lgc-sans.conf -> ../conf.avail/20-unhint-small-dejavu-lgc-sans.conf
│       │   ├── 20-unhint-small-dejavu-lgc-sans-mono.conf -> ../conf.avail/20-unhint-small-dejavu-lgc-sans-mono.conf
│       │   ├── 20-unhint-small-dejavu-lgc-serif.conf -> ../conf.avail/20-unhint-small-dejavu-lgc-serif.conf
│       │   ├── 20-unhint-small-dejavu-sans.conf -> ../conf.avail/20-unhint-small-dejavu-sans.conf
│       │   ├── 20-unhint-small-dejavu-sans-mono.conf -> ../conf.avail/20-unhint-small-dejavu-sans-mono.conf
│       │   ├── 20-unhint-small-dejavu-serif.conf -> ../conf.avail/20-unhint-small-dejavu-serif.conf
│       │   ├── 20-unhint-small-vera.conf -> ../conf.avail/20-unhint-small-vera.conf
│       │   ├── 30-metric-aliases.conf -> ../conf.avail/30-metric-aliases.conf
│       │   ├── 40-nonlatin.conf -> ../conf.avail/40-nonlatin.conf
│       │   ├── 45-generic.conf -> ../conf.avail/45-generic.conf
│       │   ├── 45-latin.conf -> ../conf.avail/45-latin.conf
│       │   ├── 49-sansserif.conf -> ../conf.avail/49-sansserif.conf
│       │   ├── 50-user.conf -> ../conf.avail/50-user.conf
│       │   ├── 51-local.conf -> ../conf.avail/51-local.conf
│       │   ├── 57-dejavu-sans.conf -> ../conf.avail/57-dejavu-sans.conf
│       │   ├── 57-dejavu-sans-mono.conf -> ../conf.avail/57-dejavu-sans-mono.conf
│       │   ├── 57-dejavu-serif.conf -> ../conf.avail/57-dejavu-serif.conf
│       │   ├── 58-dejavu-lgc-sans.conf -> ../conf.avail/58-dejavu-lgc-sans.conf
│       │   ├── 58-dejavu-lgc-sans-mono.conf -> ../conf.avail/58-dejavu-lgc-sans-mono.conf
│       │   ├── 58-dejavu-lgc-serif.conf -> ../conf.avail/58-dejavu-lgc-serif.conf
│       │   ├── 60-generic.conf -> ../conf.avail/60-generic.conf
│       │   ├── 60-latin.conf -> ../conf.avail/60-latin.conf
│       │   ├── 65-fonts-persian.conf -> ../conf.avail/65-fonts-persian.conf
│       │   ├── 65-nonlatin.conf -> ../conf.avail/65-nonlatin.conf
│       │   ├── 69-unifont.conf -> ../conf.avail/69-unifont.conf
│       │   ├── 70-no-bitmaps.conf -> ../conf.avail/70-no-bitmaps.conf
│       │   ├── 80-delicious.conf -> ../conf.avail/80-delicious.conf
│       │   ├── 90-synthetic.conf -> ../conf.avail/90-synthetic.conf
│       │   └── README
│       └── fonts.conf
├── meta
│   └── snap.yaml
└── usr
    ├── bin
    │   ├── animate -> magick
    │   ├── compare -> magick
    │   ├── composite -> magick
    │   ├── conjure -> magick
    │   ├── convert -> magick
    │   ├── display -> magick
    │   ├── fc-cache
    │   ├── fc-cat
    │   ├── fc-conflist
    │   ├── fc-list
    │   ├── fc-match
    │   ├── fc-pattern
    │   ├── fc-query
    │   ├── fc-scan
    │   ├── fc-validate
    │   ├── identify -> magick
    │   ├── import -> magick
    │   ├── magick
    │   ├── Magick++-config
    │   ├── MagickCore-config
    │   ├── magick-script -> magick
    │   ├── MagickWand-config
    │   ├── mogrify -> magick
    │   ├── montage -> magick
    │   └── stream -> magick
    ├── etc
    │   └── ImageMagick-7
    │       ├── colors.xml
    │       ├── delegates.xml
    │       ├── log.xml
    │       ├── mime.xml
    │       ├── policy.xml
    │       ├── quantization-table.xml
    │       ├── thresholds.xml
    │       ├── type-apple.xml
    │       ├── type-dejavu.xml
    │       ├── type-ghostscript.xml
    │       ├── type-urw-base35.xml
    │       ├── type-windows.xml
    │       └── type.xml
    ├── include
    │   └── ImageMagick-7
    │       ├── Magick++
    │       │   ├── Blob.h
    │       │   ├── CoderInfo.h
    │       │   ├── Color.h
    │       │   ├── Drawable.h
    │       │   ├── Exception.h
    │       │   ├── Functions.h
    │       │   ├── Geometry.h
    │       │   ├── Image.h
    │       │   ├── Include.h
    │       │   ├── Montage.h
    │       │   ├── Pixels.h
    │       │   ├── ResourceLimits.h
    │       │   ├── SecurityPolicy.h
    │       │   ├── Statistic.h
    │       │   ├── STL.h
    │       │   └── TypeMetric.h
    │       ├── MagickCore
    │       │   ├── animate.h
    │       │   ├── annotate.h
    │       │   ├── artifact.h
    │       │   ├── attribute.h
    │       │   ├── blob.h
    │       │   ├── cache.h
    │       │   ├── cache-view.h
    │       │   ├── channel.h
    │       │   ├── cipher.h
    │       │   ├── client.h
    │       │   ├── coder.h
    │       │   ├── color.h
    │       │   ├── colormap.h
    │       │   ├── colorspace.h
    │       │   ├── compare.h
    │       │   ├── composite.h
    │       │   ├── compress.h
    │       │   ├── configure.h
    │       │   ├── constitute.h
    │       │   ├── decorate.h
    │       │   ├── delegate.h
    │       │   ├── deprecate.h
    │       │   ├── display.h
    │       │   ├── distort.h
    │       │   ├── distribute-cache.h
    │       │   ├── draw.h
    │       │   ├── effect.h
    │       │   ├── enhance.h
    │       │   ├── exception.h
    │       │   ├── feature.h
    │       │   ├── fourier.h
    │       │   ├── fx.h
    │       │   ├── gem.h
    │       │   ├── geometry.h
    │       │   ├── histogram.h
    │       │   ├── identify.h
    │       │   ├── image.h
    │       │   ├── image-view.h
    │       │   ├── layer.h
    │       │   ├── linked-list.h
    │       │   ├── list.h
    │       │   ├── locale_.h
    │       │   ├── log.h
    │       │   ├── magic.h
    │       │   ├── magick-baseconfig.h
    │       │   ├── magick-config.h
    │       │   ├── MagickCore.h
    │       │   ├── magick.h
    │       │   ├── magick-type.h
    │       │   ├── matrix.h
    │       │   ├── memory_.h
    │       │   ├── method-attribute.h
    │       │   ├── methods.h
    │       │   ├── mime.h
    │       │   ├── module.h
    │       │   ├── monitor.h
    │       │   ├── montage.h
    │       │   ├── morphology.h
    │       │   ├── nt-base.h
    │       │   ├── opencl.h
    │       │   ├── option.h
    │       │   ├── paint.h
    │       │   ├── pixel-accessor.h
    │       │   ├── pixel.h
    │       │   ├── policy.h
    │       │   ├── prepress.h
    │       │   ├── profile.h
    │       │   ├── property.h
    │       │   ├── quantize.h
    │       │   ├── quantum.h
    │       │   ├── random_.h
    │       │   ├── registry.h
    │       │   ├── resample.h
    │       │   ├── resize.h
    │       │   ├── resource_.h
    │       │   ├── segment.h
    │       │   ├── semaphore.h
    │       │   ├── shear.h
    │       │   ├── signature.h
    │       │   ├── splay-tree.h
    │       │   ├── static.h
    │       │   ├── statistic.h
    │       │   ├── stream.h
    │       │   ├── string_.h
    │       │   ├── studio.h
    │       │   ├── threshold.h
    │       │   ├── timer.h
    │       │   ├── token.h
    │       │   ├── transform.h
    │       │   ├── type.h
    │       │   ├── utility.h
    │       │   ├── version.h
    │       │   ├── vision.h
    │       │   ├── visual-effects.h
    │       │   ├── widget.h
    │       │   ├── xml-tree.h
    │       │   └── xwindow.h
    │       ├── Magick++.h
    │       └── MagickWand
    │           ├── animate.h
    │           ├── compare.h
    │           ├── composite.h
    │           ├── conjure.h
    │           ├── convert.h
    │           ├── deprecate.h
    │           ├── display.h
    │           ├── drawing-wand.h
    │           ├── identify.h
    │           ├── import.h
    │           ├── magick-cli.h
    │           ├── magick-image.h
    │           ├── magick-property.h
    │           ├── MagickWand.h
    │           ├── method-attribute.h
    │           ├── mogrify.h
    │           ├── montage.h
    │           ├── operation.h
    │           ├── pixel-iterator.h
    │           ├── pixel-wand.h
    │           ├── stream.h
    │           ├── wandcli.h
    │           └── wand-view.h
    ├── lib
    │   ├── ImageMagick-7.1.1
    │   │   ├── config-Q16HDRI
    │   │   │   └── configure.xml
    │   │   └── modules-Q16HDRI
    │   │       ├── coders
    │   │       │   ├── aai.la
    │   │       │   ├── aai.so
    │   │       │   ├── art.la
    │   │       │   ├── art.so
    │   │       │   ├── ashlar.la
    │   │       │   ├── ashlar.so
    │   │       │   ├── avs.la
    │   │       │   ├── avs.so
    │   │       │   ├── bayer.la
    │   │       │   ├── bayer.so
    │   │       │   ├── bgr.la
    │   │       │   ├── bgr.so
    │   │       │   ├── bmp.la
    │   │       │   ├── bmp.so
    │   │       │   ├── braille.la
    │   │       │   ├── braille.so
    │   │       │   ├── cals.la
    │   │       │   ├── cals.so
    │   │       │   ├── caption.la
    │   │       │   ├── caption.so
    │   │       │   ├── cin.la
    │   │       │   ├── cin.so
    │   │       │   ├── cip.la
    │   │       │   ├── cip.so
    │   │       │   ├── clip.la
    │   │       │   ├── clip.so
    │   │       │   ├── cmyk.la
    │   │       │   ├── cmyk.so
    │   │       │   ├── cube.la
    │   │       │   ├── cube.so
    │   │       │   ├── cut.la
    │   │       │   ├── cut.so
    │   │       │   ├── dcm.la
    │   │       │   ├── dcm.so
    │   │       │   ├── dds.la
    │   │       │   ├── dds.so
    │   │       │   ├── debug.la
    │   │       │   ├── debug.so
    │   │       │   ├── dib.la
    │   │       │   ├── dib.so
    │   │       │   ├── dng.la
    │   │       │   ├── dng.so
    │   │       │   ├── dot.la
    │   │       │   ├── dot.so
    │   │       │   ├── dpx.la
    │   │       │   ├── dpx.so
    │   │       │   ├── farbfeld.la
    │   │       │   ├── farbfeld.so
    │   │       │   ├── fax.la
    │   │       │   ├── fax.so
    │   │       │   ├── fits.la
    │   │       │   ├── fits.so
    │   │       │   ├── fl32.la
    │   │       │   ├── fl32.so
    │   │       │   ├── ftxt.la
    │   │       │   ├── ftxt.so
    │   │       │   ├── gif.la
    │   │       │   ├── gif.so
    │   │       │   ├── gradient.la
    │   │       │   ├── gradient.so
    │   │       │   ├── gray.la
    │   │       │   ├── gray.so
    │   │       │   ├── hald.la
    │   │       │   ├── hald.so
    │   │       │   ├── hdr.la
    │   │       │   ├── hdr.so
    │   │       │   ├── histogram.la
    │   │       │   ├── histogram.so
    │   │       │   ├── hrz.la
    │   │       │   ├── hrz.so
    │   │       │   ├── html.la
    │   │       │   ├── html.so
    │   │       │   ├── icon.la
    │   │       │   ├── icon.so
    │   │       │   ├── info.la
    │   │       │   ├── info.so
    │   │       │   ├── inline.la
    │   │       │   ├── inline.so
    │   │       │   ├── ipl.la
    │   │       │   ├── ipl.so
    │   │       │   ├── jnx.la
    │   │       │   ├── jnx.so
    │   │       │   ├── json.la
    │   │       │   ├── json.so
    │   │       │   ├── kernel.la
    │   │       │   ├── kernel.so
    │   │       │   ├── label.la
    │   │       │   ├── label.so
    │   │       │   ├── mac.la
    │   │       │   ├── mac.so
    │   │       │   ├── magick.la
    │   │       │   ├── magick.so
    │   │       │   ├── map.la
    │   │       │   ├── map.so
    │   │       │   ├── mask.la
    │   │       │   ├── mask.so
    │   │       │   ├── mat.la
    │   │       │   ├── mat.so
    │   │       │   ├── matte.la
    │   │       │   ├── matte.so
    │   │       │   ├── meta.la
    │   │       │   ├── meta.so
    │   │       │   ├── miff.la
    │   │       │   ├── miff.so
    │   │       │   ├── mono.la
    │   │       │   ├── mono.so
    │   │       │   ├── mpc.la
    │   │       │   ├── mpc.so
    │   │       │   ├── mpr.la
    │   │       │   ├── mpr.so
    │   │       │   ├── msl.la
    │   │       │   ├── msl.so
    │   │       │   ├── mtv.la
    │   │       │   ├── mtv.so
    │   │       │   ├── mvg.la
    │   │       │   ├── mvg.so
    │   │       │   ├── null.la
    │   │       │   ├── null.so
    │   │       │   ├── ora.la
    │   │       │   ├── ora.so
    │   │       │   ├── otb.la
    │   │       │   ├── otb.so
    │   │       │   ├── palm.la
    │   │       │   ├── palm.so
    │   │       │   ├── pango.la
    │   │       │   ├── pango.so
    │   │       │   ├── pattern.la
    │   │       │   ├── pattern.so
    │   │       │   ├── pcd.la
    │   │       │   ├── pcd.so
    │   │       │   ├── pcl.la
    │   │       │   ├── pcl.so
    │   │       │   ├── pcx.la
    │   │       │   ├── pcx.so
    │   │       │   ├── pdb.la
    │   │       │   ├── pdb.so
    │   │       │   ├── pdf.la
    │   │       │   ├── pdf.so
    │   │       │   ├── pes.la
    │   │       │   ├── pes.so
    │   │       │   ├── pgx.la
    │   │       │   ├── pgx.so
    │   │       │   ├── pict.la
    │   │       │   ├── pict.so
    │   │       │   ├── pix.la
    │   │       │   ├── pix.so
    │   │       │   ├── plasma.la
    │   │       │   ├── plasma.so
    │   │       │   ├── pnm.la
    │   │       │   ├── pnm.so
    │   │       │   ├── ps2.la
    │   │       │   ├── ps2.so
    │   │       │   ├── ps3.la
    │   │       │   ├── ps3.so
    │   │       │   ├── psd.la
    │   │       │   ├── psd.so
    │   │       │   ├── ps.la
    │   │       │   ├── ps.so
    │   │       │   ├── pwp.la
    │   │       │   ├── pwp.so
    │   │       │   ├── qoi.la
    │   │       │   ├── qoi.so
    │   │       │   ├── raw.la
    │   │       │   ├── raw.so
    │   │       │   ├── rgb.la
    │   │       │   ├── rgb.so
    │   │       │   ├── rgf.la
    │   │       │   ├── rgf.so
    │   │       │   ├── rla.la
    │   │       │   ├── rla.so
    │   │       │   ├── rle.la
    │   │       │   ├── rle.so
    │   │       │   ├── scr.la
    │   │       │   ├── scr.so
    │   │       │   ├── sct.la
    │   │       │   ├── sct.so
    │   │       │   ├── sfw.la
    │   │       │   ├── sfw.so
    │   │       │   ├── sgi.la
    │   │       │   ├── sgi.so
    │   │       │   ├── sixel.la
    │   │       │   ├── sixel.so
    │   │       │   ├── stegano.la
    │   │       │   ├── stegano.so
    │   │       │   ├── strimg.la
    │   │       │   ├── strimg.so
    │   │       │   ├── sun.la
    │   │       │   ├── sun.so
    │   │       │   ├── svg.la
    │   │       │   ├── svg.so
    │   │       │   ├── tga.la
    │   │       │   ├── tga.so
    │   │       │   ├── thumbnail.la
    │   │       │   ├── thumbnail.so
    │   │       │   ├── tile.la
    │   │       │   ├── tile.so
    │   │       │   ├── tim2.la
    │   │       │   ├── tim2.so
    │   │       │   ├── tim.la
    │   │       │   ├── tim.so
    │   │       │   ├── ttf.la
    │   │       │   ├── ttf.so
    │   │       │   ├── txt.la
    │   │       │   ├── txt.so
    │   │       │   ├── uil.la
    │   │       │   ├── uil.so
    │   │       │   ├── url.la
    │   │       │   ├── url.so
    │   │       │   ├── uyvy.la
    │   │       │   ├── uyvy.so
    │   │       │   ├── vicar.la
    │   │       │   ├── vicar.so
    │   │       │   ├── video.la
    │   │       │   ├── video.so
    │   │       │   ├── vid.la
    │   │       │   ├── vid.so
    │   │       │   ├── viff.la
    │   │       │   ├── viff.so
    │   │       │   ├── vips.la
    │   │       │   ├── vips.so
    │   │       │   ├── wbmp.la
    │   │       │   ├── wbmp.so
    │   │       │   ├── wpg.la
    │   │       │   ├── wpg.so
    │   │       │   ├── xbm.la
    │   │       │   ├── xbm.so
    │   │       │   ├── xcf.la
    │   │       │   ├── xcf.so
    │   │       │   ├── xc.la
    │   │       │   ├── xc.so
    │   │       │   ├── xpm.la
    │   │       │   ├── xpm.so
    │   │       │   ├── xps.la
    │   │       │   ├── xps.so
    │   │       │   ├── yaml.la
    │   │       │   ├── yaml.so
    │   │       │   ├── ycbcr.la
    │   │       │   ├── ycbcr.so
    │   │       │   ├── yuv.la
    │   │       │   └── yuv.so
    │   │       └── filters
    │   │           ├── analyze.la
    │   │           └── analyze.so
    │   ├── libMagick++-7.Q16HDRI.a
    │   ├── libMagick++-7.Q16HDRI.la
    │   ├── libMagick++-7.Q16HDRI.so -> libMagick++-7.Q16HDRI.so.5.0.0
    │   ├── libMagick++-7.Q16HDRI.so.5 -> libMagick++-7.Q16HDRI.so.5.0.0
    │   ├── libMagick++-7.Q16HDRI.so.5.0.0
    │   ├── libMagickCore-7.Q16HDRI.a
    │   ├── libMagickCore-7.Q16HDRI.la
    │   ├── libMagickCore-7.Q16HDRI.so -> libMagickCore-7.Q16HDRI.so.10.0.1
    │   ├── libMagickCore-7.Q16HDRI.so.10 -> libMagickCore-7.Q16HDRI.so.10.0.1
    │   ├── libMagickCore-7.Q16HDRI.so.10.0.1
    │   ├── libMagickWand-7.Q16HDRI.a
    │   ├── libMagickWand-7.Q16HDRI.la
    │   ├── libMagickWand-7.Q16HDRI.so -> libMagickWand-7.Q16HDRI.so.10.0.1
    │   ├── libMagickWand-7.Q16HDRI.so.10 -> libMagickWand-7.Q16HDRI.so.10.0.1
    │   ├── libMagickWand-7.Q16HDRI.so.10.0.1
    │   ├── pkgconfig
    │   │   ├── ImageMagick-7.Q16HDRI.pc
    │   │   ├── ImageMagick.pc
    │   │   ├── Magick++-7.Q16HDRI.pc
    │   │   ├── MagickCore-7.Q16HDRI.pc
    │   │   ├── MagickCore.pc
    │   │   ├── Magick++.pc
    │   │   ├── MagickWand-7.Q16HDRI.pc
    │   │   └── MagickWand.pc
    │   └── x86_64-linux-gnu
    │       ├── libcairo.so.2 -> libcairo.so.2.11600.0
    │       ├── libcairo.so.2.11600.0
    │       ├── libdatrie.so.1 -> libdatrie.so.1.3.5
    │       ├── libdatrie.so.1.3.5
    │       ├── libde265.so.0 -> libde265.so.0.0.11
    │       ├── libde265.so.0.0.11
    │       ├── libdjvulibre.so.21 -> libdjvulibre.so.21.6.0
    │       ├── libdjvulibre.so.21.6.0
    │       ├── libfontconfig.so.1 -> libfontconfig.so.1.12.0
    │       ├── libfontconfig.so.1.12.0
    │       ├── libfreetype.so.6 -> libfreetype.so.6.17.1
    │       ├── libfreetype.so.6.17.1
    │       ├── libfribidi.so.0 -> libfribidi.so.0.4.0
    │       ├── libfribidi.so.0.4.0
    │       ├── libgomp.so.1 -> libgomp.so.1.0.0
    │       ├── libgomp.so.1.0.0
    │       ├── libgraphite2.so.2.0.0 -> libgraphite2.so.3
    │       ├── libgraphite2.so.3 -> libgraphite2.so.3.2.1
    │       ├── libgraphite2.so.3.2.1
    │       ├── libHalf.so.24 -> libHalf.so.24.0.0
    │       ├── libHalf.so.24.0.0
    │       ├── libharfbuzz.so.0 -> libharfbuzz.so.0.20600.4
    │       ├── libharfbuzz.so.0.20600.4
    │       ├── libheif.so.1 -> libheif.so.1.6.1
    │       ├── libheif.so.1.6.1
    │       ├── libicudata.so.66 -> libicudata.so.66.1
    │       ├── libicudata.so.66.1
    │       ├── libicui18n.so.66 -> libicui18n.so.66.1
    │       ├── libicui18n.so.66.1
    │       ├── libicuio.so.66 -> libicuio.so.66.1
    │       ├── libicuio.so.66.1
    │       ├── libicutest.so.66 -> libicutest.so.66.1
    │       ├── libicutest.so.66.1
    │       ├── libicutu.so.66 -> libicutu.so.66.1
    │       ├── libicutu.so.66.1
    │       ├── libicuuc.so.66 -> libicuuc.so.66.1
    │       ├── libicuuc.so.66.1
    │       ├── libIex-2_3.so.24 -> libIex-2_3.so.24.0.0
    │       ├── libIex-2_3.so.24.0.0
    │       ├── libIexMath-2_3.so.24 -> libIexMath-2_3.so.24.0.0
    │       ├── libIexMath-2_3.so.24.0.0
    │       ├── libIlmImf-2_3.so.24 -> libIlmImf-2_3.so.24.0.0
    │       ├── libIlmImf-2_3.so.24.0.0
    │       ├── libIlmImfUtil-2_3.so.24 -> libIlmImfUtil-2_3.so.24.0.0
    │       ├── libIlmImfUtil-2_3.so.24.0.0
    │       ├── libIlmThread-2_3.so.24 -> libIlmThread-2_3.so.24.0.0
    │       ├── libIlmThread-2_3.so.24.0.0
    │       ├── libImath-2_3.so.24 -> libImath-2_3.so.24.0.0
    │       ├── libImath-2_3.so.24.0.0
    │       ├── libjbig.so.0
    │       ├── libjpeg.so.8 -> libjpeg.so.8.2.2
    │       ├── libjpeg.so.8.2.2
    │       ├── liblcms2.so.2 -> liblcms2.so.2.0.8
    │       ├── liblcms2.so.2.0.8
    │       ├── liblqr-1.so.0 -> liblqr-1.so.0.3.2
    │       ├── liblqr-1.so.0.3.2
    │       ├── libltdl.so.7 -> libltdl.so.7.3.1
    │       ├── libltdl.so.7.3.1
    │       ├── libnuma.so.1 -> libnuma.so.1.0.0
    │       ├── libnuma.so.1.0.0
    │       ├── libopenjp2.so.2.3.1
    │       ├── libopenjp2.so.7 -> libopenjp2.so.2.3.1
    │       ├── libpango-1.0.so.0 -> libpango-1.0.so.0.4400.7
    │       ├── libpango-1.0.so.0.4400.7
    │       ├── libpangocairo-1.0.so.0 -> libpangocairo-1.0.so.0.4400.7
    │       ├── libpangocairo-1.0.so.0.4400.7
    │       ├── libpangoft2-1.0.so.0 -> libpangoft2-1.0.so.0.4400.7
    │       ├── libpangoft2-1.0.so.0.4400.7
    │       ├── libpixman-1.so.0 -> libpixman-1.so.0.38.4
    │       ├── libpixman-1.so.0.38.4
    │       ├── libpng16.so.16 -> libpng16.so.16.37.0
    │       ├── libpng16.so.16.37.0
    │       ├── libthai.so.0 -> libthai.so.0.3.1
    │       ├── libthai.so.0.3.1
    │       ├── libtiff.so.5 -> libtiff.so.5.5.0
    │       ├── libtiff.so.5.5.0
    │       ├── libwebpdemux.so.2 -> libwebpdemux.so.2.0.3
    │       ├── libwebpdemux.so.2.0.3
    │       ├── libwebpmux.so.3 -> libwebpmux.so.3.0.1
    │       ├── libwebpmux.so.3.0.1
    │       ├── libwebp.so.6 -> libwebp.so.6.0.2
    │       ├── libwebp.so.6.0.2
    │       ├── libwmf-0.2.so.7 -> libwmf-0.2.so.7.1.0
    │       ├── libwmf-0.2.so.7.1.0
    │       ├── libwmflite-0.2.so.7 -> libwmflite-0.2.so.7.0.1
    │       ├── libwmflite-0.2.so.7.0.1
    │       ├── libX11.so.6 -> libX11.so.6.3.0
    │       ├── libX11.so.6.3.0
    │       ├── libx265.so.179
    │       ├── libXau.so.6 -> libXau.so.6.0.0
    │       ├── libXau.so.6.0.0
    │       ├── libxcb-render.so.0 -> libxcb-render.so.0.0.0
    │       ├── libxcb-render.so.0.0.0
    │       ├── libxcb-shm.so.0 -> libxcb-shm.so.0.0.0
    │       ├── libxcb-shm.so.0.0.0
    │       ├── libxcb.so.1 -> libxcb.so.1.1.0
    │       ├── libxcb.so.1.1.0
    │       ├── libXdmcp.so.6 -> libXdmcp.so.6.0.0
    │       ├── libXdmcp.so.6.0.0
    │       ├── libXext.so.6 -> libXext.so.6.4.0
    │       ├── libXext.so.6.4.0
    │       ├── libxml2.so.2 -> libxml2.so.2.9.10
    │       ├── libxml2.so.2.9.10
    │       ├── libXrender.so.1 -> libXrender.so.1.3.0
    │       └── libXrender.so.1.3.0
    └── share
        ├── doc
        │   ├── fontconfig
        │   │   ├── changelog.Debian.gz -> ../libfontconfig1/changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── fontconfig-user.html
        │   │   ├── fontconfig-user.pdf.gz
        │   │   ├── fontconfig-user.txt.gz
        │   │   └── README.Debian
        │   ├── fontconfig-config
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── fonts-dejavu-core
        │   │   ├── AUTHORS
        │   │   ├── BUGS
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── langcover.txt.gz
        │   │   ├── README.md
        │   │   ├── status.txt.gz
        │   │   └── unicover.txt.gz
        │   ├── ImageMagick-7
        │   │   ├── images
        │   │   │   ├── affine.png
        │   │   │   ├── annotate.png
        │   │   │   ├── arc.png
        │   │   │   ├── atop.gif
        │   │   │   ├── background.jpg
        │   │   │   ├── bitcoin.svg
        │   │   │   ├── black.png
        │   │   │   ├── bluebells_clipped.jpg
        │   │   │   ├── bluebells_darker.jpg
        │   │   │   ├── bluebells_lin.jpg
        │   │   │   ├── bluebells_log.jpg
        │   │   │   ├── button.gif
        │   │   │   ├── color-thresholding.gif
        │   │   │   ├── color-thresholding-gray.gif
        │   │   │   ├── color-thresholding-hsv.gif
        │   │   │   ├── color-thresholding-hsv-rgb.gif
        │   │   │   ├── color-thresholding.jpg
        │   │   │   ├── color-thresholding-rgb.gif
        │   │   │   ├── configure.jpg
        │   │   │   ├── convex-hull-barn-closure.jpg
        │   │   │   ├── convex-hull-barn.jpg
        │   │   │   ├── convex-hull-blocks-closure.png
        │   │   │   ├── convex-hull-blocks.png
        │   │   │   ├── convex-hull.png
        │   │   │   ├── cylinder_shaded.png
        │   │   │   ├── difference.png
        │   │   │   ├── examples.jpg
        │   │   │   ├── frame.jpg
        │   │   │   ├── fuzzy-magick.png
        │   │   │   ├── gaussian-blur.png
        │   │   │   ├── granite.png
        │   │   │   ├── imade_art2.jpg
        │   │   │   ├── ImageMagick.ico
        │   │   │   ├── label.gif
        │   │   │   ├── logo.eps
        │   │   │   ├── logo.jpg
        │   │   │   ├── logo.png
        │   │   │   ├── logo-sm-flop.png
        │   │   │   ├── logo-sm-fx.png
        │   │   │   ├── logo-sm.png
        │   │   │   ├── montage.jpg
        │   │   │   ├── mountains-clahe.jpg
        │   │   │   ├── mountains-equalize.jpg
        │   │   │   ├── mountains.jpg
        │   │   │   ├── navy.png
        │   │   │   ├── objects.gif
        │   │   │   ├── objects.jpg
        │   │   │   ├── objects.png
        │   │   │   ├── over.gif
        │   │   │   ├── patterns
        │   │   │   │   ├── bricks.png
        │   │   │   │   ├── checkerboard.png
        │   │   │   │   ├── circles.png
        │   │   │   │   ├── crosshatch30.png
        │   │   │   │   ├── crosshatch45.png
        │   │   │   │   ├── crosshatch.png
        │   │   │   │   ├── fishscales.png
        │   │   │   │   ├── gray0.png
        │   │   │   │   ├── gray100.png
        │   │   │   │   ├── gray10.png
        │   │   │   │   ├── gray15.png
        │   │   │   │   ├── gray20.png
        │   │   │   │   ├── gray25.png
        │   │   │   │   ├── gray30.png
        │   │   │   │   ├── gray35.png
        │   │   │   │   ├── gray40.png
        │   │   │   │   ├── gray45.png
        │   │   │   │   ├── gray50.png
        │   │   │   │   ├── gray55.png
        │   │   │   │   ├── gray5.png
        │   │   │   │   ├── gray60.png
        │   │   │   │   ├── gray65.png
        │   │   │   │   ├── gray70.png
        │   │   │   │   ├── gray75.png
        │   │   │   │   ├── gray80.png
        │   │   │   │   ├── gray85.png
        │   │   │   │   ├── gray90.png
        │   │   │   │   ├── gray95.png
        │   │   │   │   ├── hexagons.png
        │   │   │   │   ├── horizontal2.png
        │   │   │   │   ├── horizontal3.png
        │   │   │   │   ├── horizontal.png
        │   │   │   │   ├── horizontalsaw.png
        │   │   │   │   ├── hs_bdiagonal.png
        │   │   │   │   ├── hs_cross.png
        │   │   │   │   ├── hs_diagcross.png
        │   │   │   │   ├── hs_fdiagonal.png
        │   │   │   │   ├── hs_horizontal.png
        │   │   │   │   ├── hs_vertical.png
        │   │   │   │   ├── left30.png
        │   │   │   │   ├── left45.png
        │   │   │   │   ├── leftshingle.png
        │   │   │   │   ├── octagons.png
        │   │   │   │   ├── right30.png
        │   │   │   │   ├── right45.png
        │   │   │   │   ├── rightshingle.png
        │   │   │   │   ├── smallfishscales.png
        │   │   │   │   ├── vertical2.png
        │   │   │   │   ├── vertical3.png
        │   │   │   │   ├── verticalbricks.png
        │   │   │   │   ├── verticalleftshingle.png
        │   │   │   │   ├── vertical.png
        │   │   │   │   ├── verticalrightshingle.png
        │   │   │   │   └── verticalsaw.png
        │   │   │   ├── piechart.png
        │   │   │   ├── radial-gradient.png
        │   │   │   ├── reconstruct.jpg
        │   │   │   ├── red-ball.png
        │   │   │   ├── red-circle.png
        │   │   │   ├── right.gif
        │   │   │   ├── rose.jpg
        │   │   │   ├── rose-over.png
        │   │   │   ├── rose.png
        │   │   │   ├── rose.pnm
        │   │   │   ├── rose-sigmoidal.png
        │   │   │   ├── script.png
        │   │   │   ├── smile.gif
        │   │   │   ├── sponsor.jpg
        │   │   │   ├── sprite.jpg
        │   │   │   ├── t-shirt.png
        │   │   │   ├── wand.ico
        │   │   │   ├── wand.png
        │   │   │   ├── white-highlight.png
        │   │   │   ├── wizard.jpg
        │   │   │   └── wizard.png
        │   │   ├── index.html
        │   │   ├── LICENSE
        │   │   ├── NEWS.txt
        │   │   └── www
        │   │       ├── advanced-linux-installation.html
        │   │       ├── advanced-unix-installation.html
        │   │       ├── advanced-windows-installation.html
        │   │       ├── animate.html
        │   │       ├── api
        │   │       │   ├── animate.html
        │   │       │   ├── annotate.html
        │   │       │   ├── attribute.html
        │   │       │   ├── blob.html
        │   │       │   ├── cache.html
        │   │       │   ├── cache-view.html
        │   │       │   ├── channel.html
        │   │       │   ├── cipher.html
        │   │       │   ├── color.html
        │   │       │   ├── colormap.html
        │   │       │   ├── colorspace.html
        │   │       │   ├── compare.html
        │   │       │   ├── composite.html
        │   │       │   ├── constitute.html
        │   │       │   ├── decorate.html
        │   │       │   ├── deprecate.html
        │   │       │   ├── display.html
        │   │       │   ├── distort.html
        │   │       │   ├── draw.html
        │   │       │   ├── drawing-wand.html
        │   │       │   ├── effect.html
        │   │       │   ├── enhance.html
        │   │       │   ├── exception.html
        │   │       │   ├── feature.html
        │   │       │   ├── fourier.html
        │   │       │   ├── fx.html
        │   │       │   ├── histogram.html
        │   │       │   ├── image.html
        │   │       │   ├── Image++.html
        │   │       │   ├── image-view.html
        │   │       │   ├── layer.html
        │   │       │   ├── list.html
        │   │       │   ├── magick++-classes.html
        │   │       │   ├── magick-deprecate.html
        │   │       │   ├── magick.html
        │   │       │   ├── magick-image.html
        │   │       │   ├── magick-property.html
        │   │       │   ├── magick-wand.html
        │   │       │   ├── memory.html
        │   │       │   ├── mime.html
        │   │       │   ├── module.html
        │   │       │   ├── mogrify.html
        │   │       │   ├── monitor.html
        │   │       │   ├── montage.html
        │   │       │   ├── morphology.html
        │   │       │   ├── paint.html
        │   │       │   ├── pixel-iterator.html
        │   │       │   ├── pixel-wand.html
        │   │       │   ├── profile.html
        │   │       │   ├── property.html
        │   │       │   ├── quantize.html
        │   │       │   ├── registry.html
        │   │       │   ├── resize.html
        │   │       │   ├── resource.html
        │   │       │   ├── segment.html
        │   │       │   ├── shear.html
        │   │       │   ├── signature.html
        │   │       │   ├── statistic.html
        │   │       │   ├── stream.html
        │   │       │   ├── transform.html
        │   │       │   ├── version.html
        │   │       │   ├── vision.html
        │   │       │   └── wand-view.html
        │   │       ├── architecture.html
        │   │       ├── assets
        │   │       │   ├── magick.css
        │   │       │   └── magick.js
        │   │       ├── changelog.html
        │   │       ├── cipher.html
        │   │       ├── cite.html
        │   │       ├── clahe.html
        │   │       ├── color.html
        │   │       ├── color-management.html
        │   │       ├── color-thresholding.html
        │   │       ├── command-line-options.html
        │   │       ├── command-line-processing.html
        │   │       ├── command-line-tools.html
        │   │       ├── compare.html
        │   │       ├── compose.html
        │   │       ├── composite.html
        │   │       ├── conjure.html
        │   │       ├── connected-components.html
        │   │       ├── contact.html
        │   │       ├── convert.html
        │   │       ├── convex-hull.html
        │   │       ├── defines.html
        │   │       ├── develop.html
        │   │       ├── display.html
        │   │       ├── distribute-pixel-cache.html
        │   │       ├── download.html
        │   │       ├── escape.html
        │   │       ├── examples.html
        │   │       ├── exception.html
        │   │       ├── export.html
        │   │       ├── favicon.ico
        │   │       ├── formats.html
        │   │       ├── fx.html
        │   │       ├── gradient.html
        │   │       ├── high-dynamic-range.html
        │   │       ├── history.html
        │   │       ├── identify.html
        │   │       ├── import.html
        │   │       ├── index.html
        │   │       ├── install-source.html
        │   │       ├── jp2.html
        │   │       ├── license.html
        │   │       ├── links.html
        │   │       ├── Magick++
        │   │       │   ├── Blob.html
        │   │       │   ├── Cache.fig
        │   │       │   ├── Cache.png
        │   │       │   ├── Cache.svg
        │   │       │   ├── ChangeLog.html
        │   │       │   ├── CoderInfo.html
        │   │       │   ├── Color.html
        │   │       │   ├── Documentation.html
        │   │       │   ├── Drawable_example_1.png
        │   │       │   ├── Drawable.html
        │   │       │   ├── Enumerations.html
        │   │       │   ├── Exception.html
        │   │       │   ├── FormatCharacters.html
        │   │       │   ├── Future.html
        │   │       │   ├── Geometry.html
        │   │       │   ├── ImageDesign.html
        │   │       │   ├── Image.fig
        │   │       │   ├── Image++.html
        │   │       │   ├── Image.html
        │   │       │   ├── ImageMagick.png
        │   │       │   ├── Image.png
        │   │       │   ├── index.html
        │   │       │   ├── Install.html
        │   │       │   ├── magick.css
        │   │       │   ├── Magick++.png
        │   │       │   ├── Montage.html
        │   │       │   ├── montage-sample-framed.jpg
        │   │       │   ├── NEWS.html
        │   │       │   ├── PixelPacket.html
        │   │       │   ├── Pixels.html
        │   │       │   ├── Quantum.html
        │   │       │   ├── README.txt
        │   │       │   ├── right_triangle.png
        │   │       │   ├── STL.html
        │   │       │   ├── thumbnail-anatomy-framed.fig
        │   │       │   ├── thumbnail-anatomy-framed.jpg
        │   │       │   ├── thumbnail-anatomy-plain.fig
        │   │       │   ├── thumbnail-anatomy-plain.jpg
        │   │       │   ├── thumbnail-sample-framed.jpg
        │   │       │   ├── thumbnail-sample-plain.jpg
        │   │       │   └── TypeMetric.html
        │   │       ├── magick-cache.html
        │   │       ├── magick-core.html
        │   │       ├── magick++.html
        │   │       ├── magick.html
        │   │       ├── magick-script.html
        │   │       ├── magick-vector-graphics.html
        │   │       ├── magick-wand.html
        │   │       ├── miff.html
        │   │       ├── mirror.html
        │   │       ├── mogrify.html
        │   │       ├── montage.html
        │   │       ├── motion-picture.html
        │   │       ├── multispectral-imagery.html
        │   │       ├── news.html
        │   │       ├── opencl.html
        │   │       ├── openmp.html
        │   │       ├── perl-magick.html
        │   │       ├── porting.html
        │   │       ├── quantize.html
        │   │       ├── resources.html
        │   │       ├── search.html
        │   │       ├── security-policy.html
        │   │       ├── sitemap.html
        │   │       ├── source
        │   │       │   ├── analyze.c
        │   │       │   ├── coder.xml
        │   │       │   ├── colors.xml
        │   │       │   ├── configure.xml
        │   │       │   ├── contrast.c
        │   │       │   ├── core.c
        │   │       │   ├── delegates.xml
        │   │       │   ├── english.xml
        │   │       │   ├── examples.pl
        │   │       │   ├── francais.xml
        │   │       │   ├── incantation.msl
        │   │       │   ├── locale.xml
        │   │       │   ├── log.xml
        │   │       │   ├── magic.xml
        │   │       │   ├── mgk.c
        │   │       │   ├── mime.xml
        │   │       │   ├── piechart.mvg
        │   │       │   ├── piechart.svg
        │   │       │   ├── policy.xml
        │   │       │   ├── quantization-table.xml
        │   │       │   ├── thresholds.xml
        │   │       │   ├── type-apple.xml
        │   │       │   ├── type-dejavu.xml
        │   │       │   ├── type-ghostscript.xml
        │   │       │   ├── type-urw-base35.xml
        │   │       │   ├── type-windows.xml
        │   │       │   ├── type.xml
        │   │       │   └── wand.c
        │   │       ├── stream.html
        │   │       ├── support.html
        │   │       ├── vpat.html
        │   │       ├── wand.png
        │   │       └── webp.html
        │   ├── libcairo2
        │   │   ├── AUTHORS.gz
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   └── README.gz
        │   ├── libdatrie1
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   └── README
        │   ├── libde265-0
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libdjvulibre21
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── NEWS.gz -> changelog.gz
        │   ├── libdjvulibre-text
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── NEWS.gz -> changelog.gz
        │   ├── libfontconfig1
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libfreetype6
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── README
        │   ├── libfribidi0
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   ├── README
        │   │   ├── THANKS
        │   │   └── TODO
        │   ├── libgomp1 -> gcc-10-base
        │   ├── libgraphite2-3
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libharfbuzz0b
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── TODO
        │   ├── libheif1
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libicu66
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libilmbase24
        │   │   ├── AUTHORS
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   └── README.md.gz
        │   ├── libjbig0
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libjpeg8
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libjpeg-turbo8
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── liblcms2-2
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── liblqr-1-0
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libltdl7
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   └── README
        │   ├── libnuma1
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libopenexr24
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libopenjp2-7
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libpango-1.0-0
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   ├── README.md
        │   │   └── THANKS
        │   ├── libpangocairo-1.0-0
        │   │   ├── changelog.Debian.gz -> ../libpango-1.0-0/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libpangoft2-1.0-0
        │   │   ├── changelog.Debian.gz -> ../libpango-1.0-0/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libpixman-1-0
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libpng16-16
        │   │   ├── ANNOUNCE
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── libpng-manual.txt.gz
        │   │   ├── README.gz
        │   │   └── TODO
        │   ├── libthai0
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libthai-data
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libtiff5
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libwebp6
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libwebpdemux2
        │   │   ├── changelog.Debian.gz -> ../libwebp6/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libwebpmux3
        │   │   ├── changelog.Debian.gz -> ../libwebp6/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libwmf0.2-7
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── CREDITS
        │   │   ├── README.gz
        │   │   ├── TODO
        │   │   └── TODO.Debian
        │   ├── libx11-6
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.Debian.gz
        │   │   └── NEWS.gz
        │   ├── libx11-data
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libx265-179
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxau6
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxcb1
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxcb-render0
        │   │   ├── changelog.Debian.gz -> ../libxcb1/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxcb-shm0
        │   │   ├── changelog.Debian.gz -> ../libxcb1/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxdmcp6
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxext6
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxml2
        │   │   ├── AUTHORS
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz -> changelog.gz
        │   │   ├── README
        │   │   └── README.Debian
        │   └── libxrender1
        │       ├── changelog.Debian.gz
        │       └── copyright
        ├── doc-base
        │   ├── fontconfig-user
        │   └── libpng16
        ├── fonts
        │   └── truetype
        │       └── dejavu
        │           ├── DejaVuSans-Bold.ttf
        │           ├── DejaVuSansMono-Bold.ttf
        │           ├── DejaVuSansMono.ttf
        │           ├── DejaVuSans.ttf
        │           ├── DejaVuSerif-Bold.ttf
        │           └── DejaVuSerif.ttf
        ├── ImageMagick-7
        │   ├── english.xml
        │   ├── francais.xml
        │   └── locale.xml
        ├── libthai
        │   └── thbrk.tri
        └── xml
            └── fontconfig
                └── fonts.dtd
```
