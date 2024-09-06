# Sleep graph



<figure><img src="https://raw.githubusercontent.com/sandipkalola/menstrual_cycle_widget_example/main/assets/sleep_graph.jpeg" alt="" width="563"><figcaption></figcaption></figure>

```dart
class MenstrualCycleGraphExample extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Sleep graph'),
      ),
      body: MenstrualSleepGraph(
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
