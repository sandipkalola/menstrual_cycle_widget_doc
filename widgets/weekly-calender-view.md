# Weekly calender view

<figure><img src="https://raw.githubusercontent.com/sandipkalola/menstrual_cycle_widget_example/main/assets/week.jpeg" alt=""><figcaption></figcaption></figure>

```dart
import 'package:menstrual_cycle_widget/menstrual_cycle_widget.dart';

class CalenderExample extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Calender View'),
      ),
      body: MenstrualCycleCalenderView(
        themeColor: Colors.black,
        daySelectedColor: Colors.blue,
        logPeriodText: "Log Period",
        backgroundColorCode: "FFFFFF",
        hideInfoView: false,
        onDateSelected: (date) {},
        onDataChanged: (value) {},
        hideBottomBar: false,
        hideLogPeriodButton: false,
        isExpanded: false,
      ),
    );
  }
}
    
```

## Parameter

<table><thead><tr><th>Parameters</th><th width="110">Datatype</th><th width="329">Description</th><th>Default Value</th></tr></thead><tbody><tr><td><code>themeColor</code></td><td>Color</td><td>Specifies the theme color to match the app’s style</td><td>Colors.black</td></tr><tr><td><code>daySelectedColor</code></td><td>Color</td><td>Specifies the selected day color.</td><td>Colors.grey</td></tr><tr><td><code>hideInfoView</code></td><td>bool</td><td>Set true to hide information view. </td><td>false</td></tr><tr><td><code>onDataChanged</code></td><td>Function</td><td>Callback this function if change any data into calender view.</td><td>-</td></tr><tr><td><code>isShowCloseIcon</code></td><td>bool</td><td>Set true to show (X) close icon on top left side of calender view. </td><td>false</td></tr><tr><td><code>onDataSelected</code></td><td>Function</td><td>Callback this function if select any date into calender view.</td><td>-</td></tr><tr><td><code>isExpanded</code></td><td>bool</td><td>Set true to show full month calender view.</td><td>false</td></tr><tr><td><code>hideBottomBar</code></td><td>bool</td><td>Set true to hide bottom bar of calender view </td><td>false</td></tr><tr><td><code>hideLogPeriodButton</code></td><td>bool</td><td>Set true to hide button of "Log Period".</td><td>false</td></tr><tr><td><code>logPeriodText</code></td><td>String</td><td>Specify the text of log period button. </td><td>Log Period</td></tr><tr><td><code>backgroundColorCode</code></td><td>Color</td><td>Specify the background color of calender view</td><td>Colors.white</td></tr></tbody></table>

