---
title: "Project.CopyTo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। प्रोजेक्ट के मुख्य डेटा और प्रॉपर्टीज़ को दूसरे प्रोजेक्ट में कॉपी करता है"
type: docs
weight: 1060
url: /hi/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

परियोजना के मुख्य डेटा और गुणों को दूसरी परियोजना में कॉपी करता है।

```csharp
public void CopyTo(Project another)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दूसरा | Project | डेटा कॉपी करने के लिए दूसरा प्रोजेक्ट। |

## उदाहरण

दिखाता है कि प्रोजेक्ट डेटा को दूसरे प्रोजेक्ट में कैसे कॉपी किया जाए।

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// सामान्य प्रोजेक्ट डेटा कॉपी करते समय व्यू डेटा की कॉपी को छोड़ें।
project.CopyTo(mppProject);
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

परियोजना के मुख्य डेटा और गुणों को दूसरी परियोजना में कॉपी करता है।

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दूसरा | Project | डेटा कॉपी करने के लिए दूसरा प्रोजेक्ट। |
| विकल्प | CopyToOptions | कॉपी प्रक्रिया को नियंत्रित करने के लिए कॉपी विकल्प। |

## उदाहरण

दिखाता है कि प्रोजेक्ट को &lt;see cref="Aspose.Tasks.CopyToOptions"/&gt; इंस्टेंस का उपयोग करके कैसे कॉपी किया जाए।

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// सामान्य प्रोजेक्ट डेटा कॉपी करते समय व्यू डेटा की कॉपी को छोड़ें।
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### संबंधित देखें

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


