---
title: "Project.ExtendedAttributes"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает объект ExtendedAttributeDefinitionCollection. Коллекция определений пользовательских полей расширенных атрибутов, связанных с проектом"
type: docs
weight: 410
url: /ru/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

Получает объект ExtendedAttributeDefinitionCollection. Коллекция определений расширенных атрибутов (пользовательских полей), связанных с проектом.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## Примеры

Показывает, как работать с расширенными атрибутами.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Если пользовательское поле не существует в проекте, создайте его
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Создать расширенный атрибут из определения
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Добавить расширенный атрибут к задаче
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


