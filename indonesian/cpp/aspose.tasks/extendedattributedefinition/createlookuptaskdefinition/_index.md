---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition metode"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks untuk C++"
description: "Metode pabrik yang membuat definisi atribut ekstensi dengan lookup."
type: docs
weight: 40
url: /id/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Metode pabrik yang membuat definisi atribut ekstensi dengan pencarian. Memiliki CalculationType yang sama dengan Tasks::CalculationType::Lookup dan hanya dapat digunakan pada Tasks. Anda harus menentukan customFieldType, fieldId, dan alias saat memanggil metode ini.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Deskripsi |
| --- | --- |
| customFieldType | Tipe CustomFieldType yang ditentukan. |
| fieldId | ID bidang ExtendedAttributeTask yang ditentukan. |
| alias | Alias System::String yang ditentukan. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Metode pabrik yang membuat definisi atribut ekstended dengan pencarian. Memiliki CalculationType yang sama dengan Tasks::CalculationType::Lookup dan hanya dapat digunakan di Tasks. Anda harus menentukan fieldId dan alias saat memanggil metode ini. Tipe bidang disimpulkan dari field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Deskripsi |
| --- | --- |
| fieldId | ID bidang ExtendedAttributeTask yang ditentukan. |
| alias | Alias System::String yang ditentukan. |

