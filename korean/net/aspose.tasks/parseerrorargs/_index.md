---
title: "클래스 ParseErrorArgs"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ParseErrorArgs 클래스. ParseErrorCallback 대리자에 대한 데이터를 제공합니다."
type: docs
weight: 1240
url: /ko/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

`ParseErrorCallback` 대리자에 대한 데이터를 제공합니다.

```csharp
public class ParseErrorArgs
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | 문자열 값을 구문 분석하는 동안 발생한 예외를 가져옵니다. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | 객체 필드 이름을 가져옵니다. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | 객체 필드 유형을 가져옵니다. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | 예외를 발생시킨 문자열 값을 가져옵니다. |

## 예제

잘못된 문자를 포함한 XML 파일이 있는 스트림에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // 손상된 기간이 있는 XML을 포함하는 파일을 엽니다.
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

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


