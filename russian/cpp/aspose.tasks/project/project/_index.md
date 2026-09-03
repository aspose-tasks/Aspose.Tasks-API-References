---
title: "Aspose::Tasks::Project::Project конструктор"
linktitle: "Проект"
articleTitle: "Проект"
second_title: "Aspose.Tasks для C++"
description: "Инициализирует новый экземпляр класса Project."
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Инициализирует новый экземпляр класса Project.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

Инициализирует новый экземпляр класса Project из защищённого паролем шаблона (существующий файл mpp или mpt).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| Параметр | Описание |
| --- | --- |
| projectTemplate | Путь к шаблону, из которого создаётся проект. |
| protectionPassword | Пароль защиты. |

---

## Project (3 of 13) {#project_3}

Инициализирует новый экземпляр класса Project из шаблона (существующий файл mpp или mpt).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| Параметр | Описание |
| --- | --- |
| projectTemplate | Путь к шаблону, из которого создаётся проект. |

---

## Project (4 of 13) {#project_4}

Инициализирует новый экземпляр класса Project из потока с указанным экземпляром класса PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Параметр | Описание |
| --- | --- |
| stream | Поток класса Project System::IO::Stream |
| options | указанный экземпляр класса PrimaveraReadOptions, который позволяет настраивать чтение форматов Primavera (XER или XML). |

---

## Project (5 of 13) {#project_5}

Инициализирует новый экземпляр класса Project из шаблона (существующий файл mpp или mpt).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Параметр | Описание |
| --- | --- |
| projectTemplate | Путь к шаблону, из которого создаётся проект. |
| parseErrorHandler | указанный метод обратного вызова для обработки ошибок разбора xml. |

---

## Project (6 of 13) {#project_6}

Инициализирует новый экземпляр класса Project из потока.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| Параметр | Описание |
| --- | --- |
| stream | Поток для загрузки шаблона. |

---

## Project (7 of 13) {#project_7}

Инициализирует новый экземпляр класса Project из экземпляра StreamReader.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| Параметр | Описание |
| --- | --- |
| reader | Потоковый читатель, из которого загружается шаблон. |

---

## Project (8 of 13) {#project_8}

Инициализирует новый экземпляр класса Project из шаблона (существующего файла MPP или MPT) с указанным экземпляром класса PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Параметр | Описание |
| --- | --- |
| projectTemplate | Путь к шаблону, из которого создаётся проект |
| options | указанный экземпляр класса PrimaveraReadOptions. |

---

## Project (9 of 13) {#project_9}

Инициализирует новый экземпляр класса Project для чтения данных из базы данных, указанной экземпляром класса DbSettings.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| Параметр | Описание |
| --- | --- |
| настройки | указанный экземпляр класса DbSettings. |

---

## Project (10 of 13) {#project_10}

Инициализирует новый экземпляр класса Project из шаблона (существующего файла mpp или mpt).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| Параметр | Описание |
| --- | --- |
| stream | Поток для загрузки шаблона. |
| parseErrorHandler | указанный метод обратного вызова для обработки ошибок разбора xml. |

---

## Project (11 of 13) {#project_11}

Инициализирует новый экземпляр класса Project из шаблона (существующего файла mpp или mpt).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| Параметр | Описание |
| --- | --- |
| stream | Поток для загрузки шаблона. |
| protectionPassword | Пароль защиты. |

---

## Project (12 of 13) {#project_12}

Инициализирует новый экземпляр класса Project из шаблона (существующего файла mpp или mpt) с указанным экземпляром класса LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| Параметр | Описание |
| --- | --- |
| projectTemplate | Путь к шаблону, из которого создаётся проект |
| options | указанный экземпляр класса LoadOptions. |

---

## Project (13 of 13) {#project_13}

Инициализирует новый экземпляр класса Project из потока с указанным экземпляром класса LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| Параметр | Описание |
| --- | --- |
| stream | Поток класса Project System::IO::Stream |
| options | указанный экземпляр класса LoadOptions |

