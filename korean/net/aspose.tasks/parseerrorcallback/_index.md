---
title: "대리자 ParseErrorCallback"
second_title: "Aspose.Tasks for .NET API 참조"
description: "XML 데이터를 읽을 때 발생할 수 있는 구문 분석 오류를 처리하기 위한 메서드 콜백을 나타냅니다."
type: docs
weight: 1250
url: /ko/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

XML 데이터를 읽을 때 발생할 수 있는 구문 분석 오류를 처리하기 위한 메서드 콜백을 나타냅니다.

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| sender | Object | 구문 분석 오류의 원본 객체입니다. |
| args | ParseErrorArgs | 이벤트 데이터를 포함하는 [`ParseErrorArgs`](../parseerrorargs/) 클래스의 인스턴스입니다. |

### 반환 값

지정된 sender 객체에 설정할 강제 변환된 값입니다.

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


