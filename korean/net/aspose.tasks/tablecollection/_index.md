---
title: "클래스 TableCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TableCollection 클래스. Table 객체 목록을 포함합니다. ICollectionTable 인터페이스를 구현합니다."
type: docs
weight: 2330
url: /ko/net/aspose.tasks/tablecollection/
---
## TableCollection class

[`Table`](../table/) 객체 목록을 포함합니다. ICollection&lt;Table&gt; 인터페이스를 구현합니다.

```csharp
public class TableCollection : ICollection<Table>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | 테이블 컬렉션을 [`Table`](../table/) 객체 목록으로 변환합니다. |

## 예제

테이블 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// 테이블을 반복합니다
Console.WriteLine("Print tables of " + project.Get(Prj.Name) + " project.");
Console.WriteLine("Table count: " + project.Tables.Count);
foreach (var tbl in project.Tables)
{
    Console.WriteLine("Name: " + tbl.Name);

    Console.WriteLine("Fields:");

    foreach (var field in tbl.TableFields)
    {
        Console.WriteLine("    {0} - '{1}' - {2}", field.Field, field.Title, field.Width);
    }
}

// 새 테이블을 추가합니다
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// 컬렉션을 두 가지 방법으로 정리할 수 있습니다
if (deleteOneByOne)
{
    // 테이블을 배열에 복사하고 하나씩 삭제합니다
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // 또는 테이블 컬렉션을 완전히 정리할 수 있습니다
    project.Tables.Clear();
}

// 컬렉션을 일반 테이블 목록으로 변환할 수 있습니다
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### 또 보기

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


