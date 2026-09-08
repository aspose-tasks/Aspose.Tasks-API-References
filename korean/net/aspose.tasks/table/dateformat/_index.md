---
title: "Table.DateFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Table 속성. 테이블의 날짜 형식을 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/table/dateformat/
---
## Table.DateFormat property

테이블의 날짜 형식을 가져오거나 설정합니다.

```csharp
public DateFormat DateFormat { get; set; }
```

## 예제

새 테이블을 정의하는 방법을 보여줍니다 (뷰에 사용).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// 편집할 테이블을 가져옵니다
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// 몇몇 속성을 조정합니다
// 테이블의 머리글 행 높이를 조정할 수 있는지 여부를 나타내는 값을 설정합니다
table.AdjustHeaderRowHeight = true;

// 테이블의 날짜 형식을 설정합니다.
table.DateFormat = DateFormat.DateDdMmYyyy;

// 테이블의 첫 번째 열이 잠겨 있는지 또는 편집 가능한지 여부를 나타내는 값을 설정합니다
table.LockFirstColumn = true;

// 테이블에서 행 높이를 설정합니다. 여기서 행 높이는 텍스트 줄 수를 의미합니다
table.RowHeight = 10;

// '새 열 추가' 인터페이스를 표시할지 여부를 나타내는 값을 설정합니다
table.ShowAddNewColumn = true;

// 프로젝트가 리본의 보기 탭에 있는 테이블 드롭다운 목록에 테이블 이름을 표시할지 여부를 나타내는 값을 설정합니다
table.ShowInMenu = true;

// 업데이트된 테이블을 저장합니다
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* enum [DateFormat](../../dateformat/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


