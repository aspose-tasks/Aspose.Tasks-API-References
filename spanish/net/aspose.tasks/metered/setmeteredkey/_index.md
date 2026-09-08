---
title: "Metered.SetMeteredKey"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Metered. Establece las claves públicas y privadas de Metered"
type: docs
weight: 40
url: /es/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Establece claves públicas y privadas medidas.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| publicKey | Cadena | La clave pública. |
| privateKey | Cadena | La clave privada. |

## Observaciones

Si compra una licencia por consumo, esta API debe llamarse al iniciar la aplicación; normalmente, eso es suficiente. Sin embargo, si el consumo falla al subir los datos de consumo durante un período de 24 horas, la licencia se establecerá en estado de evaluación. Para evitar este caso, debe comprobar regularmente el estado de la licencia. Si está en estado de evaluación, llame a esta API nuevamente.

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


