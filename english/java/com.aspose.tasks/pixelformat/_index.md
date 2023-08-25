---
title: PixelFormat
second_title: Aspose.Tasks for Java API Reference
description: Specifies the format of the color data for each pixel in the image.
type: docs
weight: 182
url: /java/com.aspose.tasks/pixelformat/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class PixelFormat extends System.Enum
```

Specifies the format of the color data for each pixel in the image.
## Fields

| Field | Description |
| --- | --- |
| [Alpha](#Alpha) | The pixel data contains alpha values that are not premultiplied. |
| [Canonical](#Canonical) | The default pixel format of 32 bits per pixel. |
| [DontCare](#DontCare) | No pixel format is specified. |
| [Extended](#Extended) | Reserved. |
| [Format16bppArgb1555](#Format16bppArgb1555) | The pixel format is 16 bits per pixel. |
| [Format16bppGrayScale](#Format16bppGrayScale) | The pixel format is 16 bits per pixel. |
| [Format16bppRgb555](#Format16bppRgb555) | Specifies that the format is 16 bits per pixel; 5 bits each are used for the red, green, and blue components. |
| [Format16bppRgb565](#Format16bppRgb565) | Specifies that the format is 16 bits per pixel; 5 bits are used for the red component, 6 bits are used for the green component, and 5 bits are used for the blue component. |
| [Format1bppIndexed](#Format1bppIndexed) | Specifies that the pixel format is 1 bit per pixel and that it uses indexed color. |
| [Format24bppRgb](#Format24bppRgb) | Specifies that the format is 24 bits per pixel; 8 bits each are used for the red, green, and blue components. |
| [Format32bppArgb](#Format32bppArgb) | Specifies that the format is 32 bits per pixel; 8 bits each are used for the alpha, red, green, and blue components. |
| [Format32bppPArgb](#Format32bppPArgb) | Specifies that the format is 32 bits per pixel; 8 bits each are used for the alpha, red, green, and blue components. |
| [Format32bppRgb](#Format32bppRgb) | Specifies that the format is 32 bits per pixel; 8 bits each are used for the red, green, and blue components. |
| [Format48bppRgb](#Format48bppRgb) | Specifies that the format is 48 bits per pixel; 16 bits each are used for the red, green, and blue components. |
| [Format4bppIndexed](#Format4bppIndexed) | Specifies that the format is 4 bits per pixel, indexed. |
| [Format64bppArgb](#Format64bppArgb) | Specifies that the format is 64 bits per pixel; 16 bits each are used for the alpha, red, green, and blue components. |
| [Format64bppPArgb](#Format64bppPArgb) | Specifies that the format is 64 bits per pixel; 16 bits each are used for the alpha, red, green, and blue components. |
| [Format8bppIndexed](#Format8bppIndexed) | Specifies that the format is 8 bits per pixel, indexed. |
| [Gdi](#Gdi) | The pixel data contains GDI colors. |
| [Indexed](#Indexed) | The pixel data contains color-indexed values, which means the values are an index to colors in the system color table, as opposed to individual color values. |
| [Max](#Max) | The maximum value for this enumeration. |
| [PAlpha](#PAlpha) | The pixel format contains premultiplied alpha values. |
| [Undefined](#Undefined) | The pixel format is undefined. |
### Alpha {#Alpha}
```
public static final int Alpha
```


The pixel data contains alpha values that are not premultiplied.

### Canonical {#Canonical}
```
public static final int Canonical
```


The default pixel format of 32 bits per pixel. The format specifies 24-bit color depth and an 8-bit alpha channel.

### DontCare {#DontCare}
```
public static final int DontCare
```


No pixel format is specified.

### Extended {#Extended}
```
public static final int Extended
```


Reserved.

### Format16bppArgb1555 {#Format16bppArgb1555}
```
public static final int Format16bppArgb1555
```


The pixel format is 16 bits per pixel. The color information specifies 32,768 shades of color, of which 5 bits are red, 5 bits are green, 5 bits are blue, and 1 bit is alpha.

### Format16bppGrayScale {#Format16bppGrayScale}
```
public static final int Format16bppGrayScale
```


The pixel format is 16 bits per pixel. The color information specifies 65536 shades of gray.

### Format16bppRgb555 {#Format16bppRgb555}
```
public static final int Format16bppRgb555
```


Specifies that the format is 16 bits per pixel; 5 bits each are used for the red, green, and blue components. The remaining bit is not used.

### Format16bppRgb565 {#Format16bppRgb565}
```
public static final int Format16bppRgb565
```


Specifies that the format is 16 bits per pixel; 5 bits are used for the red component, 6 bits are used for the green component, and 5 bits are used for the blue component.

### Format1bppIndexed {#Format1bppIndexed}
```
public static final int Format1bppIndexed
```


Specifies that the pixel format is 1 bit per pixel and that it uses indexed color. The color table therefore has two colors in it.

### Format24bppRgb {#Format24bppRgb}
```
public static final int Format24bppRgb
```


Specifies that the format is 24 bits per pixel; 8 bits each are used for the red, green, and blue components.

### Format32bppArgb {#Format32bppArgb}
```
public static final int Format32bppArgb
```


Specifies that the format is 32 bits per pixel; 8 bits each are used for the alpha, red, green, and blue components.

### Format32bppPArgb {#Format32bppPArgb}
```
public static final int Format32bppPArgb
```


Specifies that the format is 32 bits per pixel; 8 bits each are used for the alpha, red, green, and blue components. The red, green, and blue components are premultiplied, according to the alpha component.

### Format32bppRgb {#Format32bppRgb}
```
public static final int Format32bppRgb
```


Specifies that the format is 32 bits per pixel; 8 bits each are used for the red, green, and blue components. The remaining 8 bits are not used.

### Format48bppRgb {#Format48bppRgb}
```
public static final int Format48bppRgb
```


Specifies that the format is 48 bits per pixel; 16 bits each are used for the red, green, and blue components.

### Format4bppIndexed {#Format4bppIndexed}
```
public static final int Format4bppIndexed
```


Specifies that the format is 4 bits per pixel, indexed.

### Format64bppArgb {#Format64bppArgb}
```
public static final int Format64bppArgb
```


Specifies that the format is 64 bits per pixel; 16 bits each are used for the alpha, red, green, and blue components.

### Format64bppPArgb {#Format64bppPArgb}
```
public static final int Format64bppPArgb
```


Specifies that the format is 64 bits per pixel; 16 bits each are used for the alpha, red, green, and blue components. The red, green, and blue components are premultiplied according to the alpha component.

### Format8bppIndexed {#Format8bppIndexed}
```
public static final int Format8bppIndexed
```


Specifies that the format is 8 bits per pixel, indexed. The color table therefore has 256 colors in it.

### Gdi {#Gdi}
```
public static final int Gdi
```


The pixel data contains GDI colors.

### Indexed {#Indexed}
```
public static final int Indexed
```


The pixel data contains color-indexed values, which means the values are an index to colors in the system color table, as opposed to individual color values.

### Max {#Max}
```
public static final int Max
```


The maximum value for this enumeration.

### PAlpha {#PAlpha}
```
public static final int PAlpha
```


The pixel format contains premultiplied alpha values.

### Undefined {#Undefined}
```
public static final int Undefined
```


The pixel format is undefined.

