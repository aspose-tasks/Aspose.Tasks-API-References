---
title: "Prj.CurrencyCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. ISO 4217에 정의된 세 글자 통화 문자 코드입니다. 유효한 값의 예는 USD입니다."
type: docs
weight: 150
url: /ko/net/aspose.tasks/prj/currencycode/
---
## Prj.CurrencyCode field

ISO 4217에 정의된 세 글자 통화 코드입니다. 유효한 값의 예는 "USD"입니다.

```csharp
public static readonly Key<string, PrjKey> CurrencyCode;
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


