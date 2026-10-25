---
title: "클래스 CompoundDocumentHeaderException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CompoundDocumentHeaderException 클래스. MPP 파일 헤더가 손상될 때 발생하는 예외를 나타냅니다."
type: docs
weight: 280
url: /ko/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

MPP 파일 헤더가 손상되었을 때 발생하는 예외를 나타냅니다.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## 예제

예외를 포착하는 방법을 보여줍니다 &lt;see cref=\"CompoundDocumentHeaderException\" /&gt; 예외.

```csharp
try
{
    var project = new Project(DataDir + "Project1.mpp");

    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (CompoundDocumentHeaderException e)
{
    Console.WriteLine(e.Message);
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


