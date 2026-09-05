---
title: "FontSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 뷰를 렌더링할 때 사용되는 글꼴 설정을 지정합니다."
type: docs
weight: 101
url: /ko/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

프로젝트 뷰를 렌더링할 때 사용되는 글꼴 설정을 지정합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | 렌더링에 사용되는 기본(또는 대체) 글꼴을 가져옵니다. |
| [getFontResolveCallback()](#getFontResolveCallback--) | 해결된 글꼴을 사용자 지정하는 데 사용할 수 있는 콜백을 가져옵니다. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | 렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값을 가져옵니다. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | 렌더링에 사용할 기본(또는 대체) 글꼴을 설정합니다. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | 프로젝트 뷰를 렌더링할 때 Aspose.Tasks가 TrueType 글꼴을 찾는 폴더를 설정합니다. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | 해결된 글꼴을 사용자 지정하는 데 사용할 수 있는 콜백을 설정합니다. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | 렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값을 설정합니다. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


렌더링에 사용되는 기본(또는 대체) 글꼴을 가져옵니다.

**Returns:**
java.lang.String - 렌더링에 사용되는 기본(또는 대체) 글꼴.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


해결된 글꼴을 사용자 지정하는 데 사용할 수 있는 콜백을 가져옵니다.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값을 가져옵니다.

--------------------

값이 False이고 DefaultFontName이 지정된 경우, 렌더링 엔진은 DefaultFontName으로 지정된 글꼴을 대체 글꼴로 사용합니다. 그렇지 않으면 설치된 경우 'Arial' 또는 'Generic Sans Serif' 글꼴이 대체 글꼴로 사용됩니다. 대체 글꼴은 현재 운영 체제에 설치되지 않은 글꼴을 텍스트 스타일이 참조할 때 프로젝트 뷰를 렌더링하는 동안 사용됩니다. 글꼴 해석을 보다 세밀하게 제어하려면 `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) 콜백을 사용할 수 있습니다.

**Returns:**
boolean - 렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


렌더링에 사용할 기본(또는 대체) 글꼴을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 렌더링에 사용되는 기본(또는 대체) 글꼴. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


프로젝트 뷰를 렌더링할 때 Aspose.Tasks가 TrueType 글꼴을 찾는 폴더를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fontFolders | java.lang.String[] | TrueType 글꼴을 포함하는 폴더 배열. |
| recursive | boolean | true인 경우 지정된 폴더를 재귀적으로 스캔합니다. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


해결된 글꼴을 사용자 지정하는 데 사용할 수 있는 콜백을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | 해결된 글꼴을 사용자 지정하는 데 사용할 수 있는 콜백. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값을 설정합니다.

--------------------

값이 False이고 DefaultFontName이 지정된 경우, 렌더링 엔진은 DefaultFontName으로 지정된 글꼴을 대체 글꼴로 사용합니다. 그렇지 않으면 설치된 경우 'Arial' 또는 'Generic Sans Serif' 글꼴이 대체 글꼴로 사용됩니다. 대체 글꼴은 현재 운영 체제에 설치되지 않은 글꼴을 텍스트 스타일이 참조할 때 프로젝트 뷰를 렌더링하는 동안 사용됩니다. 글꼴 해석을 보다 세밀하게 제어하려면 `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) 콜백을 사용할 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값입니다. |

