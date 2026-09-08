---
title: "Project.Tables"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. Table 객체 목록을 가져옵니다"
type: docs
weight: 900
url: /ko/net/aspose.tasks/project/tables/
---
## Project.Tables property

[`Table`](../../table/) 객체 목록을 가져옵니다.

```csharp
public TableCollection Tables { get; }
```

## 예제

Gantt Chart 속성을 구성하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // 새 사용자 지정 속성을 정의합니다.
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // 생성된 작업에 사용자 지정 텍스트 속성을 추가합니다.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // 텍스트 속성 필드를 추가하여 테이블을 사용자 정의합니다
    var field = new TableField
    {
        Field = Field.TaskText1,
        Width = 20,
        Title = "Custom attribute",
        AlignTitle = HorizontalStringAlignment.Center,
        AlignData = HorizontalStringAlignment.Center
    };

    var table = project.Tables.ToList()[0];
    table.TableFields.Insert(3, field);

    project.Save(OutDir + @"ConfigureGantChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
}
catch (NotSupportedException ex)
{
    Console.WriteLine(
        ex.Message
        + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http:// Www.aspose.com/purchase/default.aspx.");
}
```

### 또 보기

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


