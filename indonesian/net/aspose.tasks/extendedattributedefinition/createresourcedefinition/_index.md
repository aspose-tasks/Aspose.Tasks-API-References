---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ExtendedAttributeDefinition. Metode pabrik yang membuat definisi atribut yang diperluas sederhana yang ditampilkan Microsoft Project sebagai None. Memiliki CalculationType yang bernilai None dan hanya dapat digunakan pada Resource. Anda harus menentukan customFieldType, fieldId, dan alias saat memanggil metode ini."
type: docs
weight: 30
url: /id/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Metode pabrik yang membuat definisi atribut yang diperluas sederhana, yang ditampilkan Microsoft Project sebagai "None". Memiliki [`CalculationType`](../calculationtype/) yang bernilai None dan hanya dapat digunakan pada Resource. Anda harus menentukan *customFieldType*, *fieldId*, dan *alias* saat memanggil metode ini.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| customFieldType | CustomFieldType | Tipe [`CustomFieldType`](../../customfieldtype/) yang ditentukan. |
| fieldId | ExtendedAttributeResource | ID bidang [`ExtendedAttributeResource`](../../extendedattributeresource/) yang ditentukan. |
| alias | String | Alias String yang ditentukan. |

### Nilai Kembali

Membuat instance kelas [`ExtendedAttributeDefinition`](../) dengan *customFieldType*, *fieldId*, dan *alias* yang ditentukan.

## Contoh

Gunakan contoh ini untuk membuat definisi bidang teks khusus:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Menampilkan cara menambahkan atribut yang diperluas ke penugasan sumber daya.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Tambahkan tugas dan sumber daya baru
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // Atribut khusus yang terlihat di tampilan "Resource Usage" dapat dibuat dengan metode ExtendedAttributeDefinition.CreateResourceDefinition.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // Tipe atribut adalah "Cost", jadi kita perlu menggunakan properti "NumericValue".
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // Atribut khusus yang terlihat di tampilan "Task Usage" dapat dibuat dengan metode ExtendedAttributeDefinition.CreateTaskDefinition.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // Tipe atribut adalah "Cost", jadi kita perlu menggunakan properti "NumericValue".
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Metode pabrik yang membuat definisi atribut yang diperluas sederhana, yang ditampilkan Microsoft Project sebagai "None". Memiliki [`CalculationType`](../calculationtype/) yang bernilai None dan hanya dapat digunakan pada Resource. Anda harus menentukan *fieldId* dan *alias* saat memanggil metode ini. Tipe bidang disimpulkan dari field id.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | ID bidang [`ExtendedAttributeResource`](../../extendedattributeresource/) yang ditentukan. |
| alias | String | Alias String yang ditentukan. |

### Nilai Kembali

Membuat instance kelas [`ExtendedAttributeDefinition`](../) dengan *fieldId* dan *alias* yang ditentukan.

## Contoh

Gunakan contoh ini untuk membuat definisi bidang teks khusus:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Menampilkan cara membuat definisi atribut yang diperluas dan mengatur nilai flag saat sedang dibangun.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// buat definisi untuk bidang khusus boolean
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// buat atribut dan atur nilai awal menjadi 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### Lihat Juga

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


