---
title: "委托 ParseErrorCallback"
second_title: "Aspose.Tasks for .NET API 参考"
description: "表示用于处理读取 XML 数据时可能出现的解析错误的方法回调"
type: docs
weight: 1250
url: /zh/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

表示用于处理读取 XML 数据时可能出现的解析错误的方法回调。

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 发送者 | 对象 | 解析错误的源对象。 |
| args | ParseErrorArgs | 包含事件数据的 [`ParseErrorArgs`](../parseerrorargs/) 类的实例。 |

### 返回值

要设置到指定发送者对象的强制转换值。

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


