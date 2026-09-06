---
title: "Project.GetWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Obtient un objet Duration avec la valeur Double spécifiée et le format de travail par défaut"
type: docs
weight: 1130
url: /fr/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

Obtient l'objet [`Duration`](../../duration/) avec la valeur Double spécifiée et le format de travail par défaut.

```csharp
public Duration GetWork(double val)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| val | Double | valeur double spécifiée. |

### Valeur de retour

Objet Duration.

## Remarques

Cette méthode doit être utilisée avec précaution car elle renvoie des durées différentes selon le paramètre Project.WorkFormat. Par exemple, GetWork(1.0) renverra 1 heure lorsque Project.WorkFormat est TimeUnitType.Hour ou 1 jour si Project.WorkFormat est TimeUnitType.Day.

## Exemples

Montre comment obtenir un travail avec le format de travail par défaut.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// créer une valeur de travail avec le format de travail par défaut du projet
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Voir aussi

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


