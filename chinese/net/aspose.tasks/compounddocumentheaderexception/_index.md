---
title: "类 CompoundDocumentHeaderException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CompoundDocumentHeaderException 类。表示在 MPP 文件的头部损坏时抛出的异常。"
type: docs
weight: 280
url: /zh/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

表示在 MPP 文件头损坏时抛出的异常。

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## 示例

展示如何捕获 &lt;see cref=\"CompoundDocumentHeaderException\" /&gt; 异常。

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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


