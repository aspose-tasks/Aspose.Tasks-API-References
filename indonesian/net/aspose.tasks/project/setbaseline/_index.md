---
title: "Project.SetBaseline"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Menyimpan bidang baseline ke baseline yang ditentukan untuk seluruh proyek"
type: docs
weight: 1250
url: /id/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Menyimpan bidang baseline ke baseline yang ditentukan untuk seluruh proyek.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| baselineType | BaselineType | Tipe baseline untuk menyimpan data baseline ke. |

## Contoh

Menampilkan cara membuat baseline untuk seluruh proyek.

```csharp
var project = new Project();

// Menambahkan tugas
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// Mengatur baseline untuk tugas yang ditentukan
project.SetBaseline(BaselineType.Baseline);
```

### Lihat Juga

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Menyimpan bidang baseline ke baseline yang ditentukan untuk tugas yang dipilih.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| baselineType | BaselineType | Tipe baseline untuk menyimpan data baseline ke. |
| taskCollection | IEnumerable`1 | Daftar tugas untuk menyimpan data baseline. |

## Contoh

Menampilkan cara membuat baseline set untuk tugas tertentu.

```csharp
var project = new Project();

// Menambahkan tugas
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Mengatur baseline untuk tugas yang ditentukan
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### Lihat Juga

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


