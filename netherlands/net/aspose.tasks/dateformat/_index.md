---
title: "Enum DateFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.DateFormat enum. Geeft het datumformaat op."
type: docs
weight: 430
url: /nl/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

Specificeert het datumformaat.

```csharp
public enum DateFormat
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | Het voorbeeld: 09/30/02 13:00 PM |
| DateMmDdYy | `1` | Het voorbeeld: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | Het voorbeeld: September 30, 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | Het voorbeeld: September 30, 2002 |
| DateMmmDdHhMmAM | `4` | Het voorbeeld: Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | Het voorbeeld: Sep 30, '02 |
| DateMmmmDd | `6` | Het voorbeeld: September 30 |
| DateMmmDd | `7` | Het voorbeeld: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | Het voorbeeld: Di 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | Het voorbeeld: Di 9/30/02 |
| DateDddMmmDdYyy | `10` | Het voorbeeld: Di Sep 30, '02 |
| DateDddHhMmAM | `11` | Het voorbeeld: Di 13:00 PM |
| DateMmDd | `12` | Het voorbeeld: 9/30 |
| DateDd | `13` | Het voorbeeld: 30 |
| DateHhMmAm | `14` | Het voorbeeld: 13:00 PM |
| DateDddMmmDd | `15` | Het voorbeeld: Di Sep 30 |
| DateDddMmDd | `16` | Het voorbeeld: Di 9/30 |
| DateDddDd | `17` | Het voorbeeld: Di 30 |
| DateWwwDd | `18` | Het voorbeeld: W41/2 |
| DateWwwDdYyHhMmAm | `19` | Het voorbeeld: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | Het voorbeeld: 9/30/2002 |
| Custom | `21` | DateTime-waarden worden opgemaakt met behulp van een opmaakstring die is ingesteld op de [`CustomDateFormat`](../prj/customdateformat/) eigenschap van het project. |
| DateDdMmYyyy | `256` | Het voorbeeld: 19/07/2016 |
| Default | `255` | Het voorbeeld: Standaard datumformaat. |

## Voorbeelden

Toont hoe het datumformaat van alle datums in het project kan worden aangepast voor export.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// Standaard project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Ma 09/22/14) pas DateFormat aan (September 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// Exporteren naar datumformaat 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


