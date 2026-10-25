---
title: "Resource.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Resource. Devuelve un valor que indica si esta instancia es igual a una instancia especificada de la clase Resource"
type: docs
weight: 820
url: /es/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

Devuelve un valor que indica si esta instancia es igual a una instancia especificada de la [`Resource`](../) clase.

```csharp
public bool Equals(Resource other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | Resource | La instancia especificada de la [`Resource`](../) clase para comparar con esta instancia. |

### Valor devuelto

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## Ejemplos

Muestra cómo comprobar la igualdad de recursos.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Ver también

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
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

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## Ejemplos

Muestra cómo comprobar la igualdad de recursos.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Ver también

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


