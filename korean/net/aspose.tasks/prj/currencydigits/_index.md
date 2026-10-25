---
title: "Prj.CurrencyDigits"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj field. 소수 기호 뒤의 자릿수"
type: docs
weight: 160
url: /ko/net/aspose.tasks/prj/currencydigits/
---
## Prj.CurrencyDigits field

소수 기호 뒤의 자리수.

```csharp
public static readonly Key<int, PrjKey> CurrencyDigits;
```

## 예제

프로젝트의 통화 속성을 쓰는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// 통화 속성을 설정합니다
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// 통화 속성을 표시합니다
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


