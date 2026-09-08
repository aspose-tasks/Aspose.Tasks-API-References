---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraXmlSaveOptions 생성자. PrimaveraXmlSaveOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

[`PrimaveraXmlSaveOptions`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PrimaveraXmlSaveOptions()
```

## 예제

Primavera XML 파일로 내보내는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### 또 보기

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


