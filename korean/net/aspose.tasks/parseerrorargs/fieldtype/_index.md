---
title: "ParseErrorArgs.FieldType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ParseErrorArgs 속성. 객체 필드 유형을 가져옵니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/parseerrorargs/fieldtype/
---
## ParseErrorArgs.FieldType property

객체 필드 유형을 가져옵니다.

```csharp
public Type FieldType { get; }
```

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

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


