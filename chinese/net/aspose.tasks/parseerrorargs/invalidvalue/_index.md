---
title: "ParseErrorArgs.InvalidValue"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ParseErrorArgs 属性。获取导致异常的字符串值"
type: docs
weight: 40
url: /zh/net/aspose.tasks/parseerrorargs/invalidvalue/
---
## ParseErrorArgs.InvalidValue property

获取导致异常的字符串值。

```csharp
public string InvalidValue { get; }
```

## 示例

展示如何从包含无效字符的 XML 文件的流中读取项目。

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // 打开包含损坏时间跨度的 XML 文件。
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### 另见

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


