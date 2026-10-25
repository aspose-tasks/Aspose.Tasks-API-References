---
title: "열거형 BackgroundPattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.BackgroundPattern enum. 배경 패턴을 지정합니다"
type: docs
weight: 100
url: /ko/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

배경 패턴을 지정합니다.

```csharp
public enum BackgroundPattern
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | 어두운 대각선 왼쪽 배경 패턴을 나타냅니다. |
| DarkDiagonalRight | `8` | 어두운 대각선 오른쪽 배경 패턴을 나타냅니다. |
| DarkDither | `13` | 어두운 디더 배경 패턴을 나타냅니다. |
| DarkFill | `4` | 어두운 채우기 배경 패턴을 나타냅니다. |
| DiagonalLeft | `5` | 대각선 왼쪽 배경 패턴을 나타냅니다. |
| DiagonalRight | `6` | 대각선 오른쪽 배경 패턴을 나타냅니다. |
| Hollow | `0` | 속이 빈 배경 패턴을 나타냅니다. |
| LightDither | `11` | 가벼운 디더 배경 패턴을 나타냅니다. |
| LightFill | `2` | 가벼운 채우기 배경 패턴을 나타냅니다. |
| MediumDither | `12` | 중간 디더 배경 패턴을 나타냅니다. |
| MediumFill | `3` | 중간 채우기 배경 패턴을 나타냅니다. |
| MediumVerticalStripe | `10` | 중간 수직 스트라이프 배경 패턴을 나타냅니다. |
| SolidFill | `1` | 단색 채우기 배경 패턴을 나타냅니다. |
| ThinVerticalStripe | `9` | 얇은 수직 스트라이프 배경 패턴을 나타냅니다. |

## 예제

프로젝트에서 다양한 텍스트 항목을 스타일링하는 데 사용되는 텍스트 스타일을 사용자 정의하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


