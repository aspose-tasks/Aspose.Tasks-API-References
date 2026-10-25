---
title: "TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for Java API Reference"
description: "간트 차트 뷰에서 작업 링크가 렌더링될 때 호출되는 콜백을 나타냅니다."
type: docs
weight: 298
url: /ko/java/com.aspose.tasks/tasklinkdrawingcallbackdelegate/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskLinkDrawingCallbackDelegate extends System.MulticastDelegate
```

간트 차트 뷰에서 작업 링크가 렌더링될 때 호출되는 콜백을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TaskLinkDrawingCallbackDelegate()](#TaskLinkDrawingCallbackDelegate--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [invoke(TaskLinkDrawingArgs args)](#invoke-com.aspose.tasks.TaskLinkDrawingArgs-) | 작업 링크 그리기 이벤트를 처리하기 위한 메서드 콜백을 나타냅니다. |
### TaskLinkDrawingCallbackDelegate() {#TaskLinkDrawingCallbackDelegate--}
```
public TaskLinkDrawingCallbackDelegate()
```


### invoke(TaskLinkDrawingArgs args) {#invoke-com.aspose.tasks.TaskLinkDrawingArgs-}
```
public abstract void invoke(TaskLinkDrawingArgs args)
```


작업 링크 그리기 이벤트를 처리하기 위한 메서드 콜백을 나타냅니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| args | [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) | 콜백 데이터를 포함하는 [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) 클래스의 인스턴스입니다. |

