---
title: "Metered.GetConsumptionQuantity"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Metered. Obtiene el tamaño del archivo de consumo"
type: docs
weight: 60
url: /es/net/aspose.tasks/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Obtiene el tamaño del archivo de consumo.

```csharp
public static decimal GetConsumptionQuantity()
```

### Valor devuelto

Devuelve el número de bytes consumidos.

## Ejemplos

Muestra cómo usar &lt;see cref="Aspose.Tasks.Metered" /&gt; tipo de licencia con Aspose.Tasks.

```csharp
// Utilicemos la licencia medida (ver https://purchase.aspose.com/faqs/licensing/metered)
// establecer licencia medida
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// trabajar con el proyecto...
// ...

// Podemos obtener los créditos actuales y el consumo de bytes.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // registrar excepción
}

// recientemente el usuario puede restablecer una licencia medida y detener el conteo de bytes
metered.ResetMeteredKey();
```

### Ver también

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


