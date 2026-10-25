---
title: "Kelas OutlineValueCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.OutlineValueCollection. Mewakili koleksi objek OutlineValue"
type: docs
weight: 1220
url: /id/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

Mewakili koleksi objek [`OutlineValue`](../outlinevalue/) .

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam koleksi ini. |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca. |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | Mengembalikan atau mengatur elemen pada indeks yang ditentukan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | Menambahkan item yang ditentukan ke koleksi ini. |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | Menghapus semua item dari koleksi ini. |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false. |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan. |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | Menentukan indeks dari item yang ditentukan dalam koleksi ini. |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | Menyisipkan item yang ditentukan pada indeks yang ditentukan. |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | Menghapus kemunculan pertama dari objek tertentu dari koleksi ini. |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | Menghapus sebuah item pada indeks yang ditentukan. |

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

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


