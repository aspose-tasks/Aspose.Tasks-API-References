---
title: "Aspose::Tasks::ResourceAssignment::MakeTPs 메서드"
linktitle: "MakeTPs"
articleTitle: "MakeTPs"
second_title: "C++용 Aspose.Tasks"
description: "시간 구분 데이터 목록을 생성합니다."
type: docs
weight: 740
url: /ko/cpp/aspose.tasks/resourceassignment/maketps/
---

## MakeTPs {#maketps}

시간 구분 데이터 목록을 생성합니다.

**Returns:** A maximum date from list or start date if list is empty.

```cpp
MakeTPs(System::DateTime start, System::TimeSpan time, const System::SharedPtr< Calendar > & calendar, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Aspose::Tasks::TimephasedData >>> & list, bool isWorking, int32_t type)
```

| 매개변수 | 설명 |
| --- | --- |
| 시작 | 지정된 시작 날짜. |
| 시간 | 지정된 작업 시간. |
| 캘린더 | 지정된 작업 캘린더. |
| 목록 | 시간 단계 데이터 목록. |
| isWorking | 시간 단계 데이터가 작업 중인지 여부를 지정하는 플래그. |
| type | 지정된 시간 단계 데이터 유형. |

