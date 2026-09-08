---
title: "Tsk.NotesText"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Texto plano de notas extraído de datos RTF"
type: docs
weight: 830
url: /es/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

Texto plano de las notas extraído de los datos RTF.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.NotesText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


