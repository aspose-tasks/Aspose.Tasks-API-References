---
title: "Project.OleObjects"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan koleksi yang berisi instance kelas OleObject yang ditautkan atau disematkan ke file proyek ini. Hanya tersedia untuk format file mpp. Koleksi ini hanya-baca kecuali untuk operasi Clear."
type: docs
weight: 700
url: /id/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

Mendapatkan koleksi yang berisi instance dari kelas [`OleObject`](../../oleobject/) yang ditautkan atau disematkan ke file proyek ini. Hanya tersedia untuk format file mpp. Koleksi ini hanya-baca kecuali untuk operasi 'Clear'.

```csharp
public OleObjectCollection OleObjects { get; }
```

## Contoh

Menampilkan cara mengekstrak objek OLE yang disematkan.

```csharp
IDictionary<string, string> formatExt = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !formatExt.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + formatExt[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### Lihat Juga

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


