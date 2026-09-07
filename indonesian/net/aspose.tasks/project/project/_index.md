---
title: "Project.Project"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor Project. Menginisialisasi instance baru dari kelas Project."
type: docs
weight: 10
url: /id/net/aspose.tasks/project/project/
---
## Project() {#constructor}

Menginisialisasi instance baru dari kelas [`Project`](../).

```csharp
public Project()
```

## Contoh

Menampilkan cara membuat proyek dan menyimpannya dalam format MPP tanpa menggunakan file templat MPP.

```csharp
var project = new Project();

// Proyek akan disimpan ke dalam MPP dengan menggunakan templat MPP internal.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

Menginisialisasi instance baru dari kelas [`Project`](../) dari templat yang dilindungi kata sandi (file mpp atau mpt yang ada).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | String | Jalur ke templat untuk membuat proyek. |
| protectionPassword | String | Kata sandi perlindungan. |

## Catatan

Membaca file yang dilindungi kata sandi saat ini hanya didukung untuk format file MSP 2003.

## Contoh

Menampilkan cara membaca file MPP yang dilindungi kata sandi.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

Menginisialisasi instance baru dari kelas [`Project`](../) dari templat (file mpp atau mpt yang ada).

```csharp
public Project(string projectTemplate)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | String | Jalur ke templat untuk membuat proyek. |

## Contoh

Menampilkan cara membaca file MPP.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

Menginisialisasi instance baru dari kelas [`Project`](../) dari Stream dengan instance yang ditentukan dari kelas [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran dari Project Streamclass |
| options | PrimaveraReadOptions | instance yang ditentukan dari [`PrimaveraReadOptions`](../../primaverareadoptions/) class yang memungkinkan untuk menyesuaikan pembacaan format Primavera (XER atau XML). |

## Contoh

Menampilkan cara membaca proyek dari aliran dengan file Primavera XML atau Primavera XER yang berisi beberapa proyek.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // Mengembalikan proyek dengan UID khusus
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Lihat Juga

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

Menginisialisasi instance baru dari kelas [`Project`](../) dari templat (file mpp atau mpt yang ada).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | String | Jalur ke templat untuk membuat proyek. |
| parseErrorHandler | ParseErrorCallback | metode callback yang ditentukan untuk menangani kesalahan parsing xml. |

## Contoh

Menampilkan cara membaca proyek dari aliran dengan file XML yang berisi karakter tidak valid.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // buka file yang berisi XML dengan rentang waktu yang rusak
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### Lihat Juga

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

Menginisialisasi instance baru dari [`Project`](../) class dari aliran.

```csharp
public Project(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran untuk memuat templat dari. |

## Contoh

Menampilkan cara membaca file proyek XML dari aliran.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

Menginisialisasi instance baru dari [`Project`](../) class dari instance StreamReader.

```csharp
public Project(StreamReader reader)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pembaca | StreamReader | Pembaca aliran tempat memuat templat dari. |

## Contoh

Menampilkan cara membaca file MPX dengan enkoding tertentu.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

Menginisialisasi instance baru dari [`Project`](../) class dari templat (file MPP atau MPT yang ada) dengan instance yang ditentukan dari [`PrimaveraReadOptions`](../../primaverareadoptions/) class.

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | String | Jalur ke templat untuk membuat proyek dari |
| options | PrimaveraReadOptions | instance yang ditentukan dari [`PrimaveraReadOptions`](../../primaverareadoptions/) class. |

## Contoh

Menampilkan cara membaca proyek dari file Primavera XML atau Primavera XER yang berisi beberapa proyek dengan menggunakan opsi pembacaan Primavera.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// Mengembalikan proyek dengan UID khusus
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Lihat Juga

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

Menginisialisasi instance baru dari [`Project`](../) class untuk membaca data dari basis data yang ditentukan oleh instance kelas [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/).

```csharp
public Project(DbSettings settings)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| settings | DbSettings | instance yang ditentukan dari [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) class. |

## Contoh

Menampilkan cara mengimpor proyek dari basis data Primavera dengan menggunakan pengaturan basis data.

```csharp
var sb = new SqlConnectionStringBuilder
{
    DataSource = "192.168.56.3,1433",
    Encrypt = true,
    TrustServerCertificate = true,
    InitialCatalog = "PrimaveraEDB",
    NetworkLibrary = "DBMSSOCN",
    UserID = "privuser",
    Password = "***",
};

// Inisialisasi instance baru dari kelas PrimaveraDbSettings dengan string koneksi dan ID proyek
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Inisialisasi instance baru dari kelas Project
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Lihat Juga

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

Menginisialisasi instance baru dari [`Project`](../) class dari templat (file mpp atau mpt yang ada).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran untuk memuat templat dari. |
| parseErrorHandler | ParseErrorCallback | metode callback yang ditentukan untuk menangani kesalahan parsing xml. |

## Contoh

Menampilkan cara membaca proyek dari file XML dengan karakter tidak valid.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // buka aliran yang berisi XML dengan rentang waktu yang rusak
    byte[] bytes = Encoding.UTF8.GetBytes(brokenXmlData);
    using (var stream = new MemoryStream(bytes))
    {
        var project = new Project(stream, CustomDurationHandlerForStream2);
        Console.WriteLine(project.Get(Prj.Name));
    }
}

public static object CustomDurationHandlerForStream2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Debug.Print("Object field : {0}, Invalid value : {1}", args.FieldName, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Debug.Print("New value : {0}", newValue);
    return newValue;
}
```

### Lihat Juga

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

Menginisialisasi instance baru dari [`Project`](../) class dari templat (file mpp atau mpt yang ada).

```csharp
public Project(Stream stream, string protectionPassword)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran untuk memuat templat dari. |
| protectionPassword | String | Kata sandi perlindungan. |

## Catatan

Membaca file yang dilindungi kata sandi saat ini hanya didukung untuk format file MSP 2003.

## Contoh

Menampilkan cara memeriksa apakah MPP dilindungi kata sandi.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

Menampilkan cara membaca file MPP yang dilindungi kata sandi dari aliran.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

Menginisialisasi instance baru dari kelas [`Project`](../) dari templat (file mpp atau mpt yang ada) dengan instance yang ditentukan dari kelas [`LoadOptions`](../../loadoptions/).

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | String | Jalur ke templat untuk membuat proyek dari |
| options | LoadOptions | instance yang ditentukan dari kelas [`LoadOptions`](../../loadoptions/). |

## Contoh

Menampilkan cara memuat proyek dari file dengan menggunakan &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; instance.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

Menampilkan cara membaca proyek dari file XML Primavera dengan kesalahan parsing.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// Mengembalikan proyek dengan UID khusus
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### Lihat Juga

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

Menginisialisasi instance baru dari kelas [`Project`](../) dari Stream dengan instance yang ditentukan dari kelas [`LoadOptions`](../../loadoptions/).

```csharp
public Project(Stream stream, LoadOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran dari Project Streamclass |
| options | LoadOptions | instance yang ditentukan dari kelas [`LoadOptions`](../../loadoptions/)class |

## Contoh

Menampilkan cara memuat proyek dari aliran dengan menggunakan &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; instance.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Lihat Juga

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


