---
title: "PrintOptions.PrintOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrintOptions 생성자. 프로젝트 인쇄를 위한 다양한 옵션을 설정하는 데 사용할 수 있는 PrintOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

`[`PrintOptions`](../)` 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 프로젝트 인쇄를 위한 다양한 옵션을 설정하는 데 사용할 수 있습니다.

```csharp
public PrintOptions()
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

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


