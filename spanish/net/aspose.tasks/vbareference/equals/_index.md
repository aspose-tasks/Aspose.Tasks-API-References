---
title: "VbaReference.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método VbaReference. Devuelve un valor que indica si esta instancia es igual al objeto VbaReference especificado"
type: docs
weight: 40
url: /es/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

Devuelve un valor que indica si esta instancia es igual al objeto [`VbaReference`](../) especificado.

```csharp
public bool Equals(VbaReference other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | VbaReference | El objeto [`VbaReference`](../) especificado para comparar con esta instancia. |

### Valor devuelto

Devuelve true si esta instancia es igual al objeto [`VbaReference`](../) especificado; de lo contrario, false.

## Ejemplos

Muestra cómo comprobar la igualdad de referencias VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// La igualdad de referencias se verifica contra el nombre de la referencia.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Ver también

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Devuelve un valor que indica si esta instancia es igual al objeto [`VbaReference`](../) especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Object | El objeto [`VbaReference`](../) especificado para comparar con esta instancia. |

### Valor devuelto

Devuelve true si esta instancia es igual al objeto [`VbaReference`](../) especificado; de lo contrario, false.

## Ejemplos

Muestra cómo comprobar la igualdad de referencias VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// La igualdad de referencias se verifica contra el nombre de la referencia.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Ver también

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


