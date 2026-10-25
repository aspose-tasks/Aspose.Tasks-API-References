---
title: "Project.GetDuration"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Mendapatkan objek Duration dengan jumlah unit yang ditentukan dan format durasi default yang didefinisikan dalam pengaturan proyek DurationFormat."
type: docs
weight: 1100
url: /id/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

Mendapatkan objek [`Duration`](../../duration/) dengan jumlah unit yang ditentukan dan format durasi default yang didefinisikan dalam pengaturan proyek [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| val | Double | jumlah unit yang ditentukan. |

### Nilai Kembali

Objek Duration.

## Catatan

Metode ini harus digunakan dengan hati-hati karena mengembalikan durasi yang berbeda tergantung pada pengaturan Project.DurationFormat. Misalnya, GetWork(1.0) akan mengembalikan 1 jam ketika Project.DurationFormat adalah TimeUnitType.Hour atau 1 hari jika Project.DurationFormat adalah TimeUnitType.Day.

## Contoh

Menampilkan cara membuat instance &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; dengan format durasi proyek default menggunakan metode fabrik proyek.

```csharp
var project = new Project();

// dapatkan durasi dengan format proyek default.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### Lihat Juga

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

Mendapatkan objek [`Duration`](../../duration/) dengan jumlah unit [`TimeUnitType`](../../timeunittype/) yang ditentukan.

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| val | Double | jumlah unit yang ditentukan. |
| timeUnit | TimeUnitType | nilai TimeUnitType yang ditentukan. |

### Nilai Kembali

Objek Duration.

## Contoh

Menampilkan cara membuat instance &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; dengan menggunakan metode fabrik proyek.

```csharp
var project = new Project();

// dapatkan durasi dengan format proyek default.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### Lihat Juga

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

Mendapatkan objek [`Duration`](../../duration/) dengan nilai TimeSpan yang ditentukan dan nilai [`TimeUnitType`](../../timeunittype/) yang ditentukan.

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| timeSpan | TimeSpan | nilai TimeSpan yang ditentukan. |
| timeUnit | TimeUnitType | nilai TimeUnitType yang ditentukan. |

### Nilai Kembali

Objek Duration.

### Lihat Juga

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


