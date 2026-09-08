---
title: "TableField.WrapText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TableField 속성. 열 텍스트가 여러 줄로 자동 줄바꿈될 수 있는지, 열 너비를 초과하면 잘릴지 여부를 나타내는 값을 가져오거나 설정합니다. MSP 2010 버전 이후에서 지원됩니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/tablefield/wraptext/
---
## TableField.WrapText property

열 텍스트가 여러 줄로 자동 줄바꿈될 수 있는지, 또는 열 너비를 초과할 경우 잘려야 하는지를 나타내는 값을 가져오거나 설정합니다. MSP 2010 버전 및 이후 버전에서 지원됩니다.

```csharp
public bool WrapText { get; set; }
```

## 예제

프로젝트 테이블을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// 테이블을 가져옵니다.
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// 모든 테이블 필드 정보를 표시합니다.
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### 또 보기

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


