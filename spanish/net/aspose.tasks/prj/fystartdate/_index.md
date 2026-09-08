---
title: "Prj.FyStartDate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El mes en que comienza el año fiscal"
type: docs
weight: 350
url: /es/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

El mes en que comienza el año fiscal.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
```

## Ejemplos

Muestra cómo escribir las propiedades del año fiscal.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// Establecer propiedades del año fiscal
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// Mostrar propiedades del año fiscal
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


