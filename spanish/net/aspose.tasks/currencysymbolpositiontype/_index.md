---
title: "Enumeración CurrencySymbolPositionType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.CurrencySymbolPositionType. Especifica la posición de un símbolo de moneda."
type: docs
weight: 370
url: /es/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

Especifica la posición del símbolo de moneda.

```csharp
public enum CurrencySymbolPositionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | Indica que un valor indefinido significa que el campo no estaba definido en el archivo de proyecto original. |
| Before | `0` | Indica el tipo de posición del símbolo de moneda antes. |
| After | `1` | Indica el tipo de posición del símbolo de moneda después. |
| BeforeWithSpace | `2` | Indica el tipo de posición del símbolo de moneda antes con espacio. |
| AfterWithSpace | `3` | Indica el tipo de posición del símbolo de moneda después con espacio. |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo especificar la ubicación del símbolo de moneda (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// establecer la ubicación del símbolo de moneda
// Antes, sin espacio ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// trabajar con el proyecto...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


