---
title: "Enum DateFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.DateFormat. Specifica il formato della data."
type: docs
weight: 430
url: /it/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

Specifica il formato della data.

```csharp
public enum DateFormat
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | L'esempio: 09/30/02 13:00 PM |
| DateMmDdYy | `1` | L'esempio: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | L'esempio: 30 settembre 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | L'esempio: 30 settembre 2002 |
| DateMmmDdHhMmAM | `4` | L'esempio: set 30 13:00 PM |
| DateMmmDdYyy | `5` | L'esempio: Sep 30, '02 |
| DateMmmmDd | `6` | L'esempio: 30 settembre |
| DateMmmDd | `7` | L'esempio: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | L'esempio: Tue 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | L'esempio: Tue 9/30/02 |
| DateDddMmmDdYyy | `10` | L'esempio: Tue Sep 30, '02 |
| DateDddHhMmAM | `11` | L'esempio: Tue 13:00 PM |
| DateMmDd | `12` | L'esempio: 9/30 |
| DateDd | `13` | L'esempio: 30 |
| DateHhMmAm | `14` | L'esempio: 13:00 PM |
| DateDddMmmDd | `15` | L'esempio: Tue Sep 30 |
| DateDddMmDd | `16` | L'esempio: Tue 9/30 |
| DateDddDd | `17` | L'esempio: Tue 30 |
| DateWwwDd | `18` | L'esempio: W41/2 |
| DateWwwDdYyHhMmAm | `19` | L'esempio: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | L'esempio: 9/30/2002 |
| Custom | `21` | I valori DateTime sono formattati usando la stringa di formato impostata nella proprietà [`CustomDateFormat`](../prj/customdateformat/) del progetto. |
| DateDdMmYyyy | `256` | L'esempio: 19/07/2016 |
| Default | `255` | L'esempio: Formato data predefinito. |

## Esempi

Mostra come personalizzare il formato data di tutte le date nel progetto da esportare.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// Per impostazione predefinita project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14) personalizza DateFormat (22 settembre 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// Esporta nel formato data 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


