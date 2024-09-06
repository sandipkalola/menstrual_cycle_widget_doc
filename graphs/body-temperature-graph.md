# Body temperature graph

<figure><img src="https://raw.githubusercontent.com/sandipkalola/menstrual_cycle_widget_example/main/assets/temp_graph.jpeg" alt="" width="563"><figcaption></figcaption></figure>

A **Body Temperature Graph** for menstrual cycle tracking is often used to visualize **Basal Body Temperature (BBT)** changes throughout the cycle. BBT is the lowest body temperature reached during rest and is typically measured first thing in the morning before any activity. This graph helps track ovulation and hormonal shifts, as body temperature tends to rise after ovulation due to the increase in **progesterone**.

```dart
import 'package:menstrual_cycle_widget/menstrual_cycle_widget.dart';

class MenstrualCycleGraphExample extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Body Temperature Graph'),
      ),
      body: MenstrualBodyTemperatureGraph(
        bodyTemperatureUnits: BodyTemperatureUnits.celsius,
        isShowMoreOptions: true,
        onPdfDownloadCallback: (pdfPath) async {
          // This function will be called when the user downloads an pdf
          // pdfPath contains the path to the downloaded pdf
        },
        onImageDownloadCallback: (imagePath) async {
          // This function will be called when the user downloads an image
          // imagePath contains the path to the downloaded image
        },
      ),
    );
  }
}
```

## Parameter



<table><thead><tr><th width="198">Parameters</th><th width="129">Datatype</th><th width="269">Description</th><th>Default Value</th></tr></thead><tbody><tr><td><code>loadingText</code></td><td>String</td><td>Specify the loading text while fetch data from databse.</td><td>Loading...</td></tr><tr><td><code>bodyTemperatureUnits</code></td><td>BodyTemperatureUnits</td><td>Specify the body temperature units for graph</td><td>celsius</td></tr><tr><td><code>isShowMoreOptions</code></td><td>bool</td><td>Specify as true to show download image and pdf options into right-top of graph.</td><td>false</td></tr><tr><td><code>onImageDownloadCallback</code></td><td>Function</td><td>Callback this function if user download image. It's return a path of the image.</td><td>-</td></tr><tr><td><code>onPdfDownloadCallback</code></td><td>Function</td><td>Callback this function if user download pdf. It's return a path of the image.</td><td>-</td></tr><tr><td><code>xAxisTitle</code></td><td>String</td><td>Specify the title of xAxis</td><td>Body temperature log date</td></tr><tr><td><code>xAxisTitleTextStyle</code></td><td>TextStyle</td><td>Specify the text style of xAxis</td><td>TextStyle(color: Colors.black, fontSize: 10)</td></tr><tr><td><code>isShowXAxisTitle</code></td><td>bool</td><td>Speficy false if want to hide xAxis title </td><td>true</td></tr><tr><td><code>yAxisTitle</code></td><td>String</td><td>Specify the title of yAxis</td><td>Temperature unit</td></tr><tr><td><code>yAxisTitleTextStyle</code></td><td>TextStyle</td><td>Specify the text style of yAxis</td><td>TextStyle(color: Colors.black, fontSize: 10)</td></tr><tr><td><code>isShowYAxisTitle</code></td><td>bool</td><td>Speficy false if want to hide yAxis title </td><td>true</td></tr><tr><td><code>topGraphColor</code></td><td>Color</td><td>Specify top color of bar line</td><td>Colors.red</td></tr><tr><td><code>centerGraphColor</code></td><td>Color</td><td>Specify central color of bar line</td><td>Colors.orange</td></tr><tr><td><code>bottomGraphColor</code></td><td>Color</td><td>Specify bottom color of bar line</td><td>Colors.yellow</td></tr><tr><td><code>tooltipBackgroundColor</code></td><td>Color</td><td>Specify background color of tooltip</td><td>Colors.black</td></tr></tbody></table>

