---
title: Project.GetPageCount
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Project metodo. Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando givenSaveOptions .
type: docs
weight: 1080
url: /it/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando given[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveOptions | SaveOptions | Le opzioni di salvataggio per ottenere il conteggio delle pagine. |

### Valore di ritorno

un conteggio delle pagine da rendere.

### Esempi

In questa istanza di esempio di HtmlSaveOptions e il numero di pagine nell'HTML risultante viene scritto nella console.

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

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando l'impostazione predefinita[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Giorni).

```csharp
public int GetPageCount()
```

### Valore di ritorno

Numero di pagine da visualizzare.

### Guarda anche

* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando given[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| scale | Timescale | La scala per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Numero di pagine da visualizzare.

### Guarda anche

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando l'impostazione predefinita[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Giorni) e dato[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | PresentationFormat | Il formato per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Numero di pagine da visualizzare.

### Guarda anche

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando given[`Timescale`](../../../aspose.tasks.visualization/timescale/) E[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | PresentationFormat | Il formato per cui ottenere il conteggio delle pagine. |
| scale | Timescale | La scala per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

un conteggio delle pagine da rendere.

### Guarda anche

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando given[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) e intervallo di date.

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

Numero di pagine da visualizzare.

### Guarda anche

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando given[`Timescale`](../../../aspose.tasks.visualization/timescale/) E[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageSize | PageSize | La dimensione per cui ottenere il conteggio delle pagine. |
| scale | Timescale | La scala per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Numero di pagine da visualizzare.

### Guarda anche

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)


