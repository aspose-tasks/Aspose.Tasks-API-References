---
title: "OutlineCodeCollection.IsReadOnly"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti OutlineCodeCollection. Mendapatkan nilai yang menunjukkan apakah koleksi ini bersifat readonly atau tidak."
type: docs
weight: 20
url: /id/net/aspose.tasks/outlinecodecollection/isreadonly/
---
## OutlineCodeCollection.IsReadOnly property

Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false.

```csharp
public bool IsReadOnly { get; }
```

## Contoh

Menunjukkan cara bekerja dengan koleksi kode outline.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

for (var i = 0; i < collector.Tasks.Count; i++)
{
    var current = collector.Tasks[i];
    if (current.Get(Tsk.Id) == 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes for the " + current.Get(Tsk.Name) + " task.");
    Console.WriteLine("Count of outline codes: " + current.OutlineCodes.Count);
    foreach (var outlineCode in current.OutlineCodes)
    {
        Console.WriteLine("Field Id: " + outlineCode.FieldId);
        Console.WriteLine("Value Id: " + outlineCode.ValueId);
        Console.WriteLine("Value Guid: " + outlineCode.ValueGuid);
        Console.WriteLine();
    }
}

// tambahkan definisi kode outline khusus
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
project.OutlineCodes.Add(outlineCodeDefinition);

// buat kode outline
var value = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(value);

var codeOne = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 1, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

var task = project.RootTask.Children.GetByUid(2);

// bisa memeriksa bahwa koleksi tidak bersifat hanya baca
if (!task.OutlineCodes.IsReadOnly)
{
    task.OutlineCodes.Add(codeOne);
}

var codeZero = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 0, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

task.OutlineCodes.Insert(0, codeZero);

var code2 = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 2, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

// sisipkan kode dengan 2 pada posisi yang salah
task.OutlineCodes.Insert(0, code2);

// perbaiki itu
var indexOf = task.OutlineCodes.IndexOf(code2);
task.OutlineCodes.RemoveAt(indexOf);

// sisipkan kode dengan 2 pada posisi yang benar
task.OutlineCodes.Insert(2, code2);

// periksa bahwa kode telah disisipkan
Console.WriteLine("Is outline codes contains the inserted value: " + task.OutlineCodes.Contains(code2));

// ...
// bekerja dengan kode outline
// ...
var otherProject = new Project(DataDir + "OutlineCodes2003.mpp");
var otherTask = otherProject.RootTask.Children.GetById(2);

// tambahkan definisi kode outline khusus
outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
otherProject.OutlineCodes.Add(outlineCodeDefinition);

// buat kode outline
var otherValue = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(otherValue);

var outlineCodes = new OutlineCode[task.OutlineCodes.Count];
task.OutlineCodes.CopyTo(outlineCodes, 0);

foreach (var code in outlineCodes)
{
    otherTask.OutlineCodes.Add(code);
}

// ...
// bekerja dengan kode outline
// ...

// hapus kode outline
otherTask.OutlineCodes.RemoveAt(0);

while (otherTask.OutlineCodes.Count > 0)
{
    otherTask.OutlineCodes.Remove(otherTask.OutlineCodes[0]);
}

// bersihkan semua nilai sekaligus
task.OutlineCodes.Clear();
```

### Lihat Juga

* class [OutlineCodeCollection](../)
* namespace [Aspose.Tasks](../../outlinecodecollection/)
* assembly [Aspose.Tasks](../../../)


