---
title: "Project.SaveReport"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Enregistre le rapport d'aperçu du projet dans le flux."
type: docs
weight: 1220
url: /fr/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

Enregistre le rapport d’aperçu du projet dans le flux.

```csharp
public void SaveReport(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Le flux où enregistrer le rapport du projet. |

## Exemples

Montre comment enregistrer le rapport d'aperçu du projet au format PDF.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// Enregistrez le rapport d'aperçu au format PDF dans le flux spécifié.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

Enregistre le rapport d’aperçu du projet dans un fichier PDF.

```csharp
public void SaveReport(string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | Chaîne | Le nom du fichier. |

## Exemples

Montre comment enregistrer le rapport d'aperçu du projet au format PDF dans un flux.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// On peut enregistrer le rapport d'aperçu au format PDF dans le chemin spécifié
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

Enregistre le rapport du projet du type spécifié dans le flux spécifié.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Le flux spécifié où enregistrer le rapport du projet. |
| reportType | ReportType | Le type de rapport spécifié.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Exemples

Montre comment enregistrer le rapport du projet au format PDF pour un type de rapport spécifique.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// Enregistrez le rapport d'aperçu au format PDF dans le flux spécifié.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Voir aussi

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

Enregistre le rapport du projet du type spécifié au format PDF dans le chemin de fichier spécifié.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | Chaîne | le nom de fichier spécifié. |
| reportType | ReportType | Le type de rapport spécifié.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Exemples

Montre comment enregistrer le rapport du projet projet au format PDF.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### Voir aussi

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


