---
title: "Project.GetPageCount"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Project. Devuelve el recuento de páginas del proyecto que se renderizará usando los SaveOptions proporcionados."
type: docs
weight: 1110
url: /es/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Devuelve el recuento de páginas del proyecto que se renderizará usando los [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveOptions | SaveOptions | Las opciones de guardado para obtener el recuento de páginas. |

### Valor devuelto

un recuento de páginas a renderizar.

## Ejemplos

En este ejemplo, la instancia de HtmlSaveOptions y el número de páginas en el HTML resultante se escribe en la consola.

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

Muestra cómo obtener el recuento de páginas para opciones de guardado específicas.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var options = new HtmlSaveOptions
                  {
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A4,
                      Timescale = Timescale.Days,
                      StartDate = project.Get(Prj.StartDate).Date,
                      EndDate = project.Get(Prj.FinishDate).Date
                  };

Console.WriteLine(project.GetPageCount(options));
```

### Ver también

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Devuelve el recuento de páginas para el proyecto que se renderizará usando el [`Timescale`](../../../aspose.tasks.visualization/timescale/) predeterminado (Días).

```csharp
public int GetPageCount()
```

### Valor devuelto

Recuento de páginas a renderizar.

## Ejemplos

Muestra cómo obtener el recuento de páginas para diferentes escalas de tiempo.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Obtener número de páginas, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Devuelve el recuento de páginas para el proyecto que se renderizará usando el [`Timescale`](../../../aspose.tasks.visualization/timescale/) proporcionado.

```csharp
public int GetPageCount(Timescale scale)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| escala | Timescale | La escala para la que se obtendrá el recuento de páginas. |

### Valor devuelto

Recuento de páginas a renderizar.

## Ejemplos

Muestra cómo obtener el recuento de páginas para diferentes escalas de tiempo.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Obtener número de páginas, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Ver también

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Devuelve el recuento de páginas para el proyecto que se renderizará usando el [`Timescale`](../../../aspose.tasks.visualization/timescale/) predeterminado (Días) y el [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) proporcionado.

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formato | PresentationFormat | El formato para el que se obtendrá el recuento de páginas. |

### Valor devuelto

Recuento de páginas a renderizar.

## Ejemplos

Muestra cómo obtener el recuento de páginas por formato de presentación y escala de tiempo.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Obtener número de páginas para Días (por defecto), Meses y ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Ver también

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Devuelve el recuento de páginas para el proyecto que se renderizará usando el [`Timescale`](../../../aspose.tasks.visualization/timescale/) y el [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) proporcionados.

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formato | PresentationFormat | El formato para el que se obtendrá el recuento de páginas. |
| escala | Timescale | La escala para la que se obtendrá el recuento de páginas. |

### Valor devuelto

un recuento de páginas a renderizar.

## Ejemplos

Muestra cómo obtener el recuento de páginas por formato de presentación y escala de tiempo.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Obtener número de páginas para Días (por defecto), Meses y ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Ver también

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Devuelve el recuento de páginas para el proyecto que se renderizará usando el [`Timescale`](../../../aspose.tasks.visualization/timescale/), el [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) y el rango de fechas proporcionados.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageSize | PageSize | El tamaño para el que se obtendrá el recuento de páginas. |
| escala | Timescale | La escala para la que se obtendrá el recuento de páginas. |
| startDate | DateTime | La fecha de inicio para la que se obtendrá el recuento de páginas. |
| endDate | DateTime | La fecha de finalización para la que se obtendrá el recuento de páginas. |

### Valor devuelto

Recuento de páginas a renderizar.

## Ejemplos

Muestra cómo obtener el recuento de páginas por tamaño de página, escala de tiempo, fecha de inicio y fecha de finalización.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### Ver también

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Devuelve el recuento de páginas para el proyecto que se renderizará usando el [`Timescale`](../../../aspose.tasks.visualization/timescale/) y el [`PageSize`](../../../aspose.tasks.visualization/pagesize/) proporcionados.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageSize | PageSize | El tamaño para el que se obtendrá el recuento de páginas. |
| escala | Timescale | La escala para la que se obtendrá el recuento de páginas. |

### Valor devuelto

Recuento de páginas a renderizar.

## Ejemplos

Muestra cómo obtener el recuento de páginas por tamaño de página y escala de tiempo.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### Ver también

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


