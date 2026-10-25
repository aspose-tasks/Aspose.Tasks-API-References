---
title: "FontResolveEventArgs"
second_title: "Aspose.Tasks for Java API Reference"
description: "글꼴이 해결될 때 호출되는 콜백에 대한 인수를 제공합니다."
type: docs
weight: 99
url: /ko/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

글꼴이 해결될 때 호출되는 콜백에 대한 인수를 제공합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | 요청된 폰트의 이름을 가져옵니다. |
| [getResolvedFontName()](#getResolvedFontName--) | 해결된 글꼴의 이름을 가져옵니다. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | 해결된 글꼴의 이름을 설정합니다. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


요청된 폰트의 이름을 가져옵니다.

**Returns:**
java.lang.String - 요청된 글꼴의 이름입니다.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


해결된 글꼴의 이름을 가져옵니다. 보기 렌더링에 사용되는 글꼴을 제어하도록 설정할 수 있습니다.

**Returns:**
java.lang.String - 글꼴이 발견되면 요청된 글꼴의 이름, 대체 글꼴의 이름, 또는 글꼴을 찾을 수 없을 경우 null입니다.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


해결된 글꼴의 이름을 설정합니다. 보기 렌더링에 사용되는 글꼴을 제어하도록 설정할 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 해결된 글꼴의 이름. |

