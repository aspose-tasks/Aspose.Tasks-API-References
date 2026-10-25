---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 페이지를 HTML로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 132
url: /ko/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

프로젝트 페이지를 HTML로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | CSS를 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져옵니다. |
| [getCssStylePrefix()](#getCssStylePrefix--) | CSS 스타일 접두사를 가져옵니다. |
| [getExportCss()](#getExportCss--) | CSS가 내보내지는 방식을 가져옵니다. |
| [getExportFonts()](#getExportFonts--) | 글꼴이 내보내지는 방식을 가져옵니다. |
| [getExportImages()](#getExportImages--) | 이미지가 내보내지는 방식을 가져옵니다. |
| [getFontFaceTypes()](#getFontFaceTypes--) | 글꼴 얼굴 유형을 가져옵니다. |
| [getFontSavingCallback()](#getFontSavingCallback--) | 글꼴을 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져옵니다. |
| [getFontSettings()](#getFontSettings--) | 프로젝트 뷰를 렌더링할 때 사용되는 글꼴 설정을 지정합니다. |
| [getImageSavingCallback()](#getImageSavingCallback--) | 글꼴을 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져옵니다. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | HTML 페이지 헤더에 프로젝트 이름을 포함할지 여부를 나타내는 값을 가져옵니다. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | HTML 제목에 프로젝트 이름을 포함할지 여부를 나타내는 값을 가져옵니다. |
| [getPageSavingCallback()](#getPageSavingCallback--) | 각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백을 가져옵니다. |
| [getPages()](#getPages--) | 프로젝트 레이아웃을 렌더링할 때 저장할 페이지 번호 목록을 가져옵니다. |
| [getReduceFooterGap()](#getReduceFooterGap--) | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 가져옵니다. |
| [getUseGradientBrush()](#getUseGradientBrush--) | 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져옵니다. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | CSS를 저장할 리소스를 생성하기 위해 호출되는 콜백을 설정합니다. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | CSS 스타일 접두사를 설정합니다. |
| [setExportCss(int value)](#setExportCss-int-) | CSS가 내보내지는 방식을 설정합니다. |
| [setExportFonts(int value)](#setExportFonts-int-) | 글꼴이 내보내지는 방식을 설정합니다. |
| [setExportImages(int value)](#setExportImages-int-) | 이미지가 내보내지는 방식을 설정합니다. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | 글꼴 종류를 설정합니다. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | 글꼴을 저장할 리소스를 생성하기 위해 호출되는 콜백을 설정합니다. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | 글꼴을 저장할 리소스를 생성하기 위해 호출되는 콜백을 설정합니다. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | HTML 페이지 헤더에 프로젝트 이름을 포함할지 여부를 나타내는 값을 설정합니다. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | HTML 제목에 프로젝트 이름을 포함할지 여부를 나타내는 값을 설정합니다. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백을 설정합니다. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | 프로젝트 레이아웃을 렌더링할 때 저장할 페이지 번호 목록을 설정합니다. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 설정합니다. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 설정합니다. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


[HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) 클래스의 새 인스턴스를 초기화합니다.

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
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


CSS를 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져옵니다.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


CSS 스타일 접두사를 가져옵니다.

**Returns:**
java.lang.String - CSS 스타일 접두사.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


CSS가 내보내지는 방식을 가져옵니다.

**Returns:**
int - CSS가 내보내지는 방식.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


글꼴이 내보내지는 방식을 가져옵니다.

**Returns:**
int - 글꼴이 내보내지는 방식.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


이미지가 내보내지는 방식을 가져옵니다.

**Returns:**
int - 이미지가 내보내지는 방식.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


글꼴 얼굴 유형을 가져옵니다.

값: 글꼴 종류.

**Returns:**
int - 글꼴 종류.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


글꼴을 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져옵니다.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


프로젝트 뷰를 렌더링할 때 사용되는 글꼴 설정을 지정합니다.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


글꼴을 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져옵니다.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


HTML 페이지 헤더에 프로젝트 이름을 포함할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - HTML 페이지 헤더에 프로젝트 이름을 포함할지 여부를 나타내는 값.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


HTML 제목에 프로젝트 이름을 포함할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - HTML 제목에 프로젝트 이름을 포함할지 여부를 나타내는 값.
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


프로젝트 레이아웃을 렌더링할 때 저장할 페이지 번호 목록을 가져옵니다.

--------------------

이 목록이 비어 있으면 모든 프로젝트 페이지가 저장됩니다.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - 프로젝트 레이아웃을 렌더링할 때 저장할 페이지 번호 목록.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져옵니다.

--------------------

현재 HTML로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다.

**Returns:**
boolean - 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


CSS를 저장할 리소스를 생성하기 위해 호출되는 콜백을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | CSS를 저장할 리소스를 생성하기 위해 호출되는 콜백. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


CSS 스타일 접두사를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | CSS 스타일 접두사. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


CSS가 내보내지는 방식을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | CSS가 내보내지는 방식. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


글꼴이 내보내지는 방식을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 글꼴이 내보내지는 방식. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


이미지가 내보내지는 방식을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 이미지가 내보내지는 방식. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


글꼴 종류를 설정합니다.

값: 글꼴 종류.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 폰트 페이스 유형. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


글꼴을 저장할 리소스를 생성하기 위해 호출되는 콜백을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | 폰트를 저장할 리소스를 생성하기 위해 호출되는 콜백. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


글꼴을 저장할 리소스를 생성하기 위해 호출되는 콜백을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | 폰트를 저장할 리소스를 생성하기 위해 호출되는 콜백. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


HTML 페이지 헤더에 프로젝트 이름을 포함할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | HTML 페이지 헤더에 프로젝트 이름을 포함할지 여부를 나타내는 값. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


HTML 제목에 프로젝트 이름을 포함할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | HTML 제목에 프로젝트 이름을 포함할지 여부를 나타내는 값. |

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


프로젝트 레이아웃을 렌더링할 때 저장할 페이지 번호 목록을 설정합니다.

--------------------

이 목록이 비어 있으면 모든 프로젝트 페이지가 저장됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.List&lt;java.lang.Integer&gt; | 프로젝트 레이아웃을 렌더링할 때 저장할 페이지 번호 목록. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 설정합니다.

--------------------

현재 HTML로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값. |

