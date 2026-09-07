---
title: "License.SetLicense"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode License. Memberi lisensi pada komponen."
type: docs
weight: 20
url: /id/net/aspose.tasks/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Melisensikan komponen.

```csharp
public void SetLicense(string licenseName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| licenseName | String | Dapat berupa nama file lengkap atau pendek atau nama sumber daya yang disematkan. Gunakan string kosong untuk beralih ke mode evaluasi. |

## Catatan

Mencoba menemukan lisensi di lokasi berikut:

1. Jalur eksplisit.

2. Folder yang berisi assembly komponen Aspose.

3. Folder yang berisi assembly pemanggil klien.

4. Folder yang berisi assembly entri (startup).

5. Sumber daya yang disematkan dalam assembly pemanggil klien.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Jalur eksplisit.

2. Sumber daya yang disematkan dalam assembly pemanggil klien.

2. Folder yang berisi file JAR komponen Aspose.

3. Folder yang berisi file JAR pemanggil klien.

## Contoh

Dalam contoh ini, akan dilakukan upaya untuk menemukan file lisensi bernama MyLicense.lic di folder yang berisi komponen, di folder yang berisi assembly pemanggil, di folder assembly entri, dan kemudian di sumber daya tersemat dari assembly pemanggil.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

file jar komponen:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Menampilkan cara menerapkan lisensi Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Lihat Juga

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)

---

## SetLicense(Stream) {#setlicense}

Melisensikan komponen.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Stream yang berisi lisensi. |

## Catatan

Gunakan metode ini untuk memuat lisensi dari stream.

## Contoh

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

Menunjukkan cara menerapkan lisensi Aspose.Tasks yang dibaca dari &lt;see cref="System.IO.FileStream" /&gt;.

```csharp
var license = new License();
using (var stream = new FileStream("Aspose.Tasks.lic", FileMode.Open))
{
    license.SetLicense(stream);
}
```

### Lihat Juga

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


