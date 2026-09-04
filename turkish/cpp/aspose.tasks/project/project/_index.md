---
title: "Aspose::Tasks::Project::Project yapıcı"
linktitle: "Project"
articleTitle: "Project"
second_title: "C++ için Aspose.Tasks"
description: "Project sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

Şifre korumalı bir şablondan (var olan mpp veya mpt dosyası) Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| Parametre | Açıklama |
| --- | --- |
| projectTemplate | Projeyi oluşturmak için şablonun yolu. |
| protectionPassword | Koruma şifresi. |

---

## Project (3 of 13) {#project_3}

Şablondan (var olan mpp veya mpt dosyası) Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| Parametre | Açıklama |
| --- | --- |
| projectTemplate | Projeyi oluşturmak için şablonun yolu. |

---

## Project (4 of 13) {#project_4}

Belirtilen PrimaveraReadOptions sınıfı örneğiyle Stream'den Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parametre | Açıklama |
| --- | --- |
| stream | Project System::IO::Stream sınıfının akışı |
| options | Primavera formatlarının (XER veya XML) okunmasını özelleştirmeye izin veren PrimaveraReadOptions sınıfının belirtilen örneği. |

---

## Project (5 of 13) {#project_5}

Şablondan (var olan mpp veya mpt dosyası) Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parametre | Açıklama |
| --- | --- |
| projectTemplate | Projeyi oluşturmak için şablonun yolu. |
| parseErrorHandler | XML ayrıştırma hatalarını işlemek için belirtilen geri çağırma yöntemi. |

---

## Project (6 of 13) {#project_6}

Bir akıştan Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| Parametre | Açıklama |
| --- | --- |
| stream | Şablonun yükleneceği akış. |

---

## Project (7 of 13) {#project_7}

StreamReader örneğinden Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| Parametre | Açıklama |
| --- | --- |
| reader | Şablonun yükleneceği akış okuyucu. |

---

## Project (8 of 13) {#project_8}

Şablondan (var olan MPP veya MPT dosyası) ve belirtilen PrimaveraReadOptions sınıfı örneğiyle Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parametre | Açıklama |
| --- | --- |
| projectTemplate | Projeyi oluşturmak için şablonun yolu |
| options | PrimaveraReadOptions sınıfının belirtilen örneği. |

---

## Project (9 of 13) {#project_9}

DbSettings sınıfının örneği tarafından belirtilen bir veritabanından veri okumak için Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| Parametre | Açıklama |
| --- | --- |
| ayarlar | DbSettings sınıfının belirtilen örneği. |

---

## Project (10 of 13) {#project_10}

Varolan mpp veya mpt dosyasından bir şablonla Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| Parametre | Açıklama |
| --- | --- |
| stream | Şablonun yükleneceği akış. |
| parseErrorHandler | XML ayrıştırma hatalarını işlemek için belirtilen geri çağırma yöntemi. |

---

## Project (11 of 13) {#project_11}

Varolan mpp veya mpt dosyasından bir şablonla Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| Parametre | Açıklama |
| --- | --- |
| stream | Şablonun yükleneceği akış. |
| protectionPassword | Koruma şifresi. |

---

## Project (12 of 13) {#project_12}

Belirtilen LoadOptions sınıfı örneğiyle varolan mpp veya mpt dosyasından bir şablon kullanarak Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| Parametre | Açıklama |
| --- | --- |
| projectTemplate | Projeyi oluşturmak için şablonun yolu |
| options | LoadOptions sınıfının belirtilen örneği. |

---

## Project (13 of 13) {#project_13}

Belirtilen LoadOptions sınıfı örneğiyle Stream'den Project sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| Parametre | Açıklama |
| --- | --- |
| stream | Project System::IO::Stream sınıfının akışı |
| options | LoadOptions sınıfının belirtilen örneği |

