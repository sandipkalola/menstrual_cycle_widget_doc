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

## Parameter

<table><thead><tr><th width="198">Parameters</th><th width="129">Datatype</th><th width="269">Description</th><th>Default Value</th></tr></thead><tbody><tr><td><code>loadingText</code></td><td>String</td><td>Specify the loading text while fetch data from databse.</td><td>Loading...</td></tr><tr><td><code>headerTitle</code></td><td>String</td><td>Specify the header title</td><td>Cycle History</td></tr><tr><td><code>headerTitleTextStyle</code></td><td>TextStyle</td><td>Specify the text style of yAxis</td><td>TextStyle(color: Colors.black, fontSize: 10)</td></tr><tr><td><code>viewCycleHistoryLength</code></td><td>int</td><td>Speficy the length of cycle history which you want to show</td><td>3</td></tr><tr><td><code>appBarBackgroundColor</code></td><td>Color</td><td>Specify the title bar color of AppBar</td><td>Colors.blueAccent</td></tr></tbody></table>
