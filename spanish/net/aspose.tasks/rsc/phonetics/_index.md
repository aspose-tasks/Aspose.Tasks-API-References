---
title: "Rsc.Phonetics"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La ortografía fonética del nombre del recurso. Solo para uso con japonés"
type: docs
weight: 560
url: /es/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

La ortografía fonética del nombre del recurso. Solo para uso con japonés.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Phonetics.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


