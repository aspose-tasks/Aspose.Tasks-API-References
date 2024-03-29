---
title: ImageSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: परयजन पृष्ठं क छवयं में प्रस्तुत करते समय अतरक्त वकल्प नर्दष्ट करने क अनुमत देत है
type: docs
weight: 1770
url: /hi/net/aspose.tasks.saving/imagesaveoptions/
---
## ImageSaveOptions class

परियोजना पृष्ठों को छवियों में प्रस्तुत करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class ImageSaveOptions : SaveOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFileFormat) | का एक नया उदाहरण प्रारंभ करता है`ImageSaveOptions` वर्ग जिसका उपयोग TIFF, PNG, BMP या JPEG स्वरूपों में प्रदान की गई छवियों को सहेजने के लिए किया जा सकता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | के उदाहरणों की सूची प्राप्त या सेट करता है[`BarStyle`](../../aspose.tasks.visualization/barstyle/) कक्षा जो प्रोजेक्ट व्यू में दिखाई देती है। |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | कस्टम पृष्ठ आकार को अंकों में प्राप्त या सेट करता है (1 बिंदु = 1/72 इंच)। |
| [DefaultFontName](../../aspose.tasks.saving/imagesaveoptions/defaultfontname/) { get; set; } | प्रतिपादन के लिए डिफ़ॉल्ट फ़ॉन्ट प्राप्त या सेट करता है। |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि क्या गैर-कार्य समय निकाला जाना चाहिए (डिफ़ॉल्ट मान TRUE है)। |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | रेंडरिंग समाप्त करने के लिए दिनांक प्राप्त करता है या सेट करता है. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि इसकी सामग्री को फिट करने के लिए पंक्ति की ऊंचाई बढ़ाई जानी चाहिए या नहीं। |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | हो जाता है या सेट करता है कि दृश्य के कैलेंडर अनुभाग को अंतिम पृष्ठ के अंत (दाईं ओर) में प्रस्तुत किया जाना चाहिए या नहीं। यदि मान गलत है, तो कैलेंडर अनुभाग को बिल्कुल एंडडेट पर प्रस्तुत किया जाता है, यहां तक कि पृष्ठ पर एक खाली स्थान भी है। |
| [FontResolveCallback](../../aspose.tasks.saving/imagesaveoptions/fontresolvecallback/) { get; set; } | एक कॉलबैक प्राप्त या सेट करता है जिसका उपयोग हल किए गए फ़ॉन्ट को अनुकूलित करने के लिए किया जा सकता है। |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | इसकी सूची प्राप्त या सेट करता है[`Gridline`](../../aspose.tasks.visualization/gridline/) जो प्रोजेक्ट व्यू में दिखाई देते हैं. |
| [HorizontalResolution](../../aspose.tasks.saving/imagesaveoptions/horizontalresolution/) { get; set; } | dpi. में क्षैतिज रिज़ॉल्यूशन प्राप्त या सेट करता है |
| [JpegQuality](../../aspose.tasks.saving/imagesaveoptions/jpegquality/) { get; set; } | जेपीईजी गुणवत्ता प्राप्त या सेट करता है। अनुमत मान श्रेणी 0..100. है |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि प्रत्येक पृष्ठ पर किंवदंती दिखायी जानी चाहिए (डिफ़ॉल्ट मान TRUE है)। |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि महत्वपूर्ण कार्यों को लाल रंग में प्रदर्शित किया जाना चाहिए (डिफ़ॉल्ट मान FALSE है)। |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | गैर-कार्य समय रंग प्राप्त या सेट करता है। |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | प्रोजेक्ट के पृष्ठों की संख्या प्राप्त या सेट करता है। |
| [Pages](../../aspose.tasks.saving/imagesaveoptions/pages/) { get; set; } | प्रोजेक्ट लेआउट को अलग फाइलों में सहेजते समय सहेजने के लिए पेज नंबरों की एक सूची प्राप्त या सेट करता है। यदि यह सूची खाली है तो सभी पृष्ठ सहेजे जाएँगे। |
| [PageSavingCallback](../../aspose.tasks.saving/imagesaveoptions/pagesavingcallback/) { get; set; } | उपयोगकर्ता परिभाषित कॉलबैक प्राप्त या सेट करता है जिसका उपयोग प्रत्येक प्रस्तुत पृष्ठ के लिए आउटपुट स्ट्रीम प्राप्त करने के लिए किया जाता है। |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | प्रस्तुत किए जाने वाले पृष्ठ के आकार को प्राप्त या सेट करता है (डिफ़ॉल्ट मान PageSize.A4 है)। |
| [PixelFormat](../../aspose.tasks.saving/imagesaveoptions/pixelformat/) { get; set; } | छवि में प्रत्येक पिक्सेल के लिए रंग डेटा का प्रारूप प्राप्त या सेट करता है। |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | हो जाता है या सेट करता है[`PresentationFormat`](../saveoptions/presentationformat/) जिसमें दस्तावेज़ सहेजा जाएगा. |
| [ReduceFooterGap](../../aspose.tasks.saving/imagesaveoptions/reducefootergap/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि अंतिम कार्य और पाद लेख के बीच का अंतर कम होना चाहिए। |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि प्रोजेक्ट को एक पृष्ठ पर रेंडर किया जाना चाहिए या नहीं जब प्रोजेक्ट को ग्राफिकल प्रारूप में सहेजा जाता है। |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि सारांश कार्य पट्टी पर उप-कार्यों को चिह्नित किया जाना चाहिए। फ़ील्ड इंगित करता है कि क्या सारांश टास्क बार रोल अप बार प्रदर्शित करता है। |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | उस प्रारूप को प्राप्त या सेट करता है जिसमें दस्तावेज़ को सहेजा जाएगा यदि यह सेव ऑप्शन ऑब्जेक्ट का उपयोग किया जाता है। |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | रेंडरिंग शुरू करने की तिथि प्राप्त करता है या सेट करता है। |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | गैंट चार्ट और टास्क शीट चार्ट पर कार्यों को सॉर्ट करने के लिए तुलनाकर्ता को प्राप्त या सेट करता है। |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | उस स्थिति को प्राप्त या सेट करता है जिसका उपयोग गैंट, टास्क शीट और टास्क यूसेज चार्ट पर किए गए कार्यों को फ़िल्टर करने के लिए किया जाता है। |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | के उदाहरणों की सूची प्राप्त या सेट करता है[`TextStyle`](../../aspose.tasks.visualization/textstyle/) कक्षा जो प्रोजेक्ट व्यू में दिखाई देती है। |
| [TiffCompression](../../aspose.tasks.saving/imagesaveoptions/tiffcompression/) { get; set; } | टीआईएफएफ प्रारूप में जेनरेट की गई छवियों को सहेजते समय लागू होने वाले संपीड़न के प्रकार को प्राप्त या सेट करता है। |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | हो जाता है या सेट करता है[`Timescale`](../saveoptions/timescale/) मूल्य जिसका उपयोग यह नियंत्रित करने के लिए किया जाता है कि प्रोजेक्ट को ग्राफिकल प्रारूप में सहेजे जाने पर टाइमस्केल (यदि मौजूद है) को कैसे प्रस्तुत किया जाता है। |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | गैंट चार्ट को प्रस्तुत करते समय ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं, यह इंगित करने वाला मान प्राप्त या सेट करता है। |
| [UseProjectDefaultFont](../../aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि प्रतिपादन के लिए डिफ़ॉल्ट फ़ॉन्ट का उपयोग किया जाना चाहिए। |
| [VerticalResolution](../../aspose.tasks.saving/imagesaveoptions/verticalresolution/) { get; set; } | dpi. में लंबवत रिज़ॉल्यूशन प्राप्त या सेट करता है |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | रेंडर करने के लिए व्यू कॉलम की सूची प्राप्त या सेट करता है ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) . यदि सेट नहीं किया गया है तो कार्य आईडी, कार्य नाम, प्रारंभ और समाप्ति केवल प्रदान की जाती है। यदि दोनों देखें और[`ViewSettings`](../saveoptions/viewsettings/)गुण सेट हैं, व्यू से कॉलम ViewSettings. से कॉलम ओवरराइड करता है |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | एक दृश्य प्राप्त करता है या सेट करता है ([`View`](../saveoptions/view/) ) सौंपने के लिए। आप इस विकल्प का उपयोग स्पष्ट रूप से निर्दिष्ट करने के लिए कर सकते हैं कि किस दृश्य को पीडीएफ, एचटीएमएल या छवि प्रारूपों में सहेजा जाना चाहिए। यदि यह संपत्ति सेट है,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) प्रोजेक्‍ट के सहेजे जाने पर गुण को अनदेखा कर दिया जाता है. दृश्‍य निम्‍न में से किसी एक स्‍क्रीन से होना चाहिए (([`Screen`](../../aspose.tasks/view/screen/) )): (गैंट, टास्कशीट, टास्कयूसेज, रिसोर्सशीट, रिसोर्सयूसेज) |

### यह सभी देखें

* class [SaveOptions](../saveoptions/)
* नाम स्थान [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* सभा [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
