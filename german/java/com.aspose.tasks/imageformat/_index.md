---
title: "ImageFormat"
second_title: "Aspose.Tasks for Java API Reference"
description: "Gibt das Dateiformat des Bildes an."
type: docs
weight: 133
url: /de/java/com.aspose.tasks/imageformat/
---

**Inheritance:**
java.lang.Object
```
public final class ImageFormat
```

Gibt das Dateiformat des Bildes an. Kann nicht erweitert werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ImageFormat(String guid)](#ImageFormat-java.lang.String-) | Initialisiert eine neue Instanz der ImageFormat-Klasse mithilfe des angegebenen Guid-Strings. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object o)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob das angegebene Objekt ein ImageFormat-Objekt ist, das diesem ImageFormat-Objekt entspricht. |
| [getBmp()](#getBmp--) | Liefert das Bitmap (BMP)-Bildformat. |
| [getEmf()](#getEmf--) | Liefert das erweiterte Metafile (EMF)-Bildformat. |
| [getExif()](#getExif--) | Liefert das Exchangeable Image File (Exif)-Format. |
| [getGif()](#getGif--) | Liefert das Graphics Interchange Format (GIF)-Bildformat. |
| [getGuid()](#getGuid--) | Liefert einen Guid-String, der dieses ImageFormat-Objekt darstellt. |
| [getIcon()](#getIcon--) | Liefert das Windows-Icon-Bildformat. |
| [getJpeg()](#getJpeg--) | Liefert das Joint Photographic Experts Group (JPEG)-Bildformat. |
| [getMemoryBmp()](#getMemoryBmp--) | Liefert das Format eines Bitmaps im Speicher. |
| [getPng()](#getPng--) | Liefert das W3C Portable Network Graphics (PNG)-Bildformat. |
| [getTiff()](#getTiff--) | Liefert das Tagged Image File Format (TIFF)-Bildformat. |
| [getWmf()](#getWmf--) | Liefert das Windows-Metafile (WMF)-Bildformat. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert zurück, der dieses Objekt darstellt. |
| [isBitmapType()](#isBitmapType--) | Bestimmt, ob ein Bildformat vom Typ Bitmap ist. |
| [isMetafileType()](#isMetafileType--) | Bestimmt, ob ein Bildformat vom Typ Metafile ist. |
| [isUnknownType()](#isUnknownType--) | Bestimmt, ob ein Bildformat vom Typ unbekannt ist. |
| [toString()](#toString--) | Konvertiert dieses ImageFormat-Objekt in eine menschenlesbare Zeichenkette. |
### ImageFormat(String guid) {#ImageFormat-java.lang.String-}
```
public ImageFormat(String guid)
```


Initialisiert eine neue Instanz der ImageFormat-Klasse mithilfe des angegebenen Guid-Strings.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| guid | java.lang.String | Der Guid-String, der ein bestimmtes Bildformat angibt. |

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


Gibt einen Wert zurück, der angibt, ob das angegebene Objekt ein ImageFormat-Objekt ist, das diesem ImageFormat-Objekt entspricht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das zu testende Objekt. |

**Returns:**
boolean - true, wenn o ein ImageFormat-Objekt ist, das diesem ImageFormat-Objekt entspricht; andernfalls false.
### getBmp() {#getBmp--}
```
public static ImageFormat getBmp()
```


Liefert das Bitmap (BMP)-Bildformat.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the bitmap image format.
### getEmf() {#getEmf--}
```
public static ImageFormat getEmf()
```


Liefert das erweiterte Metafile (EMF)-Bildformat.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the enhanced metafile image format.
### getExif() {#getExif--}
```
public static ImageFormat getExif()
```


Liefert das Exchangeable Image File (Exif)-Format.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Exif format.
### getGif() {#getGif--}
```
public static ImageFormat getGif()
```


Liefert das Graphics Interchange Format (GIF)-Bildformat.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the GIF image format.
### getGuid() {#getGuid--}
```
public String getGuid()
```


Liefert einen Guid-String, der dieses ImageFormat-Objekt darstellt.

**Returns:**
java.lang.String - Ein Guid-String, der dieses ImageFormat-Objekt darstellt.
### getIcon() {#getIcon--}
```
public static ImageFormat getIcon()
```


Liefert das Windows-Icon-Bildformat.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows icon image format.
### getJpeg() {#getJpeg--}
```
public static ImageFormat getJpeg()
```


Liefert das Joint Photographic Experts Group (JPEG)-Bildformat.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the JPEG image format.
### getMemoryBmp() {#getMemoryBmp--}
```
public static ImageFormat getMemoryBmp()
```


Liefert das Format eines Bitmaps im Speicher.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the format of a bitmap in memory.
### getPng() {#getPng--}
```
public static ImageFormat getPng()
```


Liefert das W3C Portable Network Graphics (PNG)-Bildformat.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the PNG image format.
### getTiff() {#getTiff--}
```
public static ImageFormat getTiff()
```


Liefert das Tagged Image File Format (TIFF)-Bildformat.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the TIFF image format.
### getWmf() {#getWmf--}
```
public static ImageFormat getWmf()
```


Liefert das Windows-Metafile (WMF)-Bildformat.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows metafile image format.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert zurück, der dieses Objekt darstellt.

**Returns:**
int - Ein Hashcode, der dieses Objekt darstellt.
### isBitmapType() {#isBitmapType--}
```
public boolean isBitmapType()
```


Bestimmt, ob ein Bildformat vom Typ Bitmap ist.

**Returns:**
boolean - true, wenn ein Bildformat ein Bitmap-Typ ist; andernfalls false.
### isMetafileType() {#isMetafileType--}
```
public boolean isMetafileType()
```


Bestimmt, ob ein Bildformat vom Typ Metafile ist.

**Returns:**
boolean - true, wenn ein Bildformat ein Metafile-Typ ist; andernfalls false.
### isUnknownType() {#isUnknownType--}
```
public boolean isUnknownType()
```


Bestimmt, ob ein Bildformat vom Typ unbekannt ist.

**Returns:**
boolean - true, wenn ein Bildformat ein unbekannter Typ ist; andernfalls false.
### toString() {#toString--}
```
public String toString()
```


Konvertiert dieses ImageFormat-Objekt in eine menschenlesbare Zeichenkette.

**Returns:**
java.lang.String - Ein String, der dieses ImageFormat-Objekt darstellt.
