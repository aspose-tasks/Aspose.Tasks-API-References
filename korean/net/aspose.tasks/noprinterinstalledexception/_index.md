---
title: "클래스 NoPrinterInstalledException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.NoPrinterInstalledException 클래스. 운영 체제에 설치된 프린터가 없을 때 발생하는 예외를 나타냅니다."
type: docs
weight: 1100
url: /ko/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

OS에 설치된 프린터가 없을 때 발생하는 예외를 나타냅니다.

```csharp
public class NoPrinterInstalledException : Exception
```

## 예제

인쇄 옵션을 사용하는 방법을 보여줍니다.

```csharp
try
{
    var project = new Project(DataDir + "Project2.mpp");
    var options = new PrintOptions
    {
        Timescale = Timescale.ThirdsOfMonths
    };
    if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
    {
        project.Print(options);
    }
}
catch (NoPrinterInstalledException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


