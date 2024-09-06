# Cycle history graph

<figure><img src="https://raw.githubusercontent.com/sandipkalola/menstrual_cycle_widget_example/main/assets/cycle_history.jpeg" alt="" width="563"><figcaption></figcaption></figure>

A **Cycle History Graph** is a visual representation that shows a user’s menstrual cycle patterns over an extended period, often spanning several months or even years. This graph is used to identify long-term trends in cycle length and period duration.

```dart
import 'package:menstrual_cycle_widget/menstrual_cycle_widget.dart';

class MenstrualCycleGraphExample extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Cycle history graph'),
      ),
      body: MenstrualCycleHistoryGraph(),
    );
  }
}
```

