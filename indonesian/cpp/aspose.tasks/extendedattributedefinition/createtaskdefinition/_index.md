---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition metode"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks untuk C++"
description: "Metode pabrik yang membuat definisi atribut ekstended sederhana, yang ditampilkan Microsoft Project sebagai \"None\"."
type: docs
weight: 60
url: /id/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Metode pabrik yang membuat definisi atribut ekstensi sederhana, yang ditampilkan Microsoft Project sebagai "None". Memiliki CalculationType yang sama dengan Tasks::CalculationType::None dan hanya dapat digunakan pada Tasks. Anda harus menentukan customFieldType, fieldId, dan alias saat memanggil metode ini.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Deskripsi |
| --- | --- |
| customFieldType | Tipe CustomFieldType yang ditentukan. |
| fieldId | ID bidang ExtendedAttributeTask yang ditentukan. |
| alias | Alias System::String yang ditentukan. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Metode pabrik yang membuat definisi atribut ekstended sederhana, yang ditampilkan Microsoft Project sebagai "None". Memiliki CalculationType yang sama dengan Tasks::CalculationType::None dan hanya dapat digunakan di Tasks. Anda harus menentukan fieldId dan alias saat memanggil metode ini. Tipe bidang disimpulkan dari field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Deskripsi |
| --- | --- |
| fieldId | ID bidang ExtendedAttributeTask yang ditentukan. |
| alias | Alias System::String yang ditentukan. |

