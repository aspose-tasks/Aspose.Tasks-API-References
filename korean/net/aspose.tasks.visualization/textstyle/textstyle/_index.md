---
title: "TextStyle.TextStyle"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TextStyle 생성자. 기본 설정으로 TextStyle 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

기본 설정으로 [`TextStyle`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TextStyle()
```

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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

기본 글꼴과 지정된 글꼴 크기 및 스타일로 [`TextStyle`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fontSize | Single | TextStyle의 글꼴 크기. |
| fontStyle | FontStyles | TextStyle의 글꼴 스타일. |

### 또 보기

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

기본 글꼴과 지정된 글꼴 스타일로 [`TextStyle`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TextStyle(FontStyles fontStyle)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fontStyle | FontStyles | 기본 글꼴에 적용할 글꼴 스타일. |

### 또 보기

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

지정된 글꼴 설정으로 [`TextStyle`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TextStyle(FontDescriptor font)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| font | FontDescriptor | TextStyle의 글꼴. |

### 또 보기

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


