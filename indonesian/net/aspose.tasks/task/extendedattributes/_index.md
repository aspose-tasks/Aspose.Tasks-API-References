---
title: "Task.ExtendedAttributes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan objek ExtendedAttributeCollection yang berisi nilai-nilai atribut tambahan"
type: docs
weight: 400
url: /id/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

Mendapatkan objek ExtendedAttributeCollection yang berisi nilai-nilai atribut tambahan.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Catatan

Dua potongan data diperlukan - sebuah penunjuk kembali ke tabel atribut ekstensi yang ditentukan baik dengan ID unik atau Field ID, dan nilai yang ditentukan baik dengan nilai itu sendiri, atau penunjuk kembali ke daftar nilai.

## Contoh

Menampilkan cara membaca atribut tambahan tugas.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Buat definisi atribut yang diperluas
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// Dapatkan tugas indeks nol
var tsk = project.RootTask.Children.GetById(1);

// Tambahkan atribut yang diperluas
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// Juga sintaks singkat berikut dapat digunakan: ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// Buat Definisi Atribut Tambahan dengan tipe Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Tambahkan ke koleksi Atribut Tambahan proyek
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// Buat Atribut Tambahan dari Definisi Atribut
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Tetapkan nilai ke Atribut Tambahan yang dihasilkan. Tipe atribut adalah "Text", properti "TextValue" harus digunakan.
taskExtendedAttributeText1.TextValue = "London";

// Tambahkan Atribut Tambahan ke tugas
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// Buat Definisi Atribut Tambahan dengan tipe Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Tambahkan nilai lookup untuk definisi atribut ekstended
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Tambahkan ke koleksi Atribut Tambahan proyek
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// Buat Atribut Tambahan dari Definisi Lookup Text2 untuk Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Tambahkan Atribut Tambahan ke tugas
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// Buat Definisi Atribut Tambahan dengan tipe Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Tambahkan nilai lookup untuk definisi atribut tambahan
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Tambahkan definisi ke koleksi Atribut Tambahan proyek
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// Buat Atribut Tambahan dari Definisi Lookup Duration2 untuk Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Tambahkan Atribut Tambahan ke tugas
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// Buat Definisi Atribut Tambahan dengan tipe Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Tambahkan nilai lookup untuk definisi atribut tambahan
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Tambahkan definisi ke koleksi Atribut Tambahan proyek
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// Buat Atribut Tambahan dari Definisi Lookup Finish2 untuk Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Tambahkan Atribut Tambahan ke tugas
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Baca atribut ekstended untuk tugas
foreach (var task in collector.Tasks)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}

project.Save(OutDir + "ReadWriteTaskExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


