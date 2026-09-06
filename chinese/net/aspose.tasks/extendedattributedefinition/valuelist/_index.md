---
title: "ExtendedAttributeDefinition.ValueList"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttributeDefinition 属性。获取 ListValue ValueList"
type: docs
weight: 280
url: /zh/net/aspose.tasks/extendedattributedefinition/valuelist/
---
## ExtendedAttributeDefinition.ValueList property

获取 List&lt;Value&gt; ValueList。

```csharp
public List<Value> ValueList { get; }
```

## 备注

当在模式的元素属性中指定扩展属性的值时，可以通过直接值或对本列表中包含的值的引用来指定。应用程序可以根据此处指定的顺序假设列表的顺序。目前支持 MSP 2003/2007 Xml 和 MSP 2003 mpp 格式。请勿直接修改此列表。请改用 ExtendedAttributeDefinition.AddLookupValue/RemoveLookupValue 方法。

## 示例

展示如何读取扩展属性定义的通用信息。

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// 读取扩展属性定义信息
foreach (var definition in project.ExtendedAttributes)
{
    Console.WriteLine("Guid:" + definition.Guid);
    Console.WriteLine("Secondary Guid:" + definition.SecondaryGuid);
    Console.WriteLine("Secondary Pid:" + definition.SecondaryPid);
    Console.WriteLine("Alias:" + definition.Alias);
    Console.WriteLine("Phonetics Alias:" + definition.PhoneticsAlias);
    Console.WriteLine("Field Id:" + definition.FieldId);
    Console.WriteLine("Project Name:" + definition.ParentProject.Get(Prj.Name));

    Console.WriteLine("Append New Values:" + definition.AppendNewValues);
    Console.WriteLine("Auto RollDown:" + definition.AutoRollDown);
    Console.WriteLine("Calculation Type:" + definition.CalculationType);
    Console.WriteLine("Field Name" + definition.FieldName);
    Console.WriteLine("Is User Defined Custom Field:" + definition.UserDef);
    Console.WriteLine("Rollup Type:" + definition.RollupType);

    if (definition.CalculationType == CalculationType.Lookup)
    {
        Console.WriteLine("  Next properties are used only for lookups:");
        Console.WriteLine("  Default Guid:" + definition.DefaultGuid);
        Console.WriteLine("  Element Type:" + definition.ElementType);
        Console.WriteLine("  Lookup Uid:" + definition.LookupUid);
        Console.WriteLine("  Restrict Values:" + definition.RestrictValues);
        Console.WriteLine("  Max Multi Values:" + definition.MaxMultiValues);
        Console.WriteLine("  Valuelist Sort Order:" + definition.ValuelistSortOrder);
        Console.WriteLine("  Default Value:" + definition.Default);
        Console.WriteLine("  Print values from value list:");
        foreach (var value in definition.ValueList)
        {
            Console.WriteLine("    Description: " + value.Description);
            Console.WriteLine("    Value: " + value.Val);
        }
    }

    Console.WriteLine();
}
```

### 另见

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


