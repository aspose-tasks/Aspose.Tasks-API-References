---
title: "IPageSavingCallback"
second_title: "Aspose.Tasks for Java API Reference"
description: "다중 페이지 문서의 각 페이지가 별도의 스트림에 저장될 때 호출되는 콜백을 나타냅니다."
type: docs
weight: 382
url: /ko/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

다중 페이지 문서의 각 페이지가 별도의 스트림에 저장될 때 호출되는 콜백을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [onFinish()](#onFinish--) | 모든 페이지가 기록될 때 호출되는 메서드입니다. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | 페이지가 스트림에 저장될 때 호출되는 메서드입니다. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


모든 페이지가 기록될 때 호출되는 메서드입니다.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


페이지가 스트림에 저장될 때 호출되는 메서드입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | 페이지 저장 인수. |

