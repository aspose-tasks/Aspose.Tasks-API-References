---
title: GetPageCount
second_title: Aspose.Tasks voor .NET API-referentie
description: Retourneert het aantal paginas voor het project dat moet worden weergegeven met behulp van gegevenSaveOptionsaspose.tasks.saving/saveoptions/ .
type: docs
weight: 1080
url: /nl/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Retourneert het aantal pagina's voor het project dat moet worden weergegeven met behulp van gegeven[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| saveOptions | SaveOptions | De opslagopties om het aantal pagina's voor te krijgen. |

### Winstwaarde

een aantal pagina's dat moet worden weergegeven.

### Voorbeelden

In dit voorbeeld van HtmlSaveOptions wordt het aantal pagina's in resulterende HTML naar de console geschreven.

```csharp
[C#]
Project project = new Project(@"test.mpp");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
    IncludeProjectNameInPageHeader = false,
    IncludeProjectNameInTitle = false,
    PageSize = PageSize.A4,
    Timescale = Timescale.Days,
    StartDate = project.Get(Prj.StartDate).Date,
    EndDate = project.Get(Prj.FinishDate).Date
};

Console.WriteLine(project.GetPageCount(saveOptions));
```

### Zie ook

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* naamruimte [Aspose.Tasks](../../project/)
* montage [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Retourneert het aantal pagina's voor het project dat moet worden weergegeven met standaard[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Dagen).

```csharp
public int GetPageCount()
```

### Winstwaarde

Aantal pagina's dat moet worden weergegeven.

### Zie ook

* class [Project](../)
* naamruimte [Aspose.Tasks](../../project/)
* montage [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Retourneert het aantal pagina's voor het project dat moet worden weergegeven met behulp van gegeven[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| scale | Timescale | De schaal om het aantal pagina's voor te krijgen. |

### Winstwaarde

Aantal pagina's dat moet worden weergegeven.

### Zie ook

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* naamruimte [Aspose.Tasks](../../project/)
* montage [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Retourneert het aantal pagina's voor het project dat moet worden weergegeven met standaard[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Dagen) en gegeven[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| format | PresentationFormat | Het formaat om het aantal pagina's voor te krijgen. |

### Winstwaarde

Aantal pagina's dat moet worden weergegeven.

### Zie ook

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* naamruimte [Aspose.Tasks](../../project/)
* montage [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Retourneert het aantal pagina's voor het project dat moet worden weergegeven met behulp van gegeven[`Timescale`](../../../aspose.tasks.visualization/timescale/) En[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| format | PresentationFormat | Het formaat om het aantal pagina's voor te krijgen. |
| scale | Timescale | De schaal om het aantal pagina's voor te krijgen. |

### Winstwaarde

een aantal pagina's dat moet worden weergegeven.

### Zie ook

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* naamruimte [Aspose.Tasks](../../project/)
* montage [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Retourneert het aantal pagina's voor het project dat moet worden weergegeven met behulp van gegeven[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) en datumbereik.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageSize | PageSize | Het formaat waarvoor het aantal pagina's moet worden opgehaald. |
| scale | Timescale | De schaal om het aantal pagina's voor te krijgen. |
| startDate | DateTime | De begindatum waarvoor het aantal pagina's moet worden opgehaald. |
| endDate | DateTime | De einddatum waarvoor het aantal pagina's moet worden opgehaald. |

### Winstwaarde

Aantal pagina's dat moet worden weergegeven.

### Zie ook

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* naamruimte [Aspose.Tasks](../../project/)
* montage [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Retourneert het aantal pagina's voor het project dat moet worden weergegeven met behulp van gegeven[`Timescale`](../../../aspose.tasks.visualization/timescale/) En[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageSize | PageSize | Het formaat waarvoor het aantal pagina's moet worden opgehaald. |
| scale | Timescale | De schaal om het aantal pagina's voor te krijgen. |

### Winstwaarde

Aantal pagina's dat moet worden weergegeven.

### Zie ook

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* naamruimte [Aspose.Tasks](../../project/)
* montage [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
