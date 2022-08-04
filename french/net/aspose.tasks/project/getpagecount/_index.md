---
title: GetPageCount
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Renvoie le nombre de pages pour le projet à rendre en utilisantSaveOptionsaspose.tasks.saving/saveoptions .
type: docs
weight: 300
url: /fr/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Renvoie le nombre de pages pour le projet à rendre en utilisant[`SaveOptions`](../../../aspose.tasks.saving/saveoptions) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| saveOptions | SaveOptions | Les options de sauvegarde pour lesquelles obtenir le nombre de pages. |

### Return_Value

un nombre de pages à rendre.

### Exemples

Dans cet exemple, l'instance de HtmlSaveOptions et le nombre de pages dans le code HTML résultant sont écrits dans la console.

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

### Voir également

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions)
* class [Project](../../project)
* espace de noms [Aspose.Tasks](../../project)
* Assemblée [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Renvoie le nombre de pages pour le projet à rendre en utilisant la valeur par défaut[`Timescale`](../../../aspose.tasks.visualization/timescale) (Jours).

```csharp
public int GetPageCount()
```

### Return_Value

Nombre de pages à afficher.

### Voir également

* class [Project](../../project)
* espace de noms [Aspose.Tasks](../../project)
* Assemblée [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Renvoie le nombre de pages pour le projet à rendre en utilisant[`Timescale`](../../../aspose.tasks.visualization/timescale) .

```csharp
public int GetPageCount(Timescale scale)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| scale | Timescale | L'échelle pour laquelle obtenir le nombre de pages. |

### Return_Value

Nombre de pages à afficher.

### Voir également

* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* espace de noms [Aspose.Tasks](../../project)
* Assemblée [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Renvoie le nombre de pages pour le projet à rendre en utilisant la valeur par défaut[`Timescale`](../../../aspose.tasks.visualization/timescale) (Jours) et donné[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| format | PresentationFormat | Le format pour lequel obtenir le nombre de pages. |

### Return_Value

Nombre de pages à afficher.

### Voir également

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat)
* class [Project](../../project)
* espace de noms [Aspose.Tasks](../../project)
* Assemblée [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Renvoie le nombre de pages pour le projet à rendre en utilisant[`Timescale`](../../../aspose.tasks.visualization/timescale) et[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| format | PresentationFormat | Le format pour lequel obtenir le nombre de pages. |
| scale | Timescale | L'échelle pour laquelle obtenir le nombre de pages. |

### Return_Value

un nombre de pages à rendre.

### Voir également

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* espace de noms [Aspose.Tasks](../../project)
* Assemblée [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Renvoie le nombre de pages pour le projet à rendre en utilisant[`Timescale`](../../../aspose.tasks.visualization/timescale) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat) et plage de dates.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageSize | PageSize | La taille pour laquelle obtenir le nombre de pages. |
| scale | Timescale | L'échelle pour laquelle obtenir le nombre de pages. |
| startDate | DateTime | La date de début pour laquelle obtenir le nombre de pages. |
| endDate | DateTime | La date de fin pour laquelle obtenir le nombre de pages. |

### Return_Value

Nombre de pages à afficher.

### Voir également

* enum [PageSize](../../../aspose.tasks.visualization/pagesize)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* espace de noms [Aspose.Tasks](../../project)
* Assemblée [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Renvoie le nombre de pages pour le projet à rendre en utilisant[`Timescale`](../../../aspose.tasks.visualization/timescale) et[`PageSize`](../../../aspose.tasks.visualization/pagesize) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageSize | PageSize | La taille pour laquelle obtenir le nombre de pages. |
| scale | Timescale | L'échelle pour laquelle obtenir le nombre de pages. |

### Return_Value

Nombre de pages à afficher.

### Voir également

* enum [PageSize](../../../aspose.tasks.visualization/pagesize)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* espace de noms [Aspose.Tasks](../../project)
* Assemblée [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
