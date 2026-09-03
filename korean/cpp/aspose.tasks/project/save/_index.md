---
title: "Aspose::Tasks::Project::Save 메서드"
linktitle: "Save"
articleTitle: "Save"
second_title: "C++용 Aspose.Tasks"
description: "지정된 저장 옵션을 사용하여 프로젝트를 스트림에 저장합니다."
type: docs
weight: 1190
url: /ko/cpp/aspose.tasks/project/save/
---

## Save (1 of 5) {#save_1}

지정된 저장 옵션을 사용하여 프로젝트를 스트림에 저장합니다.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| 매개변수 | 설명 |
| --- | --- |
| stream | 스트림. |
| options | 저장 옵션. |

---

## Save (2 of 5) {#save_2}

프로젝트 데이터를 스트림에 저장합니다.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, Saving::SaveFileFormat format)
```

| 매개변수 | 설명 |
| --- | --- |
| stream | 스트림. |
| 형식 | 지정된 저장 파일 형식. SaveFileFormat |

---

## Save (3 of 5) {#save_3}

프로젝트 데이터를 mpp 형식 파일에 저장합니다.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename)
```

| 매개변수 | 설명 |
| --- | --- |
| 파일 이름 | 파일 이름. |

---

## Save (4 of 5) {#save_4}

지정된 저장 옵션을 사용하여 문서를 파일에 저장합니다.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| 매개변수 | 설명 |
| --- | --- |
| 파일 이름 | 파일 이름. |
| options | 저장 옵션. |

---

## Save (5 of 5) {#save_5}

프로젝트 데이터를 파일에 저장합니다.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, Saving::SaveFileFormat format)
```

| 매개변수 | 설명 |
| --- | --- |
| 파일 이름 | 파일 이름. |
| 형식 | 저장 파일 형식. |

