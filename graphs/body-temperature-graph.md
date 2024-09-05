# Body temperature graph

<figure><img src="https://raw.githubusercontent.com/sandipkalola/menstrual_cycle_widget_example/main/assets/temp_graph.jpeg" alt="" width="563"><figcaption></figcaption></figure>

A **Body Temperature Graph** for menstrual cycle tracking is often used to visualize **Basal Body Temperature (BBT)** changes throughout the cycle. BBT is the lowest body temperature reached during rest and is typically measured first thing in the morning before any activity. This graph helps track ovulation and hormonal shifts, as body temperature tends to rise after ovulation due to the increase in **progesterone**.

```dart
import 'package:menstrual_cycle_widget/menstrual_cycle_widget.dart';

class MenstrualCyclePage extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Body Temperature Graph'),
      ),
      body: MenstrualBodyTemperatureGraph(
        bodyTemperatureUnits: BodyTemperatureUnits.celsius,
        isShowMoreOptions: true,
        onDownloadPdfPath: (file) async {},
        onDownloadImagePath: (file) async {},
      ),
    );
  }
}
```

## Parameter

