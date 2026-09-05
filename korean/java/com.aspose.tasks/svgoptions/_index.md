---
title: "SvgOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 페이지를 SVG로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 283
url: /ko/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

프로젝트 페이지를 SVG로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | SVG 형식으로 프로젝트를 저장하는 데 사용할 수 있는 [SvgOptions](../../com.aspose/tasks/svgoptions) 클래스를 새 인스턴스로 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | 렌더링된 각 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 구현 콜백을 가져옵니다. |
| [getUseGradientBrush()](#getUseGradientBrush--) | 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 결정합니다. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 렌더링된 각 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 구현 콜백을 설정합니다. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 결정합니다. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


SVG 형식으로 프로젝트를 저장하는 데 사용할 수 있는 [SvgOptions](../../com.aspose/tasks/svgoptions) 클래스를 새 인스턴스로 초기화합니다.

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
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


렌더링된 각 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 구현 콜백을 가져옵니다.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 결정합니다.

--------------------

현재 SVG로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다.

**Returns:**
boolean - 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값입니다.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


렌더링된 각 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 구현 콜백을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | 렌더링된 각 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 구현 콜백입니다. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 결정합니다.

--------------------

현재 SVG로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값입니다. |

