---
title: AddLookupValue
second_title: Aspose.Tasks untuk Referensi .NET API
description: Menambahkan nilai ke daftar pencarian internal. Ini adalah cara yang lebih disukai untuk manipulasi denganValueListaspose.tasks/extendedattributedefinition/valuelist/ .
type: docs
weight: 290
url: /id/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Menambahkan nilai ke daftar pencarian internal. Ini adalah cara yang lebih disukai untuk manipulasi dengan[`ValueList`](../valuelist/) .

```csharp
public void AddLookupValue(Value value)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| value | Value | Nilai untuk ditambahkan ke dalam pencarian. |

### Perkataan

Metode ini hanya berfungsi untuk[`ExtendedAttributeDefinition`](../) instances yang memiliki[`CalculationType`](../calculationtype/) sama denganLookup .

### Contoh

Gunakan kode ini untuk menambahkan Nilai baru ke daftar pencarian:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### Lihat juga

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
