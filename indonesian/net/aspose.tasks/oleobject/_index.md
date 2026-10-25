---
title: "Kelas OleObject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.OleObject. Mewakili objek OLE yang dapat disisipkan ke dalam Tampilan Gantt Chart dari file MPP"
type: docs
weight: 1120
url: /id/net/aspose.tasks/oleobject/
---
## OleObject class

Mewakili objek OLE yang dapat disisipkan ke dalam Tampilan Gantt Chart dari file MPP.

```csharp
public class OleObject
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [OleObject](oleobject/)() | Menginisialisasi instance baru dari kelas `OleObject`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | Mendapatkan atau mengatur nama aplikasi untuk membuka objek tersemat. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | Mendapatkan atau mengatur data file yang tersemat; null jika tidak ada data yang tersemat. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | Mendapatkan atau mengatur flag yang menunjukkan bahwa objek OLE harus ditampilkan sebagai ikon atau sebagai gambar regulernya. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | Mendapatkan atau mengatur format file dari objek tersemat. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | Mendapatkan atau mengatur jalur lengkap dari objek yang disisipkan. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | Mendapatkan atau mengatur ID objek. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | Mendapatkan atau mengatur label dari objek yang disisipkan. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | Mendapatkan nilai yang menunjukkan apakah file proyek hanya berisi tautan ke data sebenarnya yang disimpan di sumber tautan. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | Mendapatkan atau mengatur nama instance dari objek OLE. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | Mendapatkan atau mengatur jalur ke file sementara dari objek yang disisipkan. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | Mendapatkan atau mengatur instance dari kelas [`View`](./view/) yang menjadi milik objek yang disisipkan. |

## Contoh

Menampilkan cara membaca info tentang objek OLE.

```csharp
[Test]
public void WorkWithOleObject()
{
    var images = new Project(DataDir + "TaskImage2010.mpp");
    List<OleObject> oleObjects = images.OleObjects.ToList();

    Console.WriteLine("Ole Objects Count: " + oleObjects.Count);
    foreach (var oleObject in oleObjects)
    {
        Console.WriteLine(" Id: " + oleObject.Id);
        Console.WriteLine(" Name: " + oleObject.Name);
        Console.WriteLine(" DisplayAsIcon: " + oleObject.DisplayAsIcon);
        Console.WriteLine(" Application Name: " + oleObject.ApplicationName);
        Console.WriteLine(" File Format: " + oleObject.FileFormat);
        Console.WriteLine(" Label: " + oleObject.Label);
        Console.WriteLine(" Full Path: " + oleObject.FullPath);
        Console.WriteLine(" Is Linked: " + oleObject.Linked);
        Console.WriteLine(" View Name: " + oleObject.View.Name);
        Console.WriteLine(" Content (first 10 bytes): " + this.Get10Bytes(oleObject));
    }
}

private string Get10Bytes(OleObject oleObject)
{
    byte[] bytes = oleObject.Content;
    var chunk = new byte[10];
    Array.Copy(bytes, chunk, 10);
    var builder = new StringBuilder();
    foreach (var b in chunk)
    {
        builder.Append(b + ", ");
    }

    builder.Remove(builder.Length - 3, 1);
    return builder.ToString();
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


