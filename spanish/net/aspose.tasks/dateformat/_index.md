---
title: "Enum DateFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enum Aspose.Tasks.DateFormat. Especifica el formato de fecha."
type: docs
weight: 430
url: /es/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

Especifica el formato de fecha.

```csharp
public enum DateFormat
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | El ejemplo: 09/30/02 13:00 PM |
| DateMmDdYy | `1` | El ejemplo: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | El ejemplo: 30 de septiembre de 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | El ejemplo: 30 de septiembre de 2002 |
| DateMmmDdHhMmAM | `4` | El ejemplo: Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | El ejemplo: Sep 30, '02 |
| DateMmmmDd | `6` | El ejemplo: 30 de septiembre |
| DateMmmDd | `7` | El ejemplo: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | El ejemplo: mar 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | El ejemplo: mar 9/30/02 |
| DateDddMmmDdYyy | `10` | El ejemplo: mar Sep 30, '02 |
| DateDddHhMmAM | `11` | El ejemplo: mar 13:00 PM |
| DateMmDd | `12` | El ejemplo: 9/30 |
| DateDd | `13` | El ejemplo: 30 |
| DateHhMmAm | `14` | El ejemplo: 13:00 PM |
| DateDddMmmDd | `15` | El ejemplo: mar Sep 30 |
| DateDddMmDd | `16` | El ejemplo: mar 9/30 |
| DateDddDd | `17` | El ejemplo: mar 30 |
| DateWwwDd | `18` | El ejemplo: W41/2 |
| DateWwwDdYyHhMmAm | `19` | El ejemplo: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | El ejemplo: 9/30/2002 |
| Custom | `21` | Los valores DateTime se formatean usando la cadena de formato que está establecida en la propiedad [`CustomDateFormat`](../prj/customdateformat/) del proyecto. |
| DateDdMmYyyy | `256` | El ejemplo: 19/07/2016 |
| Default | `255` | El ejemplo: Formato de fecha predeterminado. |

## Ejemplos

Muestra cómo personalizar el formato de fecha de todas las fechas en el proyecto para exportarlas.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// Por defecto project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Lun 09/22/14) personaliza DateFormat (22 de septiembre de 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// Exportar al formato de fecha 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


