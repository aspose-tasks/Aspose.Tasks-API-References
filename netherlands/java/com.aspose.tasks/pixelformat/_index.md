---
title: "PixelFormat"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Specificeert het formaat van de kleurgegevens voor elke pixel in de afbeelding."
type: docs
weight: 193
url: /nl/java/com.aspose.tasks/pixelformat/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class PixelFormat extends System.Enum
```

Specificeert het formaat van de kleurgegevens voor elke pixel in de afbeelding.
## Velden

| Veld | Beschrijving |
| --- | --- |
| [Alpha](#Alpha) | De pixelgegevens bevatten alfa-waarden die niet voorvermenigvuldigd zijn. |
| [Canonical](#Canonical) | Het standaard pixelformaat van 32 bits per pixel. |
| [DontCare](#DontCare) | Er is geen pixelindeling gespecificeerd. |
| [Extended](#Extended) | Gereserveerd. |
| [Format16bppArgb1555](#Format16bppArgb1555) | De pixelindeling is 16 bits per pixel. |
| [Format16bppGrayScale](#Format16bppGrayScale) | De pixelindeling is 16 bits per pixel. |
| [Format16bppRgb555](#Format16bppRgb555) | Geeft aan dat de indeling 16 bits per pixel is; 5 bits elk worden gebruikt voor de rode, groene en blauwe componenten. |
| [Format16bppRgb565](#Format16bppRgb565) | Geeft aan dat de indeling 16 bits per pixel is; 5 bits worden gebruikt voor de rode component, 6 bits voor de groene component en 5 bits voor de blauwe component. |
| [Format1bppIndexed](#Format1bppIndexed) | Geeft aan dat de pixelindeling 1 bit per pixel is en dat er geïndexeerde kleuren worden gebruikt. |
| [Format24bppRgb](#Format24bppRgb) | Geeft aan dat de indeling 24 bits per pixel is; 8 bits elk worden gebruikt voor de rode, groene en blauwe componenten. |
| [Format32bppArgb](#Format32bppArgb) | Geeft aan dat de indeling 32 bits per pixel is; 8 bits elk worden gebruikt voor de alfa-, rode, groene en blauwe componenten. |
| [Format32bppPArgb](#Format32bppPArgb) | Geeft aan dat de indeling 32 bits per pixel is; 8 bits elk worden gebruikt voor de alfa-, rode, groene en blauwe componenten. |
| [Format32bppRgb](#Format32bppRgb) | Geeft aan dat de indeling 32 bits per pixel is; 8 bits elk worden gebruikt voor de rode, groene en blauwe componenten. |
| [Format48bppRgb](#Format48bppRgb) | Geeft aan dat de indeling 48 bits per pixel is; 16 bits elk worden gebruikt voor de rode, groene en blauwe componenten. |
| [Format4bppIndexed](#Format4bppIndexed) | Geeft aan dat de indeling 4 bits per pixel is, geïndexeerd. |
| [Format64bppArgb](#Format64bppArgb) | Geeft aan dat de indeling 64 bits per pixel is; 16 bits elk worden gebruikt voor de alfa-, rode, groene en blauwe componenten. |
| [Format64bppPArgb](#Format64bppPArgb) | Geeft aan dat de indeling 64 bits per pixel is; 16 bits elk worden gebruikt voor de alfa-, rode, groene en blauwe componenten. |
| [Format8bppIndexed](#Format8bppIndexed) | Geeft aan dat de indeling 8 bits per pixel is, geïndexeerd. |
| [Gdi](#Gdi) | De pixelgegevens bevatten GDI-kleuren. |
| [Indexed](#Indexed) | De pixelgegevens bevatten kleurgeïndexeerde waarden, wat betekent dat de waarden een index naar kleuren in de systeemtabel zijn, in plaats van individuele kleurwaarden. |
| [Max](#Max) | De maximale waarde voor deze enumeratie. |
| [PAlpha](#PAlpha) | De pixelindeling bevat voorvermenigvuldigde alfa-waarden. |
| [Undefined](#Undefined) | De pixelindeling is niet gedefinieerd. |
### Alpha {#Alpha}
```
public static final int Alpha
```


De pixelgegevens bevatten alfa-waarden die niet voorvermenigvuldigd zijn.

### Canonical {#Canonical}
```
public static final int Canonical
```


De standaard pixelindeling van 32 bits per pixel. De indeling specificeert een kleurdiepte van 24 bits en een alfa-kanaal van 8 bits.

### DontCare {#DontCare}
```
public static final int DontCare
```


Er is geen pixelindeling gespecificeerd.

### Extended {#Extended}
```
public static final int Extended
```


Gereserveerd.

### Format16bppArgb1555 {#Format16bppArgb1555}
```
public static final int Format16bppArgb1555
```


De pixelindeling is 16 bits per pixel. De kleurinformatie specificeert 32.768 kleurschakeringen, waarvan 5 bits rood, 5 bits groen, 5 bits blauw en 1 bit alfa.

### Format16bppGrayScale {#Format16bppGrayScale}
```
public static final int Format16bppGrayScale
```


De pixelindeling is 16 bits per pixel. De kleurinformatie specificeert 65.536 grijstinten.

### Format16bppRgb555 {#Format16bppRgb555}
```
public static final int Format16bppRgb555
```


Geeft aan dat de indeling 16 bits per pixel is; 5 bits elk worden gebruikt voor de rode, groene en blauwe componenten. Het resterende bit wordt niet gebruikt.

### Format16bppRgb565 {#Format16bppRgb565}
```
public static final int Format16bppRgb565
```


Geeft aan dat de indeling 16 bits per pixel is; 5 bits worden gebruikt voor de rode component, 6 bits voor de groene component en 5 bits voor de blauwe component.

### Format1bppIndexed {#Format1bppIndexed}
```
public static final int Format1bppIndexed
```


Geeft aan dat de pixelindeling 1 bit per pixel is en dat er geïndexeerde kleuren worden gebruikt. De kleurentabel bevat daarom twee kleuren.

### Format24bppRgb {#Format24bppRgb}
```
public static final int Format24bppRgb
```


Geeft aan dat de indeling 24 bits per pixel is; 8 bits elk worden gebruikt voor de rode, groene en blauwe componenten.

### Format32bppArgb {#Format32bppArgb}
```
public static final int Format32bppArgb
```


Geeft aan dat de indeling 32 bits per pixel is; 8 bits elk worden gebruikt voor de alfa-, rode, groene en blauwe componenten.

### Format32bppPArgb {#Format32bppPArgb}
```
public static final int Format32bppPArgb
```


Geeft aan dat de indeling 32 bits per pixel is; 8 bits elk worden gebruikt voor de alfa-, rode, groene en blauwe componenten. De rode, groene en blauwe componenten zijn voorvermenigvuldigd volgens de alfa-component.

### Format32bppRgb {#Format32bppRgb}
```
public static final int Format32bppRgb
```


Geeft aan dat de indeling 32 bits per pixel is; 8 bits elk worden gebruikt voor de rode, groene en blauwe componenten. De resterende 8 bits worden niet gebruikt.

### Format48bppRgb {#Format48bppRgb}
```
public static final int Format48bppRgb
```


Geeft aan dat de indeling 48 bits per pixel is; 16 bits elk worden gebruikt voor de rode, groene en blauwe componenten.

### Format4bppIndexed {#Format4bppIndexed}
```
public static final int Format4bppIndexed
```


Geeft aan dat de indeling 4 bits per pixel is, geïndexeerd.

### Format64bppArgb {#Format64bppArgb}
```
public static final int Format64bppArgb
```


Geeft aan dat de indeling 64 bits per pixel is; 16 bits elk worden gebruikt voor de alfa-, rode, groene en blauwe componenten.

### Format64bppPArgb {#Format64bppPArgb}
```
public static final int Format64bppPArgb
```


Specificeert dat het formaat 64 bits per pixel is; 16 bits elk worden gebruikt voor de alpha-, rood-, groen- en blauwcomponenten. De rood-, groen- en blauwcomponenten zijn voorvermenigvuldigd volgens de alpha-component.

### Format8bppIndexed {#Format8bppIndexed}
```
public static final int Format8bppIndexed
```


Specificeert dat het formaat 8 bits per pixel is, geïndexeerd. De kleurentabel bevat daarom 256 kleuren.

### Gdi {#Gdi}
```
public static final int Gdi
```


De pixelgegevens bevatten GDI-kleuren.

### Indexed {#Indexed}
```
public static final int Indexed
```


De pixelgegevens bevatten kleurgeïndexeerde waarden, wat betekent dat de waarden een index naar kleuren in de systeemtabel zijn, in plaats van individuele kleurwaarden.

### Max {#Max}
```
public static final int Max
```


De maximale waarde voor deze enumeratie.

### PAlpha {#PAlpha}
```
public static final int PAlpha
```


De pixelindeling bevat voorvermenigvuldigde alfa-waarden.

### Undefined {#Undefined}
```
public static final int Undefined
```


De pixelindeling is niet gedefinieerd.

