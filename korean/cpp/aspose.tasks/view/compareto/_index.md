---
title: "Aspose::Tasks::View::CompareTo 메서드"
linktitle: "CompareTo"
articleTitle: "CompareTo"
second_title: "C++용 Aspose.Tasks"
description: "현재 인스턴스를 동일한 유형의 다른 객체와 비교하고, 현재 인스턴스가 앞서는지, 뒤따르는지, 혹은 ..."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/view/compareto/
---

## CompareTo {#compareto}

현재 인스턴스를 동일 유형의 다른 객체와 비교하고, 현재 인스턴스가 정렬 순서에서 앞선, 뒤에 있거나 같은 위치에 있는지를 나타내는 정수를 반환합니다.

**Returns:** A 32-bit signed integer that indicates the relative order of the objects being compared. The return value has these meanings: Value Meaning Less than zero This instance precedes other in the sort order. Zero This instance occurs in the same position in the sort order as other . Greater than zero This instance follows other in the sort order.

```cpp
CompareTo(System::SharedPtr< View > other)
```

| 매개변수 | 설명 |
| --- | --- |
| 다른 | 지정된 View 객체와 이 인스턴스를 비교합니다. |

