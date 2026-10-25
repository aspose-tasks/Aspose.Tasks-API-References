---
title: "Kelas MspDbSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Connectivity.MspDbSettings. Memungkinkan mengatur opsi yang diperlukan untuk membaca data proyek dari basis data MS Project Server"
type: docs
weight: 310
url: /id/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

Mengizinkan untuk mengatur opsi yang diperlukan untuk membaca data proyek dari basis data MS Project Server.

```csharp
public class MspDbSettings : DbSettings
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | Menginisialisasi instance baru dari kelas `MspDbSettings`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Mendapatkan atau mengatur string koneksi. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | Mendapatkan GUID proyek yang akan dibaca. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Mendapatkan atau mengatur callback yang akan dipanggil selama operasi pemuatan proyek. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Mendapatkan atau mengatur instance DbProviderFactory yang digunakan untuk terhubung ke DB. Jika kedua ProviderFactory dan ProviderInvariantName diatur, ProviderFactory memiliki prioritas. Nilai default adalah null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Mendapatkan atau mengatur nama invarian penyedia yang digunakan untuk mendapatkan instance kelas DbProviderFactory. Nilai default adalah SqlClient. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | Mendapatkan atau mengatur skema MS Project Server. Nilai default adalah \"pub\". |

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

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


