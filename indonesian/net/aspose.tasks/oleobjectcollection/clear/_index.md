---
title: "OleObjectCollection.Clear"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode OleObjectCollection. Mengosongkan koleksi. Untuk mempertahankan perubahan ini, project.Save harus dipanggil dengan MPPSaveOptions baru  WriteViewData  true"
type: docs
weight: 10
url: /id/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Menghapus koleksi. Untuk mempertahankan perubahan ini, project.Save harus dipanggil dengan MPPSaveOptions baru { WriteViewData = true; }

```csharp
public void Clear()
```

## Contoh

Cara menghapus objek OLE dan mempertahankan perubahan ini.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

Menampilkan cara menghapus objek OLE dari proyek yang ditentukan.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### Lihat Juga

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


