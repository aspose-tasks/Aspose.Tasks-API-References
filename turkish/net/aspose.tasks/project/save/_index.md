---
title: "Project.Save"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Belirtilen kaydetme seçeneklerini kullanarak belgeyi bir dosyaya kaydeder"
type: docs
weight: 1200
url: /tr/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

Belirtilen kaydetme seçeneklerini kullanarak belgeyi dosyaya kaydeder.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | Dize | Dosya adı. |
| seçenekler | SimpleSaveOptions | Kaydetme seçenekleri. |

## Örnekler

Projeyi MPP dosyası olarak nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### Ayrıca Bakınız

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

Proje verilerini dosyaya kaydeder.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | Dize | Dosya adı. |
| biçim | SaveFileFormat | Kaydetme dosya biçimi. |

## Örnekler

Bir proje oluşturmanın ve MPP şablon dosyası geçirmeden MPP formatında kaydetmenin nasıl yapılacağını gösterir.

```csharp
var project = new Project();

// Proje, dahili MPP şablonu kullanılarak MPP olarak kaydedilecektir.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

Proje verilerini mpp formatında dosyaya kaydeder.

```csharp
public void Save(string filename)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | Dize | Dosya adı. |

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

Belirtilen kaydetme seçeneklerini kullanarak projeyi akışa kaydeder.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Akış. |
| seçenekler | SimpleSaveOptions | Kaydetme seçenekleri. |

## Örnekler

MPP kaydetme seçeneklerini kullanarak projeyi bir akışa MPP dosyası olarak nasıl kaydedeceğinizi gösterir.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // MPPSaveOptions kullanarak onu MPP biçiminde kaydediyoruz
    project.Save(stream, options);
}
```

Projeyi bir akışa görüntü olarak ve görüntü seçeneklerini kontrol ederek nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // ImageSaveOptions kullanarak projeyi görüntü formatında kaydederiz
    project.Save(stream, options);
}
```

### Ayrıca Bakınız

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

Proje verilerini akışa kaydeder.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Akış. |
| format | SaveFileFormat | belirtilen kaydetme dosya biçimi.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## Örnekler

Projeyi bir akışa XML MS Project dosyası olarak nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // Akışı XML biçimine yaz
    project.Save(stream, SaveFileFormat.Xml);
}
```

### Ayrıca Bakınız

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


