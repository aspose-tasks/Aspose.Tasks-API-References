---
title: "Énumération DateFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.DateFormat. Spécifie le format de date."
type: docs
weight: 430
url: /fr/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

Spécifie le format de date.

```csharp
public enum DateFormat
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | L'exemple : 09/30/02 13:00 PM |
| DateMmDdYy | `1` | L'exemple : 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | L'exemple : 30 septembre 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | L'exemple : 30 septembre 2002 |
| DateMmmDdHhMmAM | `4` | L'exemple : Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | L'exemple : Sep 30, '02 |
| DateMmmmDd | `6` | L'exemple : septembre 30 |
| DateMmmDd | `7` | L'exemple : sep 30 |
| DateDddMmDdYyHhMmAM | `8` | L'exemple : Mar 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | L'exemple : Mar 9/30/02 |
| DateDddMmmDdYyy | `10` | L'exemple : Mar sep 30, '02 |
| DateDddHhMmAM | `11` | L'exemple : Mar 13:00 PM |
| DateMmDd | `12` | L'exemple : 9/30 |
| DateDd | `13` | L'exemple : 30 |
| DateHhMmAm | `14` | L'exemple : 13:00 PM |
| DateDddMmmDd | `15` | L'exemple : Mar sep 30 |
| DateDddMmDd | `16` | L'exemple : Mar 9/30 |
| DateDddDd | `17` | L'exemple : Mar 30 |
| DateWwwDd | `18` | L'exemple : W41/2 |
| DateWwwDdYyHhMmAm | `19` | L'exemple : W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | L'exemple : 9/30/2002 |
| Custom | `21` | Les valeurs DateTime sont formatées à l'aide d'une chaîne de format qui est définie sur la propriété du projet [`CustomDateFormat`](../prj/customdateformat/). |
| DateDdMmYyyy | `256` | L'exemple : 19/07/2016 |
| Default | `255` | L'exemple : Format de date par défaut. |

## Exemples

Montre comment personnaliser le format de date de toutes les dates du projet à exporter.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// Par défaut project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Lun 09/22/14) personnalisez DateFormat (septembre 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// Exporter au format de date 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


