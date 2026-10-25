---
title: "OutlineValueCollection.Count"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "OutlineValueCollection propiedad. Obtiene el número de elementos contenidos en esta colección"
type: docs
weight: 10
url: /es/net/aspose.tasks/outlinevaluecollection/count/
---
## OutlineValueCollection.Count property

Obtiene el número de elementos contenidos en esta colección.

```csharp
public int Count { get; }
```

## Ejemplos

Muestra cómo trabajar con colecciones de valores de contorno.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// borrar colecciones de valores
foreach (var outlineCode in project.OutlineCodes)
{
    // borrar máscaras de contorno
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// actualizar valor mediante acceso por índice
codeDefinition.Values[0].Value = "654321";

// iterar sobre valores de contorno
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// trabajar con valores de contorno
// ...

// eliminar un valor cuando sea necesario
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// insertar un valor en la posición inicial
codeDefinition.Values.Insert(0, value);

// verificar la posición del valor insertado
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// trabajar con valores de contorno
// ...

// eliminar el último valor de la colección
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// uno puede crear otra definición de código de contorno
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// y luego copiar valores de contorno
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### Ver también

* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


