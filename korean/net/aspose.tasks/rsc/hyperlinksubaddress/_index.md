---
title: "Rsc.HyperlinkSubAddress"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 작업과 연결된 하이퍼링크 내 문서의 특정 위치"
type: docs
weight: 340
url: /ko/net/aspose.tasks/rsc/hyperlinksubaddress/
---
## Rsc.HyperlinkSubAddress field

작업과 연결된 하이퍼링크의 문서 내 특정 위치입니다.

```csharp
public static readonly Key<string, RscKey> HyperlinkSubAddress;
```

## 비고

하이퍼링크의 전체 주소(Microsoft Project의 Hyperlink Href)는 HyperlinkAddress와 HyperlinkSubAddress를 연결한 문자열입니다.

## 예제

리소스 하이퍼링크 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Hyperlink, "Click to visit our site");
resource.Set(Rsc.HyperlinkAddress, "https://products.aspose.com");
resource.Set(Rsc.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + resource.Get(Rsc.Hyperlink));
Console.WriteLine("Hyperlink Address: " + resource.Get(Rsc.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + resource.Get(Rsc.HyperlinkSubAddress));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


