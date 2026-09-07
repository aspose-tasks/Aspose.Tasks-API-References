---
title: "OleObjectCollection.ToList"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode OleObjectCollection. Mengonversi instance kelas OleObjectCollection menjadi daftar yang berisi instance kelas OleObject"
type: docs
weight: 30
url: /id/net/aspose.tasks/oleobjectcollection/tolist/
---
## OleObjectCollection.ToList method

Mengonversi instance kelas [`OleObjectCollection`](../) menjadi daftar yang berisi instance kelas [`OleObject`](../../oleobject/).

```csharp
public List<OleObject> ToList()
```

### Nilai Kembali

Dikonversi menjadi daftar instance kelas [`OleObjectCollection`](../) yang berisi instance kelas [`OleObject`](../../oleobject/).

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

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


