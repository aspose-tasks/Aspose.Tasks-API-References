---
title: "ImageFormat"
second_title: "Aspose.Tasks for Java API Reference"
description: "이미지의 파일 형식을 지정합니다."
type: docs
weight: 133
url: /ko/java/com.aspose.tasks/imageformat/
---

**Inheritance:**
java.lang.Object
```
public final class ImageFormat
```

이미지의 파일 형식을 지정합니다. 확장할 수 없습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ImageFormat(String guid)](#ImageFormat-java.lang.String-) | 지정된 Guid 문자열을 사용하여 ImageFormat 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [equals(Object o)](#equals-java.lang.Object-) | 지정된 객체가 이 ImageFormat 객체와 동등한 ImageFormat 객체인지 여부를 나타내는 값을 반환합니다. |
| [getBmp()](#getBmp--) | 비트맵(BMP) 이미지 형식을 가져옵니다. |
| [getEmf()](#getEmf--) | 향상된 메타파일(EMF) 이미지 형식을 가져옵니다. |
| [getExif()](#getExif--) | 교환 이미지 파일(Exif) 형식을 가져옵니다. |
| [getGif()](#getGif--) | 그래픽 교환 형식(GIF) 이미지 형식을 가져옵니다. |
| [getGuid()](#getGuid--) | 이 ImageFormat 객체를 나타내는 Guid 문자열을 가져옵니다. |
| [getIcon()](#getIcon--) | Windows 아이콘 이미지 형식을 가져옵니다. |
| [getJpeg()](#getJpeg--) | Joint Photographic Experts Group(JPEG) 이미지 형식을 가져옵니다. |
| [getMemoryBmp()](#getMemoryBmp--) | 메모리 내 비트맵의 형식을 가져옵니다. |
| [getPng()](#getPng--) | W3C 포터블 네트워크 그래픽스(PNG) 이미지 형식을 가져옵니다. |
| [getTiff()](#getTiff--) | 태그 이미지 파일 형식(TIFF) 이미지 형식을 가져옵니다. |
| [getWmf()](#getWmf--) | Windows 메타파일(WMF) 이미지 형식을 가져옵니다. |
| [hashCode()](#hashCode--) | 이 객체를 나타내는 해시 코드 값을 반환합니다. |
| [isBitmapType()](#isBitmapType--) | 이미지 형식이 비트맵 유형인지 여부를 결정합니다. |
| [isMetafileType()](#isMetafileType--) | 이미지 형식이 메타파일 유형인지 여부를 결정합니다. |
| [isUnknownType()](#isUnknownType--) | 이미지 형식이 알 수 없는 유형인지 여부를 결정합니다. |
| [toString()](#toString--) | 이 ImageFormat 객체를 사람이 읽을 수 있는 문자열로 변환합니다. |
### ImageFormat(String guid) {#ImageFormat-java.lang.String-}
```
public ImageFormat(String guid)
```


지정된 Guid 문자열을 사용하여 ImageFormat 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| guid | java.lang.String | 특정 이미지 형식을 지정하는 Guid 문자열입니다. |

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


지정된 객체가 이 ImageFormat 객체와 동등한 ImageFormat 객체인지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| o | java.lang.Object | 테스트할 객체입니다. |

**Returns:**
boolean - o가 이 ImageFormat 객체와 동등한 ImageFormat 객체인 경우 true; 그렇지 않으면 false.
### getBmp() {#getBmp--}
```
public static ImageFormat getBmp()
```


비트맵(BMP) 이미지 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the bitmap image format.
### getEmf() {#getEmf--}
```
public static ImageFormat getEmf()
```


향상된 메타파일(EMF) 이미지 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the enhanced metafile image format.
### getExif() {#getExif--}
```
public static ImageFormat getExif()
```


교환 이미지 파일(Exif) 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Exif format.
### getGif() {#getGif--}
```
public static ImageFormat getGif()
```


그래픽 교환 형식(GIF) 이미지 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the GIF image format.
### getGuid() {#getGuid--}
```
public String getGuid()
```


이 ImageFormat 객체를 나타내는 Guid 문자열을 가져옵니다.

**Returns:**
java.lang.String - 이 ImageFormat 객체를 나타내는 Guid 문자열.
### getIcon() {#getIcon--}
```
public static ImageFormat getIcon()
```


Windows 아이콘 이미지 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows icon image format.
### getJpeg() {#getJpeg--}
```
public static ImageFormat getJpeg()
```


Joint Photographic Experts Group(JPEG) 이미지 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the JPEG image format.
### getMemoryBmp() {#getMemoryBmp--}
```
public static ImageFormat getMemoryBmp()
```


메모리 내 비트맵의 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the format of a bitmap in memory.
### getPng() {#getPng--}
```
public static ImageFormat getPng()
```


W3C 포터블 네트워크 그래픽스(PNG) 이미지 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the PNG image format.
### getTiff() {#getTiff--}
```
public static ImageFormat getTiff()
```


태그 이미지 파일 형식(TIFF) 이미지 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the TIFF image format.
### getWmf() {#getWmf--}
```
public static ImageFormat getWmf()
```


Windows 메타파일(WMF) 이미지 형식을 가져옵니다.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows metafile image format.
### hashCode() {#hashCode--}
```
public int hashCode()
```


이 객체를 나타내는 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체를 나타내는 해시 코드.
### isBitmapType() {#isBitmapType--}
```
public boolean isBitmapType()
```


이미지 형식이 비트맵 유형인지 여부를 결정합니다.

**Returns:**
boolean - 이미지 형식이 비트맵 유형인 경우 true; 그렇지 않으면 false.
### isMetafileType() {#isMetafileType--}
```
public boolean isMetafileType()
```


이미지 형식이 메타파일 유형인지 여부를 결정합니다.

**Returns:**
boolean - 이미지 형식이 메타파일 유형인 경우 true; 그렇지 않으면 false.
### isUnknownType() {#isUnknownType--}
```
public boolean isUnknownType()
```


이미지 형식이 알 수 없는 유형인지 여부를 결정합니다.

**Returns:**
boolean - 이미지 형식이 알 수 없는 유형인 경우 true; 그렇지 않으면 false.
### toString() {#toString--}
```
public String toString()
```


이 ImageFormat 객체를 사람이 읽을 수 있는 문자열로 변환합니다.

**Returns:**
java.lang.String - 이 ImageFormat 객체를 나타내는 문자열.
