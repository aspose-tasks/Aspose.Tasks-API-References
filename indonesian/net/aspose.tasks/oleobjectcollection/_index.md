---
title: "Kelas OleObjectCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.OleObjectCollection. Mewakili koleksi yang berisi instance dari kelas OleObject."
type: docs
weight: 1130
url: /id/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

Mewakili koleksi yang berisi instance dari kelas [`OleObject`](../oleobject/).

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | Menghapus koleksi. Untuk mempertahankan perubahan ini, project.Save harus dipanggil dengan MPPSaveOptions baru { WriteViewData = true; } |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | Mengonversi instance dari kelas `OleObjectCollection` menjadi daftar yang berisi instance dari kelas [`OleObject`](../oleobject/). |

## Contoh

Menampilkan cara bekerja dengan koleksi objek OLE.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// dengan menggunakan akses indeks
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// atau enumerasi yang dapat mengiterasi objek OLE
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### Lihat Juga

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


