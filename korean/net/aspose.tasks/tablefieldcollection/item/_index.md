---
title: "TableFieldCollection.Item"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TableFieldCollection 속성. 지정된 인덱스의 요소를 반환하거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/tablefieldcollection/item/
---
## TableFieldCollection indexer

지정된 인덱스에 있는 요소를 반환하거나 설정합니다.

```csharp
public TableField this[int index] { get; set; }
```

| 매개변수 | 설명 |
| --- | --- |
| 인덱스 | 가져오거나 설정할 요소의 0부터 시작하는 인덱스. |

### 반환 값

지정된 인덱스의 요소.

## 예제

테이블 필드 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // 테이블 필드를 반복합니다
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// 새 테이블 필드를 추가합니다
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// 해당 위치에 새 필드를 삽입합니다
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// 인덱스 접근을 사용하여 새 테이블 필드를 편집합니다
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// 최근에 필드를 제거할 수 있습니다
table.TableFields.RemoveAt(idx);

// 컬렉션을 두 가지 방법으로 정리할 수 있습니다
if (deleteOneByOne)
{
    // 테이블 필드를 배열에 복사하고 하나씩 삭제합니다
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // 또는 테이블 필드 컬렉션을 완전히 비울 수 있습니다
    table.TableFields.Clear();
}
```

### 또 보기

* class [TableField](../../tablefield/)
* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)


