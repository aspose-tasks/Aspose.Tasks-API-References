---
title: "XpsOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 페이지를 XPS로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 369
url: /ko/java/com.aspose.tasks/xpsoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class XpsOptions extends SaveOptions implements ICloneableSaveOptions
```

프로젝트 페이지를 XPS로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [XpsOptions()](#XpsOptions--) | 새로운 [XpsOptions](../../com.aspose.tasks/xpsoptions) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getRenderMetafileAsBitmap()](#getRenderMetafileAsBitmap--) | 메타파일을 비트맵으로 렌더링할지 여부를 나타내는 값을 가져옵니다. |
| [setRenderMetafileAsBitmap(boolean value)](#setRenderMetafileAsBitmap-boolean-) | 메타파일을 비트맵으로 렌더링할지 여부를 나타내는 값을 설정합니다. |
### XpsOptions() {#XpsOptions--}
```
public XpsOptions()
```


새로운 [XpsOptions](../../com.aspose.tasks/xpsoptions) 클래스 인스턴스를 초기화합니다.

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
public final SaveOptions deepClone()
```


내부 사용을 위해 예약됨.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getRenderMetafileAsBitmap() {#getRenderMetafileAsBitmap--}
```
public final boolean getRenderMetafileAsBitmap()
```


메타파일을 비트맵으로 렌더링할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 메타파일을 비트맵으로 렌더링할지 여부를 나타내는 값.
### setRenderMetafileAsBitmap(boolean value) {#setRenderMetafileAsBitmap-boolean-}
```
public final void setRenderMetafileAsBitmap(boolean value)
```


메타파일을 비트맵으로 렌더링할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 메타파일을 비트맵으로 렌더링할지 여부를 나타내는 값. |

