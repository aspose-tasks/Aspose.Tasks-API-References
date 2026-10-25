---
title: "Table 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Table 클래스. Project 내의 테이블을 나타냅니다."
type: docs
weight: 2320
url: /ko/net/aspose.tasks/table/
---
## Table class

Project의 테이블을 나타냅니다.

```csharp
public class Table
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Table](table/)() | `Table` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | 테이블의 헤더 행 높이를 조정할 수 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | 테이블의 날짜 형식을 가져오거나 설정합니다. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | 테이블의 첫 번째 열이 잠겨 있는지 또는 편집 가능한지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Table 객체의 이름을 가져오거나 설정합니다. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | 테이블의 행 높이를 가져오거나 설정합니다. 여기서 행 높이는 텍스트 줄 수를 의미합니다. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | '새 열 추가' 인터페이스를 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. MSP 2010 버전 이후에서 지원됩니다. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | 프로젝트가 리본의 보기 탭에 있는 Tables 드롭다운 목록에 테이블 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | 테이블의 필드를 나타내는 TableFields 컬렉션을 가져옵니다. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | 지정된 테이블에 대한 테이블 유형을 가져오거나 설정합니다. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | 테이블의 고유 식별자를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | 이 테이블에 대한 해시 코드를 반환합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


