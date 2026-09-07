---
title: "MspDbSettings.MspDbSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor MspDbSettings. Menginisialisasi sebuah instance baru dari kelas MspDbSettings"
type: docs
weight: 10
url: /id/net/aspose.tasks.connectivity/mspdbsettings/mspdbsettings/
---
## MspDbSettings constructor

Menginisialisasi sebuah instance baru dari kelas [`MspDbSettings`](../).

```csharp
public MspDbSettings(string connectionString, Guid projectGuid)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| connectionString | String | string koneksi yang ditentukan. |
| projectGuid | Guid | guid yang ditentukan dari proyek yang akan dibaca. |

## Contoh

Menampilkan cara mengimpor proyek dari basis data.

```csharp
try
{
    // Buat string koneksi
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // buat pengaturan untuk memuat dari basis data MS
    var settings = new MspDbSettings(connectionString.ConnectionString, new Guid("E6426C44-D6CB-4B9C-AF16-48910ACE0F54"));
    settings.Schema = "dbo";

    Console.WriteLine("Project GUID to load: " + settings.ProjectGuid);

    var project = new Project(settings);

    project.Save(OutDir + "ImportProjectDataFromDatabase_out.mpp", SaveFileFormat.Mpp);
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message + " Please setup proper data source (DataSource, InitialCatalog etc)");
}
```

### Lihat Juga

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


