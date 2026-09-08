---
title: "LoadOptions.Encoding"
second_title: "Aspose.Tasks for .NET API 참조"
description: "LoadOptions 속성. 프로젝트를 HTML, MPX, XER 및 Primavera XML 형식에서 읽는 데 사용되는 인코딩을 가져오거나 설정합니다. 기본 인코딩은 UTF8입니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

HTML, MPX, XER 및 Primavera XML 형식에서 프로젝트를 읽는 데 사용되는 인코딩을 가져오거나 설정합니다. 기본 인코딩은 UTF8입니다.

```csharp
public Encoding Encoding { get; set; }
```

## 예제

Primavera XER 파일에서 프로젝트를 열 때 인코딩을 지정하는 방법을 보여줍니다.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### 또 보기

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


