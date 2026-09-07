---
title: "ExtendedAttribute.FlagValue"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ExtendedAttribute. Mendapatkan atau mengatur nilai yang menunjukkan apakah flag diatur untuk atribut dengan tipe Flag"
type: docs
weight: 50
url: /id/net/aspose.tasks/extendedattribute/flagvalue/
---
## ExtendedAttribute.FlagValue property

Mendapatkan atau mengatur nilai yang menunjukkan apakah flag diatur untuk atribut dengan tipe 'Flag'.

```csharp
public bool FlagValue { get; set; }
```

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Dilemparkan jika properti [`AttributeDefinition`](../attributedefinition/) tidak diinisialisasi atau atribut saat ini bukan atribut flag. |

## Contoh

Menampilkan cara membuat atribut extended boolean.

```csharp
var project = new Project();

// buat definisi atribut ekstended tugas baru
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Flag, ExtendedAttributeTask.Flag1, "Is Finished");

// menambahkan formula ke atribut.
definition.Formula = "[% Complete] = 100";

project.ExtendedAttributes.Add(definition);

var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.ActualDuration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.ActualFinish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.PercentComplete, 100);

var running = project.RootTask.Children.Add("Task");
running.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
running.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
running.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
running.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));

Console.WriteLine(running.Get(Tsk.PercentComplete));
// membuat atribut extended
var runningFlagAttribute = definition.CreateExtendedAttribute();
var finishedFlagAttribute = definition.CreateExtendedAttribute();
running.ExtendedAttributes.Add(runningFlagAttribute);
finished.ExtendedAttributes.Add(finishedFlagAttribute);

Console.WriteLine("Alias: {0}\n", definition.Alias);
Console.WriteLine("(Finished Task) Field Id: " + finishedFlagAttribute.FieldId);
Console.WriteLine("(Finished Task) Value: {0}\n", finishedFlagAttribute.FlagValue);
Console.WriteLine("(Running Task) Field Id: " + runningFlagAttribute.FieldId);
Console.WriteLine("(Running Task) Value: " + runningFlagAttribute.FlagValue);
```

### Lihat Juga

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


