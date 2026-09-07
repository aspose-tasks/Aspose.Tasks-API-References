---
title: "Project.CopyTo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Menyalin data utama proyek dan properti ke proyek lain"
type: docs
weight: 1060
url: /id/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

Menyalin data utama dan properti proyek ke proyek lain.

```csharp
public void CopyTo(Project another)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lain | Project | Proyek lain untuk menyalin data ke. |

## Contoh

Menampilkan cara menyalin data proyek ke proyek lain.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// lewati penyalinan data tampilan saat menyalin data proyek umum.
project.CopyTo(mppProject);
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

Menyalin data utama dan properti proyek ke proyek lain.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lain | Project | Proyek lain untuk menyalin data ke. |
| opsi | CopyToOptions | Opsi penyalinan untuk mengendalikan proses penyalinan. |

## Contoh

Menampilkan cara menyalin proyek dengan menggunakan instance &lt;see cref="Aspose.Tasks.CopyToOptions"/&gt;.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// lewati penyalinan data tampilan saat menyalin data proyek umum.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### Lihat Juga

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


