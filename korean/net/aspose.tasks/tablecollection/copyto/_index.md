---
title: "TableCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TableCollection 메서드. 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/tablecollection/copyto/
---
## TableCollection.CopyTo method

이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다.

```csharp
public void CopyTo(Table[] array, int arrayIndex)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 배열 | Table[] | 요소를 복사할 지정된 1차원 배열. |
| arrayIndex | Int32 | 복사가 시작되는 지정된 배열의 0 기반 인덱스. |

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

* class [Table](../../table/)
* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


