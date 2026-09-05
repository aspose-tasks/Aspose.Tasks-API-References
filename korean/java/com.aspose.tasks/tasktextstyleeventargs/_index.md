---
title: "TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for Java API Reference"
description: "이 클래스는 테이블 셀 내용 렌더링과 관련된 데이터 집합을 나타냅니다."
type: docs
weight: 302
url: /ko/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

이 클래스는 테이블 셀 내용 렌더링과 관련된 데이터 집합을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | 셀 내용 그리기에 사용될 TextStyle을 가져옵니다. |
| [getColumn()](#getColumn--) | 현재 렌더링된 셀이 속한 [ViewColumn](../../com.aspose.tasks/viewcolumn)을 가져옵니다. |
| [getTask()](#getTask--) | 현재 렌더링된 행에 해당하는 `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-))를 가져옵니다. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | 셀 내용 그리기에 사용될 TextStyle을 설정합니다. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


셀 내용 그리기에 사용될 TextStyle을 가져옵니다. 이 객체는 테이블 셀의 외관을 사용자 정의하는 데 사용할 수 있습니다.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


현재 렌더링된 셀이 속한 [ViewColumn](../../com.aspose.tasks/viewcolumn)을 가져옵니다.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


현재 렌더링된 행에 해당하는 `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-))를 가져옵니다.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


셀 내용 그리기에 사용될 TextStyle을 설정합니다. 이 객체는 테이블 셀의 외관을 사용자 정의하는 데 사용할 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | 셀 내용 그리기에 사용될 TextStyle. |

