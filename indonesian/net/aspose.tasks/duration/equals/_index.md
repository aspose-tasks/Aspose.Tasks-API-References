---
title: "Duration.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Duration. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan"
type: docs
weight: 80
url: /id/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public bool Equals(Duration other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lain | Durasi | Objek untuk dibandingkan dengan instance ini. |

### Nilai Kembali

Mengembalikan **True** jika instance Duration lain memiliki nilai TimeSpan dan TimeUnit yang sama dengan instance ini; jika tidak, **false**.

## Contoh

Menampilkan cara memeriksa kesetaraan durasi.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// kesetaraan durasi diperiksa terhadap timespan yang mendasarinya
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | Objek untuk dibandingkan dengan instance ini. |

### Nilai Kembali

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

## Contoh

Menampilkan cara memeriksa kesetaraan durasi.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// kesetaraan durasi diperiksa terhadap timespan yang mendasarinya
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


