---
title: "Sınıf OleObjectCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.OleObjectCollection sınıfı. OleObject sınıfının örneklerini içeren bir koleksiyonu temsil eder."
type: docs
weight: 1130
url: /tr/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

[`OleObject`](../oleobject/) sınıfının örneklerini içeren bir koleksiyonu temsil eder.

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | Koleksiyonu temizler. Bu değişiklikleri kalıcı hale getirmek için project.Save, yeni MPPSaveOptions { WriteViewData = true; } ile çağrılmalıdır. |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | `OleObjectCollection` sınıfının örneğini, [`OleObject`](../oleobject/) sınıfının örneklerini içeren bir listeye dönüştürür. |

## Örnekler

OLE nesnelerinin koleksiyonuyla nasıl çalışılacağını gösterir.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// indeks erişimi kullanarak
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// veya sayım, OLE nesneleri üzerinde yineleme yapılabilir
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


