---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraXmlSaveOptions 속성. 루트 작업을 저장할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

루트 작업을 저장할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool SaveRootTask { get; set; }
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


