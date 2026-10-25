---
title: "Metered.GetConsumptionCredit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Metered. Mendapatkan kredit konsumsi"
type: docs
weight: 50
url: /id/net/aspose.tasks/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

Mendapatkan kredit konsumsi.

```csharp
public static decimal GetConsumptionCredit()
```

### Nilai Kembali

Mengembalikan jumlah poin kredit yang dikonsumsi.

## Contoh

Menampilkan cara menggunakan &lt;see cref="Aspose.Tasks.Metered" /&gt; tipe lisensi dengan Aspose.Tasks.

```csharp
// Mari gunakan lisensi metered (lihat https://purchase.aspose.com/faqs/licensing/metered)
// atur lisensi metered
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// bekerja dengan proyek...
// ...

// Kita dapat memperoleh kredit saat ini dan konsumsi byte.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // catat pengecualian
}

// baru-baru ini pengguna dapat mereset metered dan menghentikan penghitungan byte
metered.ResetMeteredKey();
```

### Lihat Juga

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


