---
title: GetPageCount
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Restituisce il conteggio delle pagine per il progetto da renderizzare usando datoSaveOptionsaspose.tasks.saving/saveoptions .
type: docs
weight: 300
url: /it/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`SaveOptions`](../../../aspose.tasks.saving/saveoptions) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveOptions | SaveOptions | Le opzioni di salvataggio per il conteggio delle pagine. |

### Valore di ritorno

un conteggio delle pagine da visualizzare.

### Esempi

In questo esempio, l'istanza di HtmlSaveOptions e il numero di pagine nell'HTML risultante vengono scritti nella console.

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

### Guarda anche

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions)
* class [Project](../../project)
* spazio dei nomi [Aspose.Tasks](../../project)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando l'impostazione predefinita[`Timescale`](../../../aspose.tasks.visualization/timescale) (Giorni).

```csharp
public int GetPageCount()
```

### Valore di ritorno

Conteggio pagine da visualizzare.

### Guarda anche

* class [Project](../../project)
* spazio dei nomi [Aspose.Tasks](../../project)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`Timescale`](../../../aspose.tasks.visualization/timescale) .

```csharp
public int GetPageCount(Timescale scale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| scale | Timescale | La scala per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Conteggio pagine da visualizzare.

### Guarda anche

* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* spazio dei nomi [Aspose.Tasks](../../project)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando l'impostazione predefinita[`Timescale`](../../../aspose.tasks.visualization/timescale) (Giorni) e dato[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | PresentationFormat | Il formato per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Conteggio pagine da visualizzare.

### Guarda anche

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat)
* class [Project](../../project)
* spazio dei nomi [Aspose.Tasks](../../project)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`Timescale`](../../../aspose.tasks.visualization/timescale) e[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | PresentationFormat | Il formato per cui ottenere il conteggio delle pagine. |
| scale | Timescale | La scala per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

un conteggio delle pagine da visualizzare.

### Guarda anche

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* spazio dei nomi [Aspose.Tasks](../../project)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`Timescale`](../../../aspose.tasks.visualization/timescale) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat) e intervallo di date.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageSize | PageSize | La dimensione per cui ottenere il conteggio delle pagine. |
| scale | Timescale | La scala per cui ottenere il conteggio delle pagine. |
| startDate | DateTime | La data di inizio per cui ottenere il conteggio delle pagine. |
| endDate | DateTime | La data di fine per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Conteggio pagine da visualizzare.

### Guarda anche

* enum [PageSize](../../../aspose.tasks.visualization/pagesize)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* spazio dei nomi [Aspose.Tasks](../../project)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`Timescale`](../../../aspose.tasks.visualization/timescale) e[`PageSize`](../../../aspose.tasks.visualization/pagesize) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageSize | PageSize | La dimensione per cui ottenere il conteggio delle pagine. |
| scale | Timescale | La scala per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Conteggio pagine da visualizzare.

### Guarda anche

* enum [PageSize](../../../aspose.tasks.visualization/pagesize)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* spazio dei nomi [Aspose.Tasks](../../project)
* assemblea [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
