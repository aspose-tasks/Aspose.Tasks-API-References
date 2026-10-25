---
title: "Metered.SetMeteredKey"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Metered. Mengatur kunci publik dan privat metered"
type: docs
weight: 40
url: /id/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Mengatur kunci publik dan privat metered.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| publicKey | String | Kunci publik. |
| privateKey | String | Kunci pribadi. |

## Catatan

Jika Anda membeli lisensi terukur, API ini harus dipanggil saat aplikasi dimulai, biasanya ini sudah cukup. Namun, jika terukur gagal mengunggah data konsumsi selama periode 24 jam, lisensi akan diatur ke status evaluasi. Untuk menghindari kasus tersebut, Anda harus secara teratur memeriksa status lisensi. Jika statusnya evaluasi, panggil API ini lagi.

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


