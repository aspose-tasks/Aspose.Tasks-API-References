---
title: "Aspose::Tasks::Project::Project 생성자"
linktitle: "프로젝트"
articleTitle: "프로젝트"
second_title: "C++용 Aspose.Tasks"
description: "Project 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Project 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

암호로 보호된 템플릿(기존 mpp 또는 mpt 파일)에서 Project 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| 매개변수 | 설명 |
| --- | --- |
| projectTemplate | 프로젝트를 생성할 템플릿 경로. |
| protectionPassword | 보호 암호. |

---

## Project (3 of 13) {#project_3}

템플릿(기존 mpp 또는 mpt 파일)에서 Project 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| 매개변수 | 설명 |
| --- | --- |
| projectTemplate | 프로젝트를 생성할 템플릿 경로. |

---

## Project (4 of 13) {#project_4}

지정된 PrimaveraReadOptions 클래스 인스턴스를 사용하여 Stream에서 Project 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| 매개변수 | 설명 |
| --- | --- |
| stream | Project System::IO::Stream 클래스의 스트림 |
| options | PrimaveraReadOptions 클래스의 지정된 인스턴스로, Primavera 형식(XER 또는 XML) 읽기를 사용자 정의할 수 있습니다. |

---

## Project (5 of 13) {#project_5}

템플릿(기존 mpp 또는 mpt 파일)에서 Project 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| 매개변수 | 설명 |
| --- | --- |
| projectTemplate | 프로젝트를 생성할 템플릿 경로. |
| parseErrorHandler | XML 구문 분석 오류를 처리하기 위한 지정된 콜백 메서드. |

---

## Project (6 of 13) {#project_6}

스트림에서 Project 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| 매개변수 | 설명 |
| --- | --- |
| stream | 템플릿을 로드할 스트림. |

---

## Project (7 of 13) {#project_7}

StreamReader 인스턴스에서 Project 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| 매개변수 | 설명 |
| --- | --- |
| reader | 템플릿을 로드할 스트림 리더. |

---

## Project (8 of 13) {#project_8}

지정된 PrimaveraReadOptions 클래스 인스턴스를 사용하여 템플릿(기존 MPP 또는 MPT 파일)에서 Project 클래스를 새 인스턴스로 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| 매개변수 | 설명 |
| --- | --- |
| projectTemplate | 프로젝트를 생성할 템플릿 경로 |
| options | 지정된 PrimaveraReadOptions 클래스 인스턴스. |

---

## Project (9 of 13) {#project_9}

DbSettings 클래스 인스턴스로 지정된 데이터베이스에서 데이터를 읽기 위해 Project 클래스를 새 인스턴스로 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| 매개변수 | 설명 |
| --- | --- |
| 설정 | 지정된 DbSettings 클래스 인스턴스. |

---

## Project (10 of 13) {#project_10}

템플릿(기존 mpp 또는 mpt 파일)에서 Project 클래스를 새 인스턴스로 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| 매개변수 | 설명 |
| --- | --- |
| stream | 템플릿을 로드할 스트림. |
| parseErrorHandler | XML 구문 분석 오류를 처리하기 위한 지정된 콜백 메서드. |

---

## Project (11 of 13) {#project_11}

템플릿(기존 mpp 또는 mpt 파일)에서 Project 클래스를 새 인스턴스로 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| 매개변수 | 설명 |
| --- | --- |
| stream | 템플릿을 로드할 스트림. |
| protectionPassword | 보호 암호. |

---

## Project (12 of 13) {#project_12}

지정된 LoadOptions 클래스 인스턴스를 사용하여 템플릿(기존 mpp 또는 mpt 파일)에서 Project 클래스를 새 인스턴스로 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| 매개변수 | 설명 |
| --- | --- |
| projectTemplate | 프로젝트를 생성할 템플릿 경로 |
| options | 지정된 LoadOptions 클래스 인스턴스. |

---

## Project (13 of 13) {#project_13}

지정된 LoadOptions 클래스 인스턴스를 사용하여 스트림에서 Project 클래스를 새 인스턴스로 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| 매개변수 | 설명 |
| --- | --- |
| stream | Project System::IO::Stream 클래스의 스트림 |
| options | 지정된 LoadOptions 클래스 인스턴스 |

