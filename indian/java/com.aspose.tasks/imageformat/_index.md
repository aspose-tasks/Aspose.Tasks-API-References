---
title: "ImageFormat"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "छवि के फ़ाइल स्वरूप को निर्दिष्ट करता है।"
type: docs
weight: 133
url: /hi/java/com.aspose.tasks/imageformat/
---

**Inheritance:**
java.lang.Object
```
public final class ImageFormat
```

छवि की फ़ाइल फ़ॉर्मेट को निर्दिष्ट करता है। विस्तारित नहीं किया जा सकता।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ImageFormat(String guid)](#ImageFormat-java.lang.String-) | निर्दिष्ट Guid स्ट्रिंग का उपयोग करके ImageFormat क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [equals(Object o)](#equals-java.lang.Object-) | एक मान लौटाता है जो यह दर्शाता है कि निर्दिष्ट ऑब्जेक्ट एक ImageFormat ऑब्जेक्ट है जो इस ImageFormat ऑब्जेक्ट के बराबर है या नहीं। |
| [getBmp()](#getBmp--) | बिटमैप (BMP) इमेज फ़ॉर्मेट प्राप्त करता है। |
| [getEmf()](#getEmf--) | एन्हांस्ड मेटाफाइल (EMF) इमेज फ़ॉर्मेट प्राप्त करता है। |
| [getExif()](#getExif--) | एक्सचेंजेबल इमेज फ़ाइल (Exif) फ़ॉर्मेट प्राप्त करता है। |
| [getGif()](#getGif--) | ग्राफ़िक्स इंटरचेंज फ़ॉर्मेट (GIF) इमेज फ़ॉर्मेट प्राप्त करता है। |
| [getGuid()](#getGuid--) | एक Guid स्ट्रिंग प्राप्त करता है जो इस ImageFormat ऑब्जेक्ट का प्रतिनिधित्व करती है। |
| [getIcon()](#getIcon--) | विंडोज़ आइकन इमेज फ़ॉर्मेट प्राप्त करता है। |
| [getJpeg()](#getJpeg--) | जॉइंट फ़ोटोग्राफ़िक एक्सपर्ट्स ग्रुप (JPEG) इमेज फ़ॉर्मेट प्राप्त करता है। |
| [getMemoryBmp()](#getMemoryBmp--) | मेमोरी में बिटमैप का फ़ॉर्मेट प्राप्त करता है। |
| [getPng()](#getPng--) | W3C पोर्टेबल नेटवर्क ग्राफ़िक्स (PNG) इमेज फ़ॉर्मेट प्राप्त करता है। |
| [getTiff()](#getTiff--) | टैग्ड इमेज फ़ाइल फ़ॉर्मेट (TIFF) इमेज फ़ॉर्मेट प्राप्त करता है। |
| [getWmf()](#getWmf--) | विंडोज़ मेटाफाइल (WMF) इमेज फ़ॉर्मेट प्राप्त करता है। |
| [hashCode()](#hashCode--) | एक हैश कोड मान लौटाता है जो इस ऑब्जेक्ट का प्रतिनिधित्व करता है। |
| [isBitmapType()](#isBitmapType--) | निर्धारित करता है कि इमेज फ़ॉर्मेट बिटमैप प्रकार है या नहीं। |
| [isMetafileType()](#isMetafileType--) | निर्धारित करता है कि इमेज फ़ॉर्मेट मेटाफाइल प्रकार है या नहीं। |
| [isUnknownType()](#isUnknownType--) | निर्धारित करता है कि इमेज फ़ॉर्मेट अज्ञात प्रकार है या नहीं। |
| [toString()](#toString--) | इस ImageFormat ऑब्जेक्ट को मानव-पठनीय स्ट्रिंग में परिवर्तित करता है। |
### ImageFormat(String guid) {#ImageFormat-java.lang.String-}
```
public ImageFormat(String guid)
```


निर्दिष्ट Guid स्ट्रिंग का उपयोग करके ImageFormat क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| guid | java.lang.String | Guid स्ट्रिंग जो किसी विशेष इमेज फ़ॉर्मेट को निर्दिष्ट करती है। |

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


एक मान लौटाता है जो यह दर्शाता है कि निर्दिष्ट ऑब्जेक्ट एक ImageFormat ऑब्जेक्ट है जो इस ImageFormat ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| o | java.lang.Object | परीक्षण के लिए ऑब्जेक्ट। |

**Returns:**
boolean - true यदि o एक ImageFormat ऑब्जेक्ट है जो इस ImageFormat ऑब्जेक्ट के बराबर है; अन्यथा, false.
### getBmp() {#getBmp--}
```
public static ImageFormat getBmp()
```


बिटमैप (BMP) इमेज फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the bitmap image format.
### getEmf() {#getEmf--}
```
public static ImageFormat getEmf()
```


एन्हांस्ड मेटाफाइल (EMF) इमेज फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the enhanced metafile image format.
### getExif() {#getExif--}
```
public static ImageFormat getExif()
```


एक्सचेंजेबल इमेज फ़ाइल (Exif) फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Exif format.
### getGif() {#getGif--}
```
public static ImageFormat getGif()
```


ग्राफ़िक्स इंटरचेंज फ़ॉर्मेट (GIF) इमेज फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the GIF image format.
### getGuid() {#getGuid--}
```
public String getGuid()
```


एक Guid स्ट्रिंग प्राप्त करता है जो इस ImageFormat ऑब्जेक्ट का प्रतिनिधित्व करती है।

**Returns:**
java.lang.String - यह Guid स्ट्रिंग इस ImageFormat ऑब्जेक्ट का प्रतिनिधित्व करती है.
### getIcon() {#getIcon--}
```
public static ImageFormat getIcon()
```


विंडोज़ आइकन इमेज फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows icon image format.
### getJpeg() {#getJpeg--}
```
public static ImageFormat getJpeg()
```


जॉइंट फ़ोटोग्राफ़िक एक्सपर्ट्स ग्रुप (JPEG) इमेज फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the JPEG image format.
### getMemoryBmp() {#getMemoryBmp--}
```
public static ImageFormat getMemoryBmp()
```


मेमोरी में बिटमैप का फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the format of a bitmap in memory.
### getPng() {#getPng--}
```
public static ImageFormat getPng()
```


W3C पोर्टेबल नेटवर्क ग्राफ़िक्स (PNG) इमेज फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the PNG image format.
### getTiff() {#getTiff--}
```
public static ImageFormat getTiff()
```


टैग्ड इमेज फ़ाइल फ़ॉर्मेट (TIFF) इमेज फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the TIFF image format.
### getWmf() {#getWmf--}
```
public static ImageFormat getWmf()
```


विंडोज़ मेटाफाइल (WMF) इमेज फ़ॉर्मेट प्राप्त करता है।

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows metafile image format.
### hashCode() {#hashCode--}
```
public int hashCode()
```


एक हैश कोड मान लौटाता है जो इस ऑब्जेक्ट का प्रतिनिधित्व करता है।

**Returns:**
int - यह हैश कोड इस ऑब्जेक्ट का प्रतिनिधित्व करता है.
### isBitmapType() {#isBitmapType--}
```
public boolean isBitmapType()
```


निर्धारित करता है कि इमेज फ़ॉर्मेट बिटमैप प्रकार है या नहीं।

**Returns:**
boolean - true यदि एक image format bitmap प्रकार है; अन्यथा, false.
### isMetafileType() {#isMetafileType--}
```
public boolean isMetafileType()
```


निर्धारित करता है कि इमेज फ़ॉर्मेट मेटाफाइल प्रकार है या नहीं।

**Returns:**
boolean - true यदि एक image format metafile प्रकार है; अन्यथा, false.
### isUnknownType() {#isUnknownType--}
```
public boolean isUnknownType()
```


निर्धारित करता है कि इमेज फ़ॉर्मेट अज्ञात प्रकार है या नहीं।

**Returns:**
boolean - true यदि एक image format अज्ञात प्रकार है; अन्यथा, false.
### toString() {#toString--}
```
public String toString()
```


इस ImageFormat ऑब्जेक्ट को मानव-पठनीय स्ट्रिंग में परिवर्तित करता है।

**Returns:**
java.lang.String - यह स्ट्रिंग इस ImageFormat ऑब्जेक्ट का प्रतिनिधित्व करती है.
