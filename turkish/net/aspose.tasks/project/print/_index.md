---
title: "Project.Print"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Standart kullanıcı arayüzü olmayan yazdırma denetleyicisini kullanarak varsayılan yazıcı ayarlarıyla projeyi varsayılan yazıcıya yazdırır"
type: docs
weight: 1140
url: /tr/net/aspose.tasks/project/print/
---
## Print() {#print}

Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin varsayılan yazıcıya, varsayılan yazıcı ayarlarıyla yazdırır.

```csharp
public void Print()
```

## Örnekler

Bir projeyi nasıl yazdıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin varsayılan yazıcıya, varsayılan yazıcı ayarları ve özel kaydetme seçenekleriyle yazdırır.

```csharp
public void Print(PrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | PrintOptions | belirtilen [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) sınıfının örneği. |

## Örnekler

Yazdırma seçeneklerini kullanarak bir projeyi nasıl yazdıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.ThirdsOfMonths
};
if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
{
    project.Print(options);
}
```

### Ayrıca Bakınız

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcıya, varsayılan yazıcı ayarlarıyla yazdırır.

```csharp
public void Print(string printerName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | Dize | Belirtilen yazıcı adı. |

## Örnekler

Seçilen yazıcıda projeyi nasıl yazdıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

foreach (string printer in PrinterSettings.InstalledPrinters)
{
    if (!printer.ToUpperInvariant().Contains("Microsoft Print to PDF".ToUpperInvariant()))
    {
        continue;
    }

    project.Print(printer);
    break;
}
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcı ayarlarına göre yazdırır.

```csharp
public void Print(PrinterSettings printerSettings)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerSettings | PrinterSettings | PrinterSettings sınıfının belirtilen örneği. |

## Örnekler

Yazıcı ayarlarını kullanarak projeyi nasıl yazdıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// İlk iki sayfayı yazdır
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcı ayarlarına göre yazdırır.

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerSettings | PrinterSettings | PrinterSettings sınıfının belirtilen örneği. |
| documentName | Dize | gösterilecek belge adı (örneğin, bir yazdırma durumu ileti kutusunda veya yazıcı kuyruğunda). |

## Örnekler

Yazıcı ayarlarını ve bir belge adını kullanarak projeyi nasıl yazdıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// İlk iki sayfayı yazdır
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcı ayarları ve özel kaydetme seçeneklerine göre yazdırır.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerSettings | PrinterSettings | PrinterSettings sınıfının belirtilen örneği. |
| options | PrintOptions | belirtilen [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) sınıfının örneği. |

## Örnekler

Yazıcı seçeneklerini ve ayarlarını kullanarak projeyi nasıl yazdıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// İlk iki sayfayı yazdır
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### Ayrıca Bakınız

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcı ayarları, özel kaydetme seçenekleri ve belirtilen belge adıyla yazdırır.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerSettings | PrinterSettings | PrinterSettings sınıfının belirtilen örneği. |
| options | PrintOptions | belirtilen [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) sınıfının örneği. |
| documentName | Dize | gösterilecek belge adı (örneğin, bir yazdırma durumu ileti kutusunda veya yazıcı kuyruğunda). |

## Örnekler

Yazıcı seçeneklerini, yazıcı ayarlarını ve belge adını kullanarak projeyi nasıl yazdıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// İlk iki sayfayı yazdır
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### Ayrıca Bakınız

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


