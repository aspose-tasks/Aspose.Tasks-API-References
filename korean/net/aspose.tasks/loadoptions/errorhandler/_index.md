---
title: "LoadOptions.ErrorHandler"
second_title: "Aspose.Tasks for .NET API 참조"
description: "LoadOptions 속성. XML 구문 분석 오류를 처리하기 위한 콜백 메서드를 가져오거나 설정합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

XML 구문 분석 오류를 처리하기 위한 콜백 메서드를 가져오거나 설정합니다.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## 예제

오류가 발생한 파싱을 포함한 Primavera XML 파일에서 프로젝트를 읽는 방법을 보여줍니다.

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

// 특수 UID를 가진 프로젝트를 반환합니다.
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

오류 처리를 포함하여 &lt;see cref=\"LoadOptions\" /&gt;를 사용해 Primavera 프로젝트를 로드하는 방법을 보여줍니다.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // Primavera 읽기 옵션 설정
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // 프로젝트와 작업...
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

### 또 보기

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


