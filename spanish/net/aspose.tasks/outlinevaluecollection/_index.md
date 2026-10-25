---
title: "Clase OutlineValueCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.OutlineValueCollection. Representa una colección de objetos OutlineValue"
type: docs
weight: 1220
url: /es/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

Representa una colección de [`OutlineValue`](../outlinevalue/) objetos.

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | Obtiene el número de elementos contenidos en esta colección. |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura. |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | Devuelve o establece el elemento en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | Agrega el elemento especificado a esta colección. |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | Elimina todos los elementos de esta colección. |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado. |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | Determina el índice del elemento especificado en esta colección. |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | Inserta el elemento especificado en el índice especificado. |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | Elimina la primera aparición de un objeto específico de esta colección. |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | Elimina un elemento en el índice especificado. |

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

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


