---
title: "Aspose::Tasks::TimephasedDataCollection::SelectBetweenStartAndFinish 메서드"
linktitle: "SelectBetweenStartAndFinish"
articleTitle: "SelectBetweenStartAndFinish"
second_title: "C++용 Aspose.Tasks"
description: "startTime과 finishTime 사이의 모든 시간 단계들을 선택합니다."
type: docs
weight: 120
url: /ko/cpp/aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/
---

## SelectBetweenStartAndFinish {#selectbetweenstartandfinish}

startTime과 finishTime 사이의 모든 시간 단계를 선택합니다. 평균 경우 O(log n) 복잡도를 가집니다.

**Returns:** Returns new list instance of TimephasedDataCollection data ordered by Start property.

```cpp
SelectBetweenStartAndFinish(TimephasedDataType timephasedDataType, System::DateTime startTime, System::DateTime finishTime)
```

| 매개변수 | 설명 |
| --- | --- |
| timephasedDataType | 선택할 시간 단계의 유형입니다. |
| startTime | 구간 시작. |
| finishTime | 구간 종료. |

