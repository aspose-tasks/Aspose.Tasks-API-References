---
title: "Clase Metered"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Metered. Proporciona métodos para establecer la clave medida"
type: docs
weight: 1020
url: /es/net/aspose.tasks/metered/
---
## Metered class

Proporciona métodos para establecer la clave medida.

```csharp
public class Metered
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Metered](metered/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | Comprueba si el producto está licenciado correctamente mediante una licencia medida. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Elimina la licencia configurada previamente. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Establece claves públicas y privadas medidas. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Obtiene el crédito de consumo. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Obtiene el tamaño del archivo de consumo. |

## Ejemplos

En este ejemplo, se intentará establecer la clave pública y privada medida

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

el archivo jar del componente:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


