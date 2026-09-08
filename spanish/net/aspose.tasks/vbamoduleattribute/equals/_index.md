---
title: "VbaModuleAttribute.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método VbaModuleAttribute. Devuelve un valor que indica si esta instancia es igual al objeto VbaModuleAttribute especificado"
type: docs
weight: 30
url: /es/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

Devuelve un valor que indica si esta instancia es igual al objeto [`VbaModuleAttribute`](../) especificado.

```csharp
public bool Equals(VbaModuleAttribute other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | VbaModuleAttribute | El objeto [`VbaModuleAttribute`](../) especificado para comparar con esta instancia. |

### Valor devuelto

Devuelve true si esta instancia es igual al objeto [`VbaModuleAttribute`](../) especificado; de lo contrario, false.

## Ejemplos

Muestra cómo comprobar la igualdad de los atributos del módulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Ver también

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Devuelve un valor que indica si esta instancia es igual al objeto [`VbaModuleAttribute`](../) especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Object | El objeto [`VbaModuleAttribute`](../) especificado para comparar con esta instancia. |

### Valor devuelto

Devuelve true si esta instancia es igual al objeto [`VbaModuleAttribute`](../) especificado; de lo contrario, false.

## Ejemplos

Muestra cómo comprobar la igualdad de los atributos del módulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Ver también

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


