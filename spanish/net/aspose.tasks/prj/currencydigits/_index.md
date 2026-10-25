---
title: "Prj.CurrencyDigits"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El número de dígitos después del símbolo decimal"
type: docs
weight: 160
url: /es/net/aspose.tasks/prj/currencydigits/
---
## Prj.CurrencyDigits field

El número de dígitos después del símbolo decimal.

```csharp
public static readonly Key<int, PrjKey> CurrencyDigits;
```

## Ejemplos

Muestra cómo escribir las propiedades de moneda del proyecto.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// Establecer propiedades de moneda
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// Mostrar propiedades de moneda
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


