---
title: "ExtendedAttributeDefinition.CreateLookupResourceDefinition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ExtendedAttributeDefinition. Metode pabrik yang membuat definisi atribut ekstensi dengan pencarian. Memiliki CalculationType yang sama dengan Lookup dan hanya dapat digunakan pada Resources. Anda harus menentukan fieldId dan alias saat memanggil metode ini. Tipe bidang disimpulkan dari field id."
type: docs
weight: 10
url: /id/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Metode pabrik yang membuat definisi atribut ekstensi dengan pencarian. Memiliki [`CalculationType`](../calculationtype/) yang sama dengan Lookup dan hanya dapat digunakan pada Resources. Anda harus menentukan *fieldId* dan *alias* saat memanggil metode ini. Tipe bidang disimpulkan dari field id.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | ID bidang [`ExtendedAttributeResource`](../../extendedattributeresource/) yang ditentukan. |
| alias | String | Alias String yang ditentukan. |

### Nilai Kembali

Membuat instance kelas [`ExtendedAttributeDefinition`](../) dengan *fieldId* dan *alias* yang ditentukan.

## Contoh

Gunakan contoh ini untuk membuat definisi bidang khusus untuk sumber daya dengan pencarian, lalu mengisinya dengan nilai teks:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

Menampilkan cara menulis definisi atribut ekstensi yang diperbarui.

```csharp
var project = new Project(DataDir + "WriteUpdatedExtendedAttributeDefinitions.mpp");

// Tambahkan atribut ekstensi text3 baru dengan pencarian dan satu nilai pencarian
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text3, "New text3 attribute");
definition.ElementType = ElementType.Task;
project.ExtendedAttributes.Add(definition);

var textVal = new Value
{
    Id = 1,
    Description = "Text value descr",
    Val = "Text value1"
};

definition.AddLookupValue(textVal);

// Tambahkan atribut ekstensi cost1 baru dengan pencarian dan dua nilai biaya
var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Cost1, "New cost1 attribute");
project.ExtendedAttributes.Add(taskCostAttributeDefinition);

var costVal1 = new Value
{
    Id = 2,
    Description = "Cost value 1 descr",
    Val = "99900"
};

var costVal2 = new Value
{
    Id = 3,
    Description = "Cost value 2 descr",
    Val = "11100"
};

taskCostAttributeDefinition.AddLookupValue(costVal1);
taskCostAttributeDefinition.AddLookupValue(costVal2);

// Tambahkan tugas baru dan tetapkan nilai pencarian atribut.
var task = project.RootTask.Children.Add("New task");

var taskAttr = taskCostAttributeDefinition.CreateExtendedAttribute(costVal1);
task.ExtendedAttributes.Add(taskAttr);

var taskStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Start7, "New start 7 attribute");

var startVal = new Value
{
    Id = 4,
    DateTimeValue = DateTime.Now,
    Description = "Start 7 value description"
};

taskStartAttributeDefinition.AddLookupValue(startVal);

project.ExtendedAttributes.Add(taskStartAttributeDefinition);

var taskFinishAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Finish4, "New finish 4 attribute");

var finishVal = new Value
{
    Id = 5,
    DateTimeValue = DateTime.Now,
    Description = "Finish 4 value description"
};

taskFinishAttributeDefinition.ValueList.Add(finishVal);

project.ExtendedAttributes.Add(taskFinishAttributeDefinition);

var numberAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Number20, "New number attribute");

var val1 = new Value
{
    Id = 6,
    Val = "1",
    Description = "Number 1 value"
};
var val2 = new Value
{
    Id = 7,
    Val = "2",
    Description = "Number 2 value"
};
var val3 = new Value();
val2.Id = 8;
val3.Val = "3";
val3.Description = "Number 3 value";

numberAttributeDefinition.AddLookupValue(val1);
numberAttributeDefinition.AddLookupValue(val2);
numberAttributeDefinition.AddLookupValue(val3);

project.ExtendedAttributes.Add(numberAttributeDefinition);

var rscStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Start5, "New start5 attribute");

var value = new Value
{
    Id = 9,
    DateTimeValue = DateTime.Now,
    Description = "this is start5 value descr"
};

rscStartAttributeDefinition.AddLookupValue(value);

project.ExtendedAttributes.Add(rscStartAttributeDefinition);

// Definisikan atribut durasi tanpa pencarian.
var taskDurationAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "New Duration");
project.ExtendedAttributes.Add(taskDurationAttributeDefinition);

// Tambahkan tugas baru dan tetapkan nilai durasi ke atribut durasi yang telah didefinisikan sebelumnya.
var timeTask = project.RootTask.Children.Add("New task");

var durationExtendedAttribute = taskDurationAttributeDefinition.CreateExtendedAttribute();

durationExtendedAttribute.DurationValue = project.GetDuration(3.0, TimeUnitType.Hour);
timeTask.ExtendedAttributes.Add(durationExtendedAttribute);

var options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "WriteUpdatedExtendedAttributeDefinitions_out.mpp", options);
```

### Lihat Juga

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Metode pabrik yang membuat definisi atribut ekstensi dengan pencarian. Memiliki [`CalculationType`](../calculationtype/) yang sama dengan Lookup dan hanya dapat digunakan pada Resources. Anda harus menentukan *customFieldType*, *fieldId*, dan *alias* saat memanggil metode ini.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| customFieldType | CustomFieldType | Tipe [`CustomFieldType`](../../customfieldtype/) yang ditentukan. |
| fieldId | ExtendedAttributeResource | ID bidang [`ExtendedAttributeResource`](../../extendedattributeresource/) yang ditentukan. |
| alias | String | Alias String yang ditentukan. |

### Nilai Kembali

Membuat instance kelas [`ExtendedAttributeDefinition`](../) dengan *customFieldType*, *fieldId*, dan *alias* yang ditentukan.

## Contoh

Gunakan contoh ini untuk membuat definisi bidang khusus untuk sumber daya dengan pencarian, lalu mengisinya dengan nilai teks:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

Menampilkan cara menambahkan atribut tambahan dengan pencarian untuk penugasan.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Tetapkan sumber daya "1 TRG: Trade Group" ke "TASK 1" dengan membuat objek ResourceAssignment.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Buat definisi atribut kustom dengan pencarian.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Nilai ini dapat dilihat di tampilan "Resource usage" pada MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Buat definisi atribut kustom dengan pencarian.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Nilai ini dapat dilihat di tampilan "Task usage" pada MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// nilai yang salah dapat dihapus nanti
taskCostAttr.RemoveLookupValue(taskWrongValue);

// bekerja dengan proyek...
```

### Lihat Juga

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


