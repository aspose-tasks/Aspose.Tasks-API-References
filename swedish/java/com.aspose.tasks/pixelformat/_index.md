---
title: "PixelFormat"
second_title: "Aspose.Tasks for Java API-referens"
description: "Anger formatet för färgdata för varje pixel i bilden."
type: docs
weight: 193
url: /sv/java/com.aspose.tasks/pixelformat/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class PixelFormat extends System.Enum
```

Anger formatet för färgdata för varje pixel i bilden.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [Alpha](#Alpha) | Pixeldata innehåller alfavärden som inte är förmultiplicerade. |
| [Canonical](#Canonical) | Standardpixelformatet är 32 bitar per pixel. |
| [DontCare](#DontCare) | Ingen pixelformat har angetts. |
| [Extended](#Extended) | Reserverad. |
| [Format16bppArgb1555](#Format16bppArgb1555) | Pixelformatet är 16 bitar per pixel. |
| [Format16bppGrayScale](#Format16bppGrayScale) | Pixelformatet är 16 bitar per pixel. |
| [Format16bppRgb555](#Format16bppRgb555) | Anger att formatet är 16 bitar per pixel; 5 bitar vardera används för de röda, gröna och blå komponenterna. |
| [Format16bppRgb565](#Format16bppRgb565) | Anger att formatet är 16 bitar per pixel; 5 bitar används för den röda komponenten, 6 bitar för den gröna komponenten och 5 bitar för den blå komponenten. |
| [Format1bppIndexed](#Format1bppIndexed) | Anger att pixelformatet är 1 bit per pixel och att det använder indexerad färg. |
| [Format24bppRgb](#Format24bppRgb) | Anger att formatet är 24 bitar per pixel; 8 bitar vardera används för de röda, gröna och blå komponenterna. |
| [Format32bppArgb](#Format32bppArgb) | Anger att formatet är 32 bitar per pixel; 8 bitar vardera används för alfakanalen, de röda, gröna och blå komponenterna. |
| [Format32bppPArgb](#Format32bppPArgb) | Anger att formatet är 32 bitar per pixel; 8 bitar vardera används för alfakanalen, de röda, gröna och blå komponenterna. |
| [Format32bppRgb](#Format32bppRgb) | Anger att formatet är 32 bitar per pixel; 8 bitar vardera används för de röda, gröna och blå komponenterna. |
| [Format48bppRgb](#Format48bppRgb) | Anger att formatet är 48 bitar per pixel; 16 bitar vardera används för de röda, gröna och blå komponenterna. |
| [Format4bppIndexed](#Format4bppIndexed) | Anger att formatet är 4 bitar per pixel, indexerat. |
| [Format64bppArgb](#Format64bppArgb) | Anger att formatet är 64 bitar per pixel; 16 bitar vardera används för alfakanalen, de röda, gröna och blå komponenterna. |
| [Format64bppPArgb](#Format64bppPArgb) | Anger att formatet är 64 bitar per pixel; 16 bitar vardera används för alfakanalen, de röda, gröna och blå komponenterna. |
| [Format8bppIndexed](#Format8bppIndexed) | Anger att formatet är 8 bitar per pixel, indexerat. |
| [Gdi](#Gdi) | Pixeldata innehåller GDI-färger. |
| [Indexed](#Indexed) | Pixeldata innehåller färgindexerade värden, vilket betyder att värdena är ett index till färger i systemets färgtabell, snarare än enskilda färgvärden. |
| [Max](#Max) | Det maximala värdet för den här uppräkningen. |
| [PAlpha](#PAlpha) | Pixelformatet innehåller förmultiplicerade alfavärden. |
| [Undefined](#Undefined) | Pixelformatet är odefinierat. |
### Alpha {#Alpha}
```
public static final int Alpha
```


Pixeldata innehåller alfavärden som inte är förmultiplicerade.

### Canonical {#Canonical}
```
public static final int Canonical
```


Standardpixelformatet är 32 bitar per pixel. Formatet specificerar 24-bitars färgdjup och en 8-bitars alfakanal.

### DontCare {#DontCare}
```
public static final int DontCare
```


Ingen pixelformat har angetts.

### Extended {#Extended}
```
public static final int Extended
```


Reserverad.

### Format16bppArgb1555 {#Format16bppArgb1555}
```
public static final int Format16bppArgb1555
```


Pixelformatet är 16 bitar per pixel. Färginformationen specificerar 32 768 färgnyanser, varav 5 bitar är röd, 5 bitar är grön, 5 bitar är blå och 1 bit är alfa.

### Format16bppGrayScale {#Format16bppGrayScale}
```
public static final int Format16bppGrayScale
```


Pixelformatet är 16 bitar per pixel. Färginformationen specificerar 65 536 gråskala nyanser.

### Format16bppRgb555 {#Format16bppRgb555}
```
public static final int Format16bppRgb555
```


Specificerar att formatet är 16 bitar per pixel; 5 bitar vardera används för de röda, gröna och blå komponenterna. Den återstående biten används inte.

### Format16bppRgb565 {#Format16bppRgb565}
```
public static final int Format16bppRgb565
```


Anger att formatet är 16 bitar per pixel; 5 bitar används för den röda komponenten, 6 bitar för den gröna komponenten och 5 bitar för den blå komponenten.

### Format1bppIndexed {#Format1bppIndexed}
```
public static final int Format1bppIndexed
```


Specificerar att pixelformatet är 1 bit per pixel och att det använder indexerad färg. Färgtabellen har därför två färger.

### Format24bppRgb {#Format24bppRgb}
```
public static final int Format24bppRgb
```


Anger att formatet är 24 bitar per pixel; 8 bitar vardera används för de röda, gröna och blå komponenterna.

### Format32bppArgb {#Format32bppArgb}
```
public static final int Format32bppArgb
```


Anger att formatet är 32 bitar per pixel; 8 bitar vardera används för alfakanalen, de röda, gröna och blå komponenterna.

### Format32bppPArgb {#Format32bppPArgb}
```
public static final int Format32bppPArgb
```


Specificerar att formatet är 32 bitar per pixel; 8 bitar vardera används för alfakanalen, röd, grön och blå komponenter. De röda, gröna och blå komponenterna är förmultiplicerade enligt alfakanalen.

### Format32bppRgb {#Format32bppRgb}
```
public static final int Format32bppRgb
```


Specificerar att formatet är 32 bitar per pixel; 8 bitar vardera används för de röda, gröna och blå komponenterna. De återstående 8 bitarna används inte.

### Format48bppRgb {#Format48bppRgb}
```
public static final int Format48bppRgb
```


Anger att formatet är 48 bitar per pixel; 16 bitar vardera används för de röda, gröna och blå komponenterna.

### Format4bppIndexed {#Format4bppIndexed}
```
public static final int Format4bppIndexed
```


Anger att formatet är 4 bitar per pixel, indexerat.

### Format64bppArgb {#Format64bppArgb}
```
public static final int Format64bppArgb
```


Anger att formatet är 64 bitar per pixel; 16 bitar vardera används för alfakanalen, de röda, gröna och blå komponenterna.

### Format64bppPArgb {#Format64bppPArgb}
```
public static final int Format64bppPArgb
```


Specificerar att formatet är 64 bitar per pixel; 16 bitar vardera används för alfakanalen, röd, grön och blå komponenter. De röda, gröna och blå komponenterna är förmultiplicerade enligt alfakanalen.

### Format8bppIndexed {#Format8bppIndexed}
```
public static final int Format8bppIndexed
```


Specificerar att formatet är 8 bitar per pixel, indexerat. Färgtabellen har därför 256 färger.

### Gdi {#Gdi}
```
public static final int Gdi
```


Pixeldata innehåller GDI-färger.

### Indexed {#Indexed}
```
public static final int Indexed
```


Pixeldata innehåller färgindexerade värden, vilket betyder att värdena är ett index till färger i systemets färgtabell, snarare än enskilda färgvärden.

### Max {#Max}
```
public static final int Max
```


Det maximala värdet för den här uppräkningen.

### PAlpha {#PAlpha}
```
public static final int PAlpha
```


Pixelformatet innehåller förmultiplicerade alfavärden.

### Undefined {#Undefined}
```
public static final int Undefined
```


Pixelformatet är odefinierat.

