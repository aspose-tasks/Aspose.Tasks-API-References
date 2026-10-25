---
title: "Aspose::Tasks::Task::GetTimephasedData 메서드"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "C++용 Aspose.Tasks"
description: "주어진 시작 및 종료 날짜 범위 내의 TimephasedData 값을 포함하는 TimephasedDataCollection 객체를 반환합니다."
type: docs
weight: 1360
url: /ko/cpp/aspose.tasks/task/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

주어진 시작 및 종료 날짜 범위 내의 TimephasedData 값을 포함하는 TimephasedDataCollection 객체를 반환합니다.

**Returns:** List of Aspose::Tasks::TimephasedData to be filled in.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| 매개변수 | 설명 |
| --- | --- |
| 시작 | 시간 단계 데이터의 시작 날짜. |
| end | 시간 단계 데이터의 종료 날짜입니다. |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

지정된 시간 구간 데이터 유형의 시작 및 종료 날짜 내에 있는 TimephasedData 값을 포함하는 TimephasedDataCollection 객체를 반환합니다.

**Returns:** A TimephasedDataCollection object with TimephasedData values within given start and end dates of specified timephased data type.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| 매개변수 | 설명 |
| --- | --- |
| 시작 | 시간 단계 데이터의 시작 날짜. |
| end | 시간 단계 데이터의 종료 날짜입니다. |
| timephasedType | 시간 단계 데이터의 유형 ( Aspose::Tasks::TimephasedDataType ). |

