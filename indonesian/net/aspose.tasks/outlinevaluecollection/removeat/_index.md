---
title: "OutlineValueCollection.RemoveAt"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode OutlineValueCollection. Menghapus item pada indeks yang ditentukan"
type: docs
weight: 120
url: /id/net/aspose.tasks/outlinevaluecollection/removeat/
---
## OutlineValueCollection.RemoveAt method

Menghapus sebuah item pada indeks yang ditentukan.

```csharp
public void RemoveAt(int index)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | Int32 | indeks berbasis nol yang ditentukan untuk menghapus item. |

## Contoh

Menampilkan cara bekerja dengan koleksi nilai outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// hapus koleksi nilai
foreach (var outlineCode in project.OutlineCodes)
{
    // hapus mask outline
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// perbarui nilai melalui akses indeks
codeDefinition.Values[0].Value = "654321";

// iterasi atas nilai outline
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// bekerja dengan nilai outline
// ...

// hapus nilai bila diperlukan
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// sisipkan nilai pada posisi awal
codeDefinition.Values.Insert(0, value);

// periksa posisi nilai yang disisipkan
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// bekerja dengan nilai outline
// ...

// hapus nilai terakhir dari koleksi
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// seseorang dapat membuat definisi kode outline lainnya
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// dan kemudian menyalin nilai outline
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### Lihat Juga

* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


