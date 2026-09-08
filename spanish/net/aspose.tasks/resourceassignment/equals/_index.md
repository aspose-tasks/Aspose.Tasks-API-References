---
title: "ResourceAssignment.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceAssignment. Devuelve un valor que indica si esta instancia es igual a una instancia especificada de la clase ResourceAssignment"
type: docs
weight: 690
url: /es/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

Devuelve un valor que indica si esta instancia es igual a una instancia especificada de la clase [`ResourceAssignment`](../).

```csharp
public bool Equals(ResourceAssignment other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | ResourceAssignment | La instancia especificada de la clase [`ResourceAssignment`](../) para comparar con esta instancia. |

### Valor devuelto

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## Ejemplos

Muestra cómo comprobar la igualdad de asignaciones de recursos.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Ver también

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El objeto para comparar con esta instancia. |

### Valor devuelto

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## Ejemplos

Muestra cómo comprobar la igualdad de asignaciones de recursos.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Ver también

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


