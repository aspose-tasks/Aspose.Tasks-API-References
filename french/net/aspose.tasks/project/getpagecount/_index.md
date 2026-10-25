---
title: "Project.GetPageCount"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Retourne le nombre de pages du projet à rendre en utilisant les SaveOptions fournis"
type: docs
weight: 1110
url: /fr/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Retourne le nombre de pages du projet à rendre en utilisant les [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveOptions | SaveOptions | Les options de sauvegarde pour obtenir le nombre de pages. |

### Valeur de retour

un nombre de pages à rendre.

## Exemples

Dans cet exemple, l'instance de HtmlSaveOptions et le nombre de pages du HTML résultant sont écrits dans la console.

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

Montre comment obtenir le nombre de pages pour des options d'enregistrement spécifiques.

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

### Voir aussi

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days) par défaut.

```csharp
public int GetPageCount()
```

### Valeur de retour

Nombre de pages à rendre.

## Exemples

Montre comment obtenir le nombre de pages pour différentes échelles de temps.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Obtenir le nombre de pages, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../../aspose.tasks.visualization/timescale/) fourni.

```csharp
public int GetPageCount(Timescale scale)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| échelle | Timescale | L'échelle pour obtenir le nombre de pages. |

### Valeur de retour

Nombre de pages à rendre.

## Exemples

Montre comment obtenir le nombre de pages pour différentes échelles de temps.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Obtenir le nombre de pages, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Voir aussi

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days) par défaut et le [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) fourni.

```csharp
public int GetPageCount(PresentationFormat format)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| format | PresentationFormat | Le format pour obtenir le nombre de pages. |

### Valeur de retour

Nombre de pages à rendre.

## Exemples

Montre comment obtenir le nombre de pages par format de présentation et échelle de temps.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Obtenir le nombre de pages pour Days (par défaut), Months et ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Voir aussi

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../../aspose.tasks.visualization/timescale/) et le [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) fournis.

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| format | PresentationFormat | Le format pour obtenir le nombre de pages. |
| échelle | Timescale | L'échelle pour obtenir le nombre de pages. |

### Valeur de retour

un nombre de pages à rendre.

## Exemples

Montre comment obtenir le nombre de pages par format de présentation et échelle de temps.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Obtenir le nombre de pages pour Days (par défaut), Months et ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Voir aussi

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../../aspose.tasks.visualization/timescale/), le [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) et la plage de dates.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageSize | PageSize | La taille pour obtenir le nombre de pages. |
| échelle | Timescale | L'échelle pour obtenir le nombre de pages. |
| startDate | DateTime | La date de début pour obtenir le nombre de pages. |
| endDate | DateTime | La date de fin pour obtenir le nombre de pages. |

### Valeur de retour

Nombre de pages à rendre.

## Exemples

Montre comment obtenir le nombre de pages par taille de page, échelle de temps, dates de début et de fin.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### Voir aussi

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../../aspose.tasks.visualization/timescale/) et le [`PageSize`](../../../aspose.tasks.visualization/pagesize/) fournis.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageSize | PageSize | La taille pour obtenir le nombre de pages. |
| échelle | Timescale | L'échelle pour obtenir le nombre de pages. |

### Valeur de retour

Nombre de pages à rendre.

## Exemples

Montre comment obtenir le nombre de pages selon une taille de page et une échelle de temps.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### Voir aussi

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


