---
title: "PixelFormat"
second_title: "Aspose.Tasks for Java API Reference"
description: "Gibt das Format der Farbdaten für jedes Pixel im Bild an."
type: docs
weight: 193
url: /de/java/com.aspose.tasks/pixelformat/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class PixelFormat extends System.Enum
```

Gibt das Format der Farbdaten für jedes Pixel im Bild an.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [Alpha](#Alpha) | Die Pixeldaten enthalten Alphawerte, die nicht vorab multipliziert sind. |
| [Canonical](#Canonical) | Das Standard-Pixel-Format von 32 Bit pro Pixel. |
| [DontCare](#DontCare) | Kein Pixel-Format angegeben. |
| [Extended](#Extended) | Reserviert. |
| [Format16bppArgb1555](#Format16bppArgb1555) | Das Pixel-Format hat 16 Bit pro Pixel. |
| [Format16bppGrayScale](#Format16bppGrayScale) | Das Pixel-Format hat 16 Bit pro Pixel. |
| [Format16bppRgb555](#Format16bppRgb555) | Gibt an, dass das Format 16 Bit pro Pixel beträgt; jeweils 5 Bit werden für die roten, grünen und blauen Komponenten verwendet. |
| [Format16bppRgb565](#Format16bppRgb565) | Gibt an, dass das Format 16 Bit pro Pixel beträgt; 5 Bit werden für die rote Komponente, 6 Bit für die grüne Komponente und 5 Bit für die blaue Komponente verwendet. |
| [Format1bppIndexed](#Format1bppIndexed) | Gibt an, dass das Pixel-Format 1 Bit pro Pixel beträgt und indizierte Farben verwendet. |
| [Format24bppRgb](#Format24bppRgb) | Gibt an, dass das Format 24 Bit pro Pixel beträgt; jeweils 8 Bit werden für die roten, grünen und blauen Komponenten verwendet. |
| [Format32bppArgb](#Format32bppArgb) | Gibt an, dass das Format 32 Bit pro Pixel beträgt; jeweils 8 Bit werden für die Alpha-, Rot-, Grün- und Blaukomponenten verwendet. |
| [Format32bppPArgb](#Format32bppPArgb) | Gibt an, dass das Format 32 Bit pro Pixel beträgt; jeweils 8 Bit werden für die Alpha-, Rot-, Grün- und Blaukomponenten verwendet. |
| [Format32bppRgb](#Format32bppRgb) | Gibt an, dass das Format 32 Bit pro Pixel beträgt; jeweils 8 Bit werden für die roten, grünen und blauen Komponenten verwendet. |
| [Format48bppRgb](#Format48bppRgb) | Gibt an, dass das Format 48 Bit pro Pixel beträgt; jeweils 16 Bit für die roten, grünen und blauen Komponenten verwendet werden. |
| [Format4bppIndexed](#Format4bppIndexed) | Gibt an, dass das Format 4 Bit pro Pixel beträgt, indiziert. |
| [Format64bppArgb](#Format64bppArgb) | Gibt an, dass das Format 64 Bit pro Pixel beträgt; jeweils 16 Bit für die Alpha-, Rot-, Grün- und Blaukomponenten verwendet werden. |
| [Format64bppPArgb](#Format64bppPArgb) | Gibt an, dass das Format 64 Bit pro Pixel beträgt; jeweils 16 Bit für die Alpha-, Rot-, Grün- und Blaukomponenten verwendet werden. |
| [Format8bppIndexed](#Format8bppIndexed) | Gibt an, dass das Format 8 Bit pro Pixel beträgt, indiziert. |
| [Gdi](#Gdi) | Die Pixeldaten enthalten GDI‑Farben. |
| [Indexed](#Indexed) | Die Pixeldaten enthalten farbindizierte Werte, was bedeutet, dass die Werte ein Index zu Farben in der Systemfarbtabelle sind, im Gegensatz zu einzelnen Farbwerten. |
| [Max](#Max) | Der Maximalwert für diese Aufzählung. |
| [PAlpha](#PAlpha) | Das Pixelformat enthält vorvermultiplizierte Alpha‑Werte. |
| [Undefined](#Undefined) | Das Pixelformat ist undefiniert. |
### Alpha {#Alpha}
```
public static final int Alpha
```


Die Pixeldaten enthalten Alphawerte, die nicht vorab multipliziert sind.

### Canonical {#Canonical}
```
public static final int Canonical
```


Das Standard‑Pixelformat von 32 Bit pro Pixel. Das Format gibt eine Farbtiefe von 24 Bit und einen 8‑Bit‑Alpha‑Kanal an.

### DontCare {#DontCare}
```
public static final int DontCare
```


Kein Pixel-Format angegeben.

### Extended {#Extended}
```
public static final int Extended
```


Reserviert.

### Format16bppArgb1555 {#Format16bppArgb1555}
```
public static final int Format16bppArgb1555
```


Das Pixelformat beträgt 16 Bit pro Pixel. Die Farbinformation gibt 32.768 Farbabstufungen an, wobei 5 Bit Rot, 5 Bit Grün, 5 Bit Blau und 1 Bit Alpha sind.

### Format16bppGrayScale {#Format16bppGrayScale}
```
public static final int Format16bppGrayScale
```


Das Pixelformat beträgt 16 Bit pro Pixel. Die Farbinformation gibt 65.536 Graustufen an.

### Format16bppRgb555 {#Format16bppRgb555}
```
public static final int Format16bppRgb555
```


Gibt an, dass das Format 16 Bit pro Pixel beträgt; jeweils 5 Bit für die roten, grünen und blauen Komponenten verwendet werden. Das verbleibende Bit wird nicht verwendet.

### Format16bppRgb565 {#Format16bppRgb565}
```
public static final int Format16bppRgb565
```


Gibt an, dass das Format 16 Bit pro Pixel beträgt; 5 Bit werden für die rote Komponente, 6 Bit für die grüne Komponente und 5 Bit für die blaue Komponente verwendet.

### Format1bppIndexed {#Format1bppIndexed}
```
public static final int Format1bppIndexed
```


Gibt an, dass das Pixelformat 1 Bit pro Pixel beträgt und indizierte Farben verwendet. Die Farbpalette enthält daher zwei Farben.

### Format24bppRgb {#Format24bppRgb}
```
public static final int Format24bppRgb
```


Gibt an, dass das Format 24 Bit pro Pixel beträgt; jeweils 8 Bit werden für die roten, grünen und blauen Komponenten verwendet.

### Format32bppArgb {#Format32bppArgb}
```
public static final int Format32bppArgb
```


Gibt an, dass das Format 32 Bit pro Pixel beträgt; jeweils 8 Bit werden für die Alpha-, Rot-, Grün- und Blaukomponenten verwendet.

### Format32bppPArgb {#Format32bppPArgb}
```
public static final int Format32bppPArgb
```


Gibt an, dass das Format 32 Bit pro Pixel beträgt; jeweils 8 Bit für die Alpha-, Rot-, Grün- und Blaukomponenten verwendet werden. Die Rot-, Grün- und Blaukomponenten sind gemäß der Alpha‑Komponente vorvermultipliziert.

### Format32bppRgb {#Format32bppRgb}
```
public static final int Format32bppRgb
```


Gibt an, dass das Format 32 Bit pro Pixel beträgt; jeweils 8 Bit für die Rot-, Grün- und Blaukomponenten verwendet werden. Die verbleibenden 8 Bit werden nicht verwendet.

### Format48bppRgb {#Format48bppRgb}
```
public static final int Format48bppRgb
```


Gibt an, dass das Format 48 Bit pro Pixel beträgt; jeweils 16 Bit für die roten, grünen und blauen Komponenten verwendet werden.

### Format4bppIndexed {#Format4bppIndexed}
```
public static final int Format4bppIndexed
```


Gibt an, dass das Format 4 Bit pro Pixel beträgt, indiziert.

### Format64bppArgb {#Format64bppArgb}
```
public static final int Format64bppArgb
```


Gibt an, dass das Format 64 Bit pro Pixel beträgt; jeweils 16 Bit für die Alpha-, Rot-, Grün- und Blaukomponenten verwendet werden.

### Format64bppPArgb {#Format64bppPArgb}
```
public static final int Format64bppPArgb
```


Gibt an, dass das Format 64 Bit pro Pixel beträgt; jeweils 16 Bit für die Alpha-, Rot-, Grün- und Blaukomponenten verwendet werden. Die Rot-, Grün- und Blaukomponenten sind gemäß der Alpha‑Komponente vorvermultipliziert.

### Format8bppIndexed {#Format8bppIndexed}
```
public static final int Format8bppIndexed
```


Gibt an, dass das Format 8 Bit pro Pixel beträgt, indiziert. Die Farbpalette enthält daher 256 Farben.

### Gdi {#Gdi}
```
public static final int Gdi
```


Die Pixeldaten enthalten GDI‑Farben.

### Indexed {#Indexed}
```
public static final int Indexed
```


Die Pixeldaten enthalten farbindizierte Werte, was bedeutet, dass die Werte ein Index zu Farben in der Systemfarbtabelle sind, im Gegensatz zu einzelnen Farbwerten.

### Max {#Max}
```
public static final int Max
```


Der Maximalwert für diese Aufzählung.

### PAlpha {#PAlpha}
```
public static final int PAlpha
```


Das Pixelformat enthält vorvermultiplizierte Alpha‑Werte.

### Undefined {#Undefined}
```
public static final int Undefined
```


Das Pixelformat ist undefiniert.

