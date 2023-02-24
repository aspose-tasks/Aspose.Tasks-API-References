---
title: Class Metered
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.Metered clase. Proporciona métodos para configurar la clave medida.
type: docs
weight: 890
url: /es/net/aspose.tasks/metered/
---
## Metered class

Proporciona métodos para configurar la clave medida.

```csharp
public class Metered
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Metered](metered/)() | Constructor predeterminado |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Elimina la licencia de instalación anterior. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Establece claves públicas y privadas medidas. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Obtiene crédito de consumo. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Obtiene el tamaño del archivo de consumo. |

### Ejemplos

En este ejemplo, se intentará establecer una clave pública y privada medidas

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

### Ver también

* espacio de nombres [Aspose.Tasks](../../aspose.tasks/)
* asamblea [Aspose.Tasks](../../)


