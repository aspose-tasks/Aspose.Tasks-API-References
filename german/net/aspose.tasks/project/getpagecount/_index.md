---
title: Project.GetPageCount
second_title: Aspose.Tasks für .NET-API-Referenz
description: Project methode. Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurückSaveOptions .
type: docs
weight: 1080
url: /de/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveOptions | SaveOptions | Die Speicheroptionen, für die die Seitenanzahl abgerufen werden soll. |

### Rückgabewert

eine Seitenzahl, die gerendert werden soll.

### Beispiele

In diesem Beispiel wird eine Instanz von HtmlSaveOptions und die Anzahl der Seiten im resultierenden HTML in die Konsole geschrieben.

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

### Siehe auch

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namensraum [Aspose.Tasks](../../project/)
* Montage [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Gibt die Seitenzahl für das zu rendernde Projekt zurück, wobei der Standardwert verwendet wird[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Tage).

```csharp
public int GetPageCount()
```

### Rückgabewert

Anzahl der zu rendernden Seiten.

### Siehe auch

* class [Project](../)
* namensraum [Aspose.Tasks](../../project/)
* Montage [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| scale | Timescale | Die Skala, für die die Seitenanzahl abgerufen werden soll. |

### Rückgabewert

Anzahl der zu rendernden Seiten.

### Siehe auch

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namensraum [Aspose.Tasks](../../project/)
* Montage [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Gibt die Seitenzahl für das zu rendernde Projekt zurück, wobei der Standardwert verwendet wird[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Tage) und gegeben[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| format | PresentationFormat | Das Format, für das die Seitenzahl abgerufen werden soll. |

### Rückgabewert

Anzahl der zu rendernden Seiten.

### Siehe auch

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namensraum [Aspose.Tasks](../../project/)
* Montage [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`Timescale`](../../../aspose.tasks.visualization/timescale/) Und[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| format | PresentationFormat | Das Format, für das die Seitenzahl abgerufen werden soll. |
| scale | Timescale | Die Skala, für die die Seitenanzahl abgerufen werden soll. |

### Rückgabewert

eine Seitenzahl, die gerendert werden soll.

### Siehe auch

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namensraum [Aspose.Tasks](../../project/)
* Montage [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) und Datumsbereich.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageSize | PageSize | Die Größe, für die die Seitenzahl abgerufen werden soll. |
| scale | Timescale | Die Skala, für die die Seitenanzahl abgerufen werden soll. |
| startDate | DateTime | Das Startdatum, für das die Seitenzahl abgerufen werden soll. |
| endDate | DateTime | Das Enddatum, für das die Seitenanzahl abgerufen werden soll. |

### Rückgabewert

Anzahl der zu rendernden Seiten.

### Siehe auch

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namensraum [Aspose.Tasks](../../project/)
* Montage [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`Timescale`](../../../aspose.tasks.visualization/timescale/) Und[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageSize | PageSize | Die Größe, für die die Seitenzahl abgerufen werden soll. |
| scale | Timescale | Die Skala, für die die Seitenanzahl abgerufen werden soll. |

### Rückgabewert

Anzahl der zu rendernden Seiten.

### Siehe auch

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namensraum [Aspose.Tasks](../../project/)
* Montage [Aspose.Tasks](../../../)


