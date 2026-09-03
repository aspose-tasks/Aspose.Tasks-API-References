---
title: "Aspose::Tasks::Project::GetPageCount 메서드"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "C++용 Aspose.Tasks"
description: "기본 Timescale(일)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다."
type: docs
weight: 1090
url: /ko/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

기본 Timescale(일)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

주어진 SaveOptions 를 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| 매개변수 | 설명 |
| --- | --- |
| saveOptions | 페이지 수를 가져오기 위한 저장 옵션입니다. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

주어진 Timescale 및 PageSize를 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| 매개변수 | 설명 |
| --- | --- |
| pageSize | 페이지 수를 가져올 크기입니다. |
| scale | 페이지 수를 가져올 스케일입니다. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

주어진 Timescale, PresentationFormat 및 날짜 범위를 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| 매개변수 | 설명 |
| --- | --- |
| pageSize | 페이지 수를 가져올 크기입니다. |
| scale | 페이지 수를 가져올 스케일입니다. |
| startDate | 페이지 수를 가져올 시작 날짜입니다. |
| endDate | 페이지 수를 가져올 종료 날짜입니다. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

기본 Timescale(일)과 주어진 PresentationFormat을 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| 매개변수 | 설명 |
| --- | --- |
| 형식 | 페이지 수를 가져올 형식입니다. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

주어진 Timescale 및 PresentationFormat을 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| 매개변수 | 설명 |
| --- | --- |
| 형식 | 페이지 수를 가져올 형식입니다. |
| scale | 페이지 수를 가져올 스케일입니다. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

주어진 Timescale을 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| 매개변수 | 설명 |
| --- | --- |
| scale | 페이지 수를 가져올 스케일입니다. |

