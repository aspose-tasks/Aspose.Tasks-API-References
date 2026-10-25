---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ExtendedAttributeDefinition. Metode pabrik yang membuat definisi atribut ekstensi sederhana yang ditampilkan Microsoft Project sebagai None. Memiliki CalculationType yang sama dengan None dan hanya dapat digunakan pada Tasks. Anda harus menentukan customFieldType, fieldId, dan alias saat memanggil metode ini."
type: docs
weight: 40
url: /id/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Metode pabrik yang membuat definisi atribut ekstensi sederhana, yang ditampilkan Microsoft Project sebagai "None". Memiliki [`CalculationType`](../calculationtype/) yang sama dengan None dan hanya dapat digunakan pada Tasks. Anda harus menentukan *customFieldType*, *fieldId*, dan *alias* saat memanggil metode ini.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| customFieldType | CustomFieldType | Tipe [`CustomFieldType`](../../customfieldtype/) yang ditentukan. |
| fieldId | ExtendedAttributeTask | ID bidang [`ExtendedAttributeTask`](../../extendedattributetask/) yang ditentukan. |
| alias | String | Alias String yang ditentukan. |

### Nilai Kembali

Membuat instance kelas [`ExtendedAttributeDefinition`](../) dengan *customFieldType*, *fieldId*, dan *alias* yang ditentukan.

## Contoh

Gunakan contoh ini untuk membuat definisi bidang teks khusus:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Menampilkan cara membuat atribut tambahan tugas.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Buat Definisi Atribut Tambahan dengan tipe Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Tambahkan ke koleksi Atribut Tambahan proyek
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// Tambahkan tugas ke proyek
var task = project.RootTask.Children.Add("Task 1");

// Buat Atribut Tambahan dari Definisi Atribut
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Tetapkan nilai ke Atribut Tambahan yang dihasilkan. Tipe atribut adalah "Text", properti "TextValue" harus digunakan.
taskExtendedAttributeText1.TextValue = "London";

// Tambahkan Atribut Tambahan ke tugas
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Buat Definisi Atribut Tambahan dengan tipe Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Tambahkan nilai lookup untuk definisi atribut ekstended
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Tambahkan ke koleksi Atribut Tambahan proyek
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// Tambahkan tugas ke proyek
var task2 = project4.RootTask.Children.Add("Task 2");

// Buat Atribut Tambahan dari Definisi Lookup Text2 untuk Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Tambahkan Atribut Tambahan ke tugas
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Buat Definisi Atribut Tambahan dengan tipe Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Tambahkan nilai lookup untuk definisi atribut tambahan
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Tambahkan definisi ke koleksi Atribut Tambahan proyek
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// Tambahkan tugas ke proyek
var task3 = project2.RootTask.Children.Add("Task 3");

// Buat Atribut Tambahan dari Definisi Lookup Duration2 untuk Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Tambahkan Atribut Tambahan ke tugas
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Buat Definisi Atribut Tambahan dengan tipe Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Tambahkan nilai lookup untuk definisi atribut tambahan
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Tambahkan definisi ke koleksi Atribut Tambahan proyek
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// Tambahkan tugas ke proyek
var task4 = project3.RootTask.Children.Add("Task 4");

// Buat Atribut Tambahan dari Definisi Lookup Finish2 untuk Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Tambahkan Atribut Tambahan ke tugas
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan Microsoft Project sebagai "None". Ia memiliki [`CalculationType`](../calculationtype/) yang bernilai None dan hanya dapat digunakan pada Tugas. Anda harus menentukan *fieldId* dan *alias* saat memanggil metode ini. Tipe bidang disimpulkan dari id bidang.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | ID bidang [`ExtendedAttributeTask`](../../extendedattributetask/) yang ditentukan. |
| alias | String | Alias String yang ditentukan. |

### Nilai Kembali

Membuat instance kelas [`ExtendedAttributeDefinition`](../) dengan *fieldId* dan *alias* yang ditentukan.

## Contoh

Gunakan contoh ini untuk membuat definisi bidang teks khusus:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Menampilkan cara membuat definisi atribut ekstensi dan mengatur nilai string atribut saat konstruksinya.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// buat atribut ekstensi dengan nilai yang sama dengan 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// tambahkan atribut ekstensi yang diinisialisasi dengan nilai 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### Lihat Juga

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


