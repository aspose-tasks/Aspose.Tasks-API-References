---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 페이지를 이미지로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 134
url: /ko/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

프로젝트 페이지를 이미지로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | 렌더링된 이미지를 TIFF, PNG, BMP 또는 JPEG 형식으로 저장하는 데 사용할 수 있는 [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | 프로젝트 뷰를 렌더링할 때 사용되는 글꼴 설정을 지정합니다. |
| [getHorizontalResolution()](#getHorizontalResolution--) | dpi 단위의 수평 해상도를 가져옵니다. |
| [getJpegQuality()](#getJpegQuality--) | JPEG 품질을 가져옵니다. |
| [getPageSavingCallback()](#getPageSavingCallback--) | 각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백을 가져옵니다. |
| [getPages()](#getPages--) | 프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 가져옵니다. |
| [getPixelFormat()](#getPixelFormat--) | 이미지의 각 픽셀에 대한 색상 데이터 형식을 가져옵니다. |
| [getReduceFooterGap()](#getReduceFooterGap--) | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 가져옵니다. |
| [getTiffCompression()](#getTiffCompression--) | 생성된 이미지를 TIFF 형식으로 저장할 때 적용할 압축 유형을 가져옵니다. |
| [getVerticalResolution()](#getVerticalResolution--) | dpi 단위의 세로 해상도를 가져옵니다. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | dpi 단위의 가로 해상도를 설정합니다. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | JPEG 품질을 설정합니다. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백을 설정합니다. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | 프로젝트 레이아웃을 별도의 파일로 저장할 때 저장할 페이지 번호 목록을 설정합니다. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | 이미지의 각 픽셀에 대한 색상 데이터 형식을 설정합니다. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 설정합니다. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | 생성된 이미지를 TIFF 형식으로 저장할 때 적용할 압축 유형을 설정합니다. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | dpi 단위의 세로 해상도를 설정합니다. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


렌더링된 이미지를 TIFF, PNG, BMP 또는 JPEG 형식으로 저장하는 데 사용할 수 있는 [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| saveFormat | int | TIFF, PNG, BMP 또는 JPEG[SaveFileFormat](../../com.aspose/tasks/savefileformat)일 수 있습니다. |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


내부 사용을 위해 예약됨.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


내부 사용을 위해 예약됨.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


프로젝트 뷰를 렌더링할 때 사용되는 글꼴 설정을 지정합니다.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


dpi 단위의 수평 해상도를 가져옵니다.

**Returns:**
float - dpi 단위의 가로 해상도.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


JPEG 품질을 가져옵니다. 허용값 범위는 0..100입니다.

**Returns:**
int - JPEG 품질.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백을 가져옵니다.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 가져옵니다.

--------------------

이 목록이 비어 있으면 모든 페이지가 저장됩니다.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - 프로젝트 레이아웃을 별도의 파일로 저장할 때 저장할 페이지 번호 목록.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


이미지의 각 픽셀에 대한 색상 데이터 형식을 가져옵니다.

**Returns:**
int - 이미지의 각 픽셀에 대한 색상 데이터 형식.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


생성된 이미지를 TIFF 형식으로 저장할 때 적용할 압축 유형을 가져옵니다.

--------------------

TIFF로 저장할 때만 효과가 있습니다. 기본값은 `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-))입니다.

**Returns:**
int - TIFF 형식으로 생성된 이미지를 저장할 때 적용할 압축 유형.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


dpi 단위의 세로 해상도를 가져옵니다.

**Returns:**
float - dpi 단위의 세로 해상도.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


dpi 단위의 가로 해상도를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | float | dpi 단위의 가로 해상도. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


JPEG 품질을 설정합니다. 허용값 범위는 0..100입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | JPEG 품질. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | 각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


프로젝트 레이아웃을 별도의 파일로 저장할 때 저장할 페이지 번호 목록을 설정합니다.

--------------------

이 목록이 비어 있으면 모든 페이지가 저장됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.List&lt;java.lang.Integer&gt; | 프로젝트 레이아웃을 별도의 파일로 저장할 때 저장할 페이지 번호 목록. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


이미지의 각 픽셀에 대한 색상 데이터 형식을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 이미지의 각 픽셀에 대한 색상 데이터 형식. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


생성된 이미지를 TIFF 형식으로 저장할 때 적용할 압축 유형을 설정합니다.

--------------------

TIFF로 저장할 때만 효과가 있습니다. 기본값은 `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-))입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | TIFF 형식으로 생성된 이미지를 저장할 때 적용할 압축 유형. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


dpi 단위의 세로 해상도를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | float | dpi 단위의 세로 해상도. |

