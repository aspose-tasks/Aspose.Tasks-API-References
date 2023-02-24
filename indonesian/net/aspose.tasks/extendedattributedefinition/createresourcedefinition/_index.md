---
title: CreateResourceDefinition
second_title: Aspose.Tasks untuk Referensi .NET API
description: Metode pabrik yang membuat definisi atribut tambahan sederhana yang ditampilkan Microsoft Project sebagai Tidak Ada. MemilikiCalculationTypeaspose.tasks/extendedattributedefinition/calculationtype/ sama denganNone dan hanya dapat digunakan di Resource. Anda harus menentukancustomFieldType fieldId Danalias saat memanggil metode ini.
type: docs
weight: 30
url: /id/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan Microsoft Project sebagai "Tidak Ada". Memiliki[`CalculationType`](../calculationtype/) sama denganNone dan hanya dapat digunakan di Resource. Anda harus menentukan*customFieldType* ,*fieldId* Dan*alias* saat memanggil metode ini.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| customFieldType | CustomFieldType | Yang ditentukan[`CustomFieldType`](../../customfieldtype/) jenis. |
| fieldId | ExtendedAttributeResource | Yang ditentukan[`ExtendedAttributeResource`](../../extendedattributeresource/) ID lapangan. |
| alias | String | Yang ditentukanString alias. |

### Nilai Pengembalian

Contoh yang dibuat dari[`ExtendedAttributeDefinition`](../) kelas dengan yang ditentukan*customFieldType* ,*fieldId* Dan*alias*.

### Contoh

Gunakan contoh ini untuk membuat definisi bidang teks kustom:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Lihat juga

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan Microsoft Project sebagai "Tidak Ada". Memiliki[`CalculationType`](../calculationtype/) sama denganNone dan hanya dapat digunakan di Resource. Anda harus menentukan*fieldId* Dan*alias* saat memanggil metode ini. Jenis bidang disimpulkan dari id bidang.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Yang ditentukan[`ExtendedAttributeResource`](../../extendedattributeresource/) ID lapangan. |
| alias | String | Yang ditentukanString alias. |

### Nilai Pengembalian

Contoh yang dibuat dari[`ExtendedAttributeDefinition`](../) kelas dengan yang ditentukan*fieldId* Dan*alias*.

### Contoh

Gunakan contoh ini untuk membuat definisi bidang teks kustom:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Lihat juga

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->