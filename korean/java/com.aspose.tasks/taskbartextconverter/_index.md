---
title: "TaskBarTextConverter"
second_title: "Aspose.Tasks for Java API Reference"
description: "작업 데이터를 막대 텍스트로 변환하는 사용자 지정 변환기입니다."
type: docs
weight: 290
url: /ko/java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

작업 데이터의 막대 텍스트 변환을 위한 사용자 지정 변환기입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | 작업 데이터의 막대 텍스트 변환을 위한 사용자 지정 변환기입니다. |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


작업 데이터의 막대 텍스트 변환을 위한 사용자 지정 변환기입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 작업 표시줄 텍스트가 렌더링될 작업입니다. |

**Returns:**
java.lang.String - 지정된 작업에 해당하는 막대를 렌더링할 텍스트입니다.
