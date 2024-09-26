---
title: Rsc.Phonetics
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The phonetic spelling of the resource name. For use with Japanese only
type: docs
weight: 560
url: /net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

The phonetic spelling of the resource name. For use with Japanese only.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## Examples

Shows how to read/write Rsc.Phonetics property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


