---
title: Project.GetPageCount
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Project método. Devuelve el recuento de páginas del proyecto que se representará utilizandoSaveOptions .
type: docs
weight: 1080
url: /es/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Devuelve el recuento de páginas del proyecto que se representará utilizando[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| saveOptions | SaveOptions | Las opciones de guardado para obtener el recuento de páginas. |

### Valor_devuelto

un recuento de páginas que se representará.

### Ejemplos

En este ejemplo, la instancia de HtmlSaveOptions y el número de páginas del HTML resultante se escriben en la consola.

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

### Ver también

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* espacio de nombres [Aspose.Tasks](../../project/)
* asamblea [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Devuelve el recuento de páginas para que el proyecto se represente usando el valor predeterminado[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Días).

```csharp
public int GetPageCount()
```

### Valor_devuelto

Recuento de páginas que se van a representar.

### Ver también

* class [Project](../)
* espacio de nombres [Aspose.Tasks](../../project/)
* asamblea [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Devuelve el recuento de páginas del proyecto que se representará utilizando[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| scale | Timescale | La escala para obtener el recuento de páginas. |

### Valor_devuelto

Recuento de páginas que se van a representar.

### Ver también

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* espacio de nombres [Aspose.Tasks](../../project/)
* asamblea [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Devuelve el recuento de páginas para que el proyecto se represente usando el valor predeterminado[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Días) y dado[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| format | PresentationFormat | El formato para obtener el recuento de páginas. |

### Valor_devuelto

Recuento de páginas que se van a representar.

### Ver también

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* espacio de nombres [Aspose.Tasks](../../project/)
* asamblea [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Devuelve el recuento de páginas del proyecto que se representará utilizando[`Timescale`](../../../aspose.tasks.visualization/timescale/) y[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| format | PresentationFormat | El formato para obtener el recuento de páginas. |
| scale | Timescale | La escala para obtener el recuento de páginas. |

### Valor_devuelto

un recuento de páginas que se representará.

### Ver también

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* espacio de nombres [Aspose.Tasks](../../project/)
* asamblea [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Devuelve el recuento de páginas del proyecto que se representará utilizando[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) y rango de fechas.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageSize | PageSize | El tamaño para obtener el recuento de páginas. |
| scale | Timescale | La escala para obtener el recuento de páginas. |
| startDate | DateTime | La fecha de inicio para obtener el recuento de páginas. |
| endDate | DateTime | La fecha de finalización para obtener el recuento de páginas. |

### Valor_devuelto

Recuento de páginas que se van a representar.

### Ver también

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* espacio de nombres [Aspose.Tasks](../../project/)
* asamblea [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Devuelve el recuento de páginas del proyecto que se representará utilizando[`Timescale`](../../../aspose.tasks.visualization/timescale/) y[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageSize | PageSize | El tamaño para obtener el recuento de páginas. |
| scale | Timescale | La escala para obtener el recuento de páginas. |

### Valor_devuelto

Recuento de páginas que se van a representar.

### Ver también

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* espacio de nombres [Aspose.Tasks](../../project/)
* asamblea [Aspose.Tasks](../../../)


