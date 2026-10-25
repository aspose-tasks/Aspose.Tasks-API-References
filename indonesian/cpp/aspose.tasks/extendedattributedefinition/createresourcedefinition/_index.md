---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition metode"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks untuk C++"
description: "Metode pabrik yang membuat definisi atribut ekstended sederhana, yang ditampilkan Microsoft Project sebagai \"None\"."
type: docs
weight: 50
url: /id/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Metode pabrik yang membuat definisi atribut ekstensi sederhana, yang ditampilkan Microsoft Project sebagai "None". Memiliki CalculationType yang sama dengan Tasks::CalculationType::None dan hanya dapat digunakan pada Resource. Anda harus menentukan customFieldType, fieldId, dan alias saat memanggil metode ini.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Deskripsi |
| --- | --- |
| customFieldType | Tipe CustomFieldType yang ditentukan. |
| fieldId | ID bidang ExtendedAttributeResource yang ditentukan. |
| alias | Alias System::String yang ditentukan. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan oleh Microsoft Project sebagai "None". Memiliki CalculationType yang sama dengan Tasks::CalculationType::None dan hanya dapat digunakan pada Resource. Anda harus menentukan fieldId dan alias saat memanggil metode ini. Tipe bidang disimpulkan dari field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Deskripsi |
| --- | --- |
| fieldId | ID bidang ExtendedAttributeResource yang ditentukan. |
| alias | Alias System::String yang ditentukan. |

