---
title: "Aspose::Tasks::Project::Project constructor"
linktitle: "Project"
articleTitle: "Project"
second_title: "Aspose.Tasks for C++"
description: "Initializes a new instance of the Project class."
type: docs
weight: 10
url: /cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Initializes a new instance of the Project class.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

Initializes a new instance of the Project class from a password protected template (existent mpp or mpt file).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| Parameter | Description |
| --- | --- |
| projectTemplate | Path to template to create project from. |
| protectionPassword | Protection password. |

---

## Project (3 of 13) {#project_3}

Initializes a new instance of the Project class from a template (existent mpp or mpt file).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| Parameter | Description |
| --- | --- |
| projectTemplate | Path to template to create project from. |

---

## Project (4 of 13) {#project_4}

Initializes a new instance of the Project class from the Stream with the specified instance of the PrimaveraReadOptions class.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parameter | Description |
| --- | --- |
| stream | Stream of the Project System::IO::Stream class |
| options | the specified instance of the PrimaveraReadOptions class which allows to customize reading of Primavera formats (XER or XML). |

---

## Project (5 of 13) {#project_5}

Initializes a new instance of the Project class from a template (existent mpp or mpt file).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parameter | Description |
| --- | --- |
| projectTemplate | Path to template to create project from. |
| parseErrorHandler | the specified callback method to handle xml parse errors. |

---

## Project (6 of 13) {#project_6}

Initializes a new instance of the Project class from a stream.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| Parameter | Description |
| --- | --- |
| stream | Stream to load a template from. |

---

## Project (7 of 13) {#project_7}

Initializes a new instance of the Project class from a StreamReader instance.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| Parameter | Description |
| --- | --- |
| reader | The stream reader where to load a template from. |

---

## Project (8 of 13) {#project_8}

Initializes a new instance of the Project class from a template (existent MPP or MPT file) with the specified instance of the PrimaveraReadOptions class.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parameter | Description |
| --- | --- |
| projectTemplate | Path to template to create project from |
| options | the specified instance of the PrimaveraReadOptions class. |

---

## Project (9 of 13) {#project_9}

Initializes a new instance of the Project class to read data from a database which is specified by the instance of the DbSettings class.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| Parameter | Description |
| --- | --- |
| settings | the specified instance of the DbSettings class. |

---

## Project (10 of 13) {#project_10}

Initializes a new instance of the Project class from a template(existent mpp or mpt file).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| Parameter | Description |
| --- | --- |
| stream | Stream to load a template from. |
| parseErrorHandler | the specified callback method to handle xml parse errors. |

---

## Project (11 of 13) {#project_11}

Initializes a new instance of the Project class from a template(existent mpp or mpt file).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| Parameter | Description |
| --- | --- |
| stream | Stream to load a template from. |
| protectionPassword | Protection password. |

---

## Project (12 of 13) {#project_12}

Initializes a new instance of the Project class from a template (existent mpp or mpt file) with the specified instance of the LoadOptions class.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| Parameter | Description |
| --- | --- |
| projectTemplate | Path to template to create project from |
| options | the specified instance of the LoadOptions class. |

---

## Project (13 of 13) {#project_13}

Initializes a new instance of the Project class from the Stream with the specified instance of the LoadOptions class.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| Parameter | Description |
| --- | --- |
| stream | Stream of the Project System::IO::Stream class |
| options | the specified instance of the LoadOptions class |

