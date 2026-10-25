---
title: "Prj.CriticalSlackLimit"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Las tareas se consideran críticas en MS Project si el holgura total es menor o igual a este número de días"
type: docs
weight: 140
url: /es/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

MS Project considera que las tareas son críticas si el holgura total es menor o igual a este número de días.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.CriticalSlackLimit.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


