---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition method"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks untuk C++"
description: "Metode pabrik yang membuat definisi atribut ekstensi dengan lookup."
type: docs
weight: 30
url: /id/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Metode pabrik yang membuat definisi atribut ekstensi dengan pencarian. Memiliki CalculationType yang sama dengan Tasks::CalculationType::Lookup dan hanya dapat digunakan pada Resources. Anda harus menentukan customFieldType, fieldId, dan alias saat memanggil metode ini.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Deskripsi |
| --- | --- |
| customFieldType | Tipe CustomFieldType yang ditentukan. |
| fieldId | ID bidang ExtendedAttributeResource yang ditentukan. |
| alias | Alias System::String yang ditentukan. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Metode pabrik yang membuat definisi atribut ekstended dengan pencarian. Memiliki CalculationType yang sama dengan Tasks::CalculationType::Lookup dan hanya dapat digunakan di Resources. Anda harus menentukan fieldId dan alias saat memanggil metode ini. Tipe bidang disimpulkan dari field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Deskripsi |
| --- | --- |
| fieldId | ID bidang ExtendedAttributeResource yang ditentukan. |
| alias | Alias System::String yang ditentukan. |

