---
title: "Table.TableFields"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Table 속성. 테이블의 필드를 나타내는 TableFields 컬렉션을 가져옵니다."
type: docs
weight: 90
url: /ko/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

테이블의 필드를 나타내는 TableFields 컬렉션을 가져옵니다.

```csharp
public TableFieldCollection TableFields { get; }
```

## 예제

프로젝트 테이블 작업 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// 새 사용자 지정 속성을 정의합니다.
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// 생성된 작업에 사용자 지정 텍스트 속성을 추가합니다.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// 텍스트 속성 필드를 추가하여 테이블을 사용자 정의합니다
var field = new TableField();
field.Field = Field.TaskText1;
field.Width = 20;
field.Title = "Custom attribute";
field.AlignTitle = HorizontalStringAlignment.Center;
field.AlignData = HorizontalStringAlignment.Center;

var table = project.Tables.ToList()[0];
table.TableFields.Insert(3, field);

project.Save(OutDir + "ConfigureGanttChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### 또 보기

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


