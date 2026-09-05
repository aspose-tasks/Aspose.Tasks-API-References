---
title: "PageInfo"
second_title: "Aspose.Tasks for Java API Reference"
description: "인쇄에 사용되는 MPP 파일 형식에 존재하는 페이지 설정 데이터를 나타냅니다."
type: docs
weight: 176
url: /ko/java/com.aspose.tasks/pageinfo/
---

**Inheritance:**
java.lang.Object
```
public class PageInfo
```

인쇄에 사용되는 MPP 파일 형식에 존재하는 페이지 설정 데이터를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PageInfo()](#PageInfo--) | 새로운 [PageInfo](../../com.aspose.tasks/pageinfo) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getFooter()](#getFooter--) | 푸터 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스를 가져옵니다. |
| [getHeader()](#getHeader--) | 헤더 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스를 가져옵니다. |
| [getLegend()](#getLegend--) | 페이지 전설의 렌더링 옵션을 지정하는 [PageLegend](../../com.aspose/tasks/pagelegend) 클래스의 인스턴스를 가져옵니다. |
| [getMargins()](#getMargins--) | 페이지 여백을 지정하는 [PageMargins](../../com.aspose/tasks/pagemargins) 클래스의 인스턴스를 가져옵니다. |
| [getName()](#getName--) | 설정 데이터가 사용되는 뷰의 이름을 가져옵니다. |
| [getPageSettings()](#getPageSettings--) | `PageSettings`([getPageSettings()](../../com.aspose/tasks/pageinfo\#getPageSettings--)) 클래스의 인스턴스를 가져옵니다. 페이지 인쇄 설정을 지정합니다. |
| [getPageViewSettings()](#getPageViewSettings--) | `PageViewSettings`([getPageViewSettings()](../../com.aspose/tasks/pageinfo\#getPageViewSettings--)) 클래스의 인스턴스를 가져옵니다. 페이지 뷰 인쇄 설정을 지정합니다. |
| [setFooter(HeaderFooterInfo value)](#setFooter-com.aspose.tasks.HeaderFooterInfo-) | 푸터 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스를 설정합니다. |
| [setHeader(HeaderFooterInfo value)](#setHeader-com.aspose.tasks.HeaderFooterInfo-) | 헤더 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스를 설정합니다. |
| [setLegend(PageLegend value)](#setLegend-com.aspose.tasks.PageLegend-) | 페이지 전설의 렌더링 옵션을 지정하는 [PageLegend](../../com.aspose/tasks/pagelegend) 클래스의 인스턴스를 설정합니다. |
### PageInfo() {#PageInfo--}
```
public PageInfo()
```


[PageInfo](../../com.aspose/tasks/pageinfo) 클래스의 새 인스턴스를 초기화합니다. MPP 파일 형식에 존재하고 인쇄에 사용되는 페이지 설정 데이터를 나타냅니다.

### getFooter() {#getFooter--}
```
public final HeaderFooterInfo getFooter()
```


푸터 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) - an instance of the [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) class which represents a footer data.
### getHeader() {#getHeader--}
```
public final HeaderFooterInfo getHeader()
```


헤더 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) - the instance of the [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) class which represents a header data.
### getLegend() {#getLegend--}
```
public final PageLegend getLegend()
```


페이지 전설의 렌더링 옵션을 지정하는 [PageLegend](../../com.aspose/tasks/pagelegend) 클래스의 인스턴스를 가져옵니다.

--------------------

현재는 간트 차트 뷰에만 적용됩니다.

**Returns:**
[PageLegend](../../com.aspose.tasks/pagelegend) - an instance of the [PageLegend](../../com.aspose.tasks/pagelegend) class which specifies rendering options of page legend.
### getMargins() {#getMargins--}
```
public final PageMargins getMargins()
```


페이지 여백을 지정하는 [PageMargins](../../com.aspose/tasks/pagemargins) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[PageMargins](../../com.aspose.tasks/pagemargins) - an instance of the [PageMargins](../../com.aspose.tasks/pagemargins) class which specifies page margins.
### getName() {#getName--}
```
public final String getName()
```


설정 데이터가 사용되는 뷰의 이름을 가져옵니다.

**Returns:**
java.lang.String - 설정 데이터가 사용되는 뷰의 이름.
### getPageSettings() {#getPageSettings--}
```
public final PageSettings getPageSettings()
```


`PageSettings`([getPageSettings()](../../com.aspose/tasks/pageinfo\#getPageSettings--)) 클래스의 인스턴스를 가져옵니다. 페이지 인쇄 설정을 지정합니다.

**Returns:**
[PageSettings](../../com.aspose.tasks/pagesettings) - an instance of the `PageSettings`([getPageSettings()](../../com.aspose.tasks/pageinfo\#getPageSettings--)) class which specifies page printing settings.
### getPageViewSettings() {#getPageViewSettings--}
```
public final PageViewSettings getPageViewSettings()
```


`PageViewSettings`([getPageViewSettings()](../../com.aspose/tasks/pageinfo\#getPageViewSettings--)) 클래스의 인스턴스를 가져옵니다. 페이지 뷰 인쇄 설정을 지정합니다.

**Returns:**
[PageViewSettings](../../com.aspose.tasks/pageviewsettings) - an instance of the `PageViewSettings`([getPageViewSettings()](../../com.aspose.tasks/pageinfo\#getPageViewSettings--)) class which specifies page view printing settings.
### setFooter(HeaderFooterInfo value) {#setFooter-com.aspose.tasks.HeaderFooterInfo-}
```
public final void setFooter(HeaderFooterInfo value)
```


푸터 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) | 푸터 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스. |

### setHeader(HeaderFooterInfo value) {#setHeader-com.aspose.tasks.HeaderFooterInfo-}
```
public final void setHeader(HeaderFooterInfo value)
```


헤더 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) | 헤더 데이터를 나타내는 [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) 클래스의 인스턴스. |

### setLegend(PageLegend value) {#setLegend-com.aspose.tasks.PageLegend-}
```
public final void setLegend(PageLegend value)
```


페이지 전설의 렌더링 옵션을 지정하는 [PageLegend](../../com.aspose/tasks/pagelegend) 클래스의 인스턴스를 설정합니다.

--------------------

현재는 간트 차트 뷰에만 적용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [PageLegend](../../com.aspose.tasks/pagelegend) | 페이지 전설의 렌더링 옵션을 지정하는 [PageLegend](../../com.aspose/tasks/pagelegend) 클래스의 인스턴스. |

