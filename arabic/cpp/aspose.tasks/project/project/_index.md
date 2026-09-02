---
title: "منشئ Aspose::Tasks::Project::Project"
linktitle: "Project"
articleTitle: "Project"
second_title: "Aspose.Tasks لـ C++"
description: "يُنشئ مثيلًا جديدًا من فئة Project."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

يُنشئ مثيلًا جديدًا من فئة Project.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

يُنشئ مثيلاً جديدًا لفئة Project من قالب محمي بكلمة مرور (ملف mpp أو mpt موجود).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| معامل | الوصف |
| --- | --- |
| projectTemplate | المسار إلى القالب لإنشاء المشروع منه. |
| protectionPassword | كلمة مرور الحماية. |

---

## Project (3 of 13) {#project_3}

يُنشئ مثيلاً جديدًا لفئة Project من قالب (ملف mpp أو mpt موجود).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| معامل | الوصف |
| --- | --- |
| projectTemplate | المسار إلى القالب لإنشاء المشروع منه. |

---

## Project (4 of 13) {#project_4}

يُنشئ مثيلاً جديدًا لفئة Project من الـ Stream مع المثيل المحدد من فئة PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| معامل | الوصف |
| --- | --- |
| stream | دفق من فئة Project System::IO::Stream |
| options | المثيل المحدد من فئة PrimaveraReadOptions الذي يسمح بتخصيص قراءة صيغ Primavera (XER أو XML). |

---

## Project (5 of 13) {#project_5}

يُنشئ مثيلاً جديدًا لفئة Project من قالب (ملف mpp أو mpt موجود).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| معامل | الوصف |
| --- | --- |
| projectTemplate | المسار إلى القالب لإنشاء المشروع منه. |
| parseErrorHandler | طريقة الاستدعاء المحددة لمعالجة أخطاء تحليل XML. |

---

## Project (6 of 13) {#project_6}

يُنشئ مثيلاً جديدًا لفئة Project من دفق.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| معامل | الوصف |
| --- | --- |
| stream | دفق لتحميل القالب منه. |

---

## Project (7 of 13) {#project_7}

يُنشئ مثيلاً جديدًا لفئة Project من مثيل StreamReader.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| معامل | الوصف |
| --- | --- |
| reader | قارئ الدفق الذي يُحمَّل منه القالب. |

---

## Project (8 of 13) {#project_8}

يُنشئ مثيلاً جديدًا لفئة Project من قالب (ملف MPP أو MPT موجود) مع المثيل المحدد من فئة PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| معامل | الوصف |
| --- | --- |
| projectTemplate | المسار إلى القالب لإنشاء المشروع منه |
| options | المثيل المحدد من فئة PrimaveraReadOptions. |

---

## Project (9 of 13) {#project_9}

يُنشئ مثيلًا جديدًا من فئة Project لقراءة البيانات من قاعدة بيانات يتم تحديدها بواسطة مثيل فئة DbSettings.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| معامل | الوصف |
| --- | --- |
| الإعدادات | المثيل المحدد من فئة DbSettings. |

---

## Project (10 of 13) {#project_10}

يُنشئ مثيلًا جديدًا من فئة Project من قالب (ملف mpp أو mpt موجود).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| معامل | الوصف |
| --- | --- |
| stream | دفق لتحميل القالب منه. |
| parseErrorHandler | طريقة الاستدعاء المحددة لمعالجة أخطاء تحليل XML. |

---

## Project (11 of 13) {#project_11}

يُنشئ مثيلًا جديدًا من فئة Project من قالب (ملف mpp أو mpt موجود).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| معامل | الوصف |
| --- | --- |
| stream | دفق لتحميل القالب منه. |
| protectionPassword | كلمة مرور الحماية. |

---

## Project (12 of 13) {#project_12}

يُنشئ مثيلًا جديدًا من فئة Project من قالب (ملف mpp أو mpt موجود) مع المثيل المحدد من فئة LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| معامل | الوصف |
| --- | --- |
| projectTemplate | المسار إلى القالب لإنشاء المشروع منه |
| options | المثيل المحدد من فئة LoadOptions. |

---

## Project (13 of 13) {#project_13}

يُنشئ مثيلًا جديدًا من فئة Project من الـ Stream مع المثيل المحدد من فئة LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| معامل | الوصف |
| --- | --- |
| stream | دفق من فئة Project System::IO::Stream |
| options | المثيل المحدد من فئة LoadOptions |

