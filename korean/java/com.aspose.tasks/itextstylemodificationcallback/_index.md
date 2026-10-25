---
title: "ITextStyleModificationCallback"
second_title: "Aspose.Tasks for Java API Reference"
description: "TextStyle이 테이블 셀에 적용되기 전에 호출되는 콜백을 나타냅니다."
type: docs
weight: 383
url: /ko/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

TextStyle이 테이블 셀에 적용되기 전에 호출되는 콜백을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | 다음 보기('Gantt Chart', 'Task Sheet', 'Task Usage')에서 작업 행의 테이블 셀을 렌더링하기 전에 호출되는 메서드. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


다음 보기('Gantt Chart', 'Task Sheet', 'Task Usage')에서 작업 행의 테이블 셀을 렌더링하기 전에 호출되는 메서드.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | 해당 [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) 객체. |

