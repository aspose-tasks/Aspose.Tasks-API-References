---
title: "Tsk.EarnedValueMethod"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si el campo Complete o Physical Complete debe usarse para calcular el costo presupuestado del trabajo realizado BCWP"
type: docs
weight: 350
url: /es/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

Determina si el campo % Complete o Physical % Complete debe usarse para calcular el costo presupuestado del trabajo realizado (BCWP).

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.EarnedValueMethod.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


