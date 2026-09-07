---
title: "Project.Save"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Project method. Menyimpan dokumen ke file menggunakan opsi penyimpanan yang ditentukan"
type: docs
weight: 1200
url: /id/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

Menyimpan dokumen ke file menggunakan opsi penyimpanan yang ditentukan.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama file | String | Nama file. |
| opsi | SimpleSaveOptions | Opsi penyimpanan. |

## Contoh

Menampilkan cara menyimpan proyek sebagai file MPP.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### Lihat Juga

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

Menyimpan data proyek ke file.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama file | String | Nama file. |
| format | SaveFileFormat | Format file penyimpanan. |

## Contoh

Menampilkan cara membuat proyek dan menyimpannya dalam format MPP tanpa menggunakan file templat MPP.

```csharp
var project = new Project();

// Proyek akan disimpan ke dalam MPP dengan menggunakan templat MPP internal.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

Menyimpan data proyek ke file dalam format mpp.

```csharp
public void Save(string filename)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama file | String | Nama file. |

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

Menyimpan proyek ke aliran menggunakan opsi penyimpanan yang ditentukan.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran. |
| opsi | SimpleSaveOptions | Opsi penyimpanan. |

## Contoh

Menampilkan cara menyimpan proyek ke dalam stream sebagai file MPP dengan menggunakan opsi penyimpanan MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // Dengan menggunakan MPPSaveOptions kami menyimpannya dalam format MPP
    project.Save(stream, options);
}
```

Menampilkan cara menyimpan proyek ke dalam stream sebagai gambar dan mengontrol opsi gambar.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // dengan menggunakan ImageSaveOptions kami menyimpan proyek ke dalam format gambar
    project.Save(stream, options);
}
```

### Lihat Juga

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

Menyimpan data proyek ke aliran.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran. |
| format | SaveFileFormat | format file penyimpanan yang ditentukan.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## Contoh

Menampilkan cara menyimpan proyek ke dalam stream sebagai file XML MS Project.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // Tulis stream ke dalam format XML
    project.Save(stream, SaveFileFormat.Xml);
}
```

### Lihat Juga

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


