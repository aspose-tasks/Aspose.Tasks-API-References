---
title: "OleObjectCollection.GetEnumerator"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode OleObjectCollection. Mengembalikan enumerator untuk koleksi ini"
type: docs
weight: 20
url: /id/net/aspose.tasks/oleobjectcollection/getenumerator/
---
## OleObjectCollection.GetEnumerator method

Mengembalikan enumerator untuk koleksi ini.

```csharp
public IEnumerator<OleObject> GetEnumerator()
```

### Nilai Kembali

enumerator untuk koleksi ini.

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


