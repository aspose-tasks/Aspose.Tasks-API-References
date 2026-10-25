---
title: "LoadOptions.ErrorHandler"
second_title: "Aspose.Tasks for .NET API 参考"
description: "LoadOptions 属性。获取或设置用于处理 xml 解析错误的回调方法"
type: docs
weight: 40
url: /zh/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

获取或设置处理 XML 解析错误的回调方法。

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## 示例

展示如何从 Primavera XML 文件中读取项目（解析错误）。

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// 返回具有特殊 UID 的项目
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

展示如何使用 &lt;see cref=\"LoadOptions\" /&gt; 加载 Primavera 项目并进行错误处理。

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // 设置 Primavera 读取选项
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // 处理项目...
}

private static object CustomDurationHandlerForFile(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var value = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", value);
    return value;
}
```

### 另见

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


