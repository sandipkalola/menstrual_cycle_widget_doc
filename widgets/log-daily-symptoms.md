# Log daily symptoms

<div><figure><img src="https://raw.githubusercontent.com/sandipkalola/menstrual_cycle_widget_example/main/assets/log_symptoms2.jpeg" alt="" width="375"><figcaption></figcaption></figure> <figure><img src="https://raw.githubusercontent.com/sandipkalola/menstrual_cycle_widget_example/main/assets/log_symptoms.jpeg" alt="" width="375"><figcaption></figcaption></figure></div>

```dart
MenstrualLogPeriodView(
                displaySymptomsData: DisplaySymptomsData(),
                onError: onError(),
                onSuccess: (int id) {
                  onSuccess();
                },
                symptomsLogDate:
                    DateTime.now().add(Duration(days: next(1, 500))),
            )
```

## Parameter

<table><thead><tr><th>Parameters</th><th width="110">Datatype</th><th width="329">Description</th><th>Default Value</th></tr></thead><tbody><tr><td><code>symptomsLogDate</code></td><td>DateTime</td><td>Specifies the date of symptoms log date</td><td>DateTime.now()</td></tr><tr><td><code>onSuccess</code></td><td>Function</td><td>Call back this function upon successfully storing log data in the local database.</td><td>-</td></tr><tr><td><code>onError</code></td><td>Function</td><td>Call back this function upon error during storing log data in the local database.</td><td>-</td></tr><tr><td><code>isRequiredWaterView</code></td><td>bool</td><td>Set to false to hide the water view.</td><td>true</td></tr><tr><td><code>isRequiredBodyTemperatureView</code></td><td>bool</td><td>Set to false to hide the body temperture view.</td><td>true</td></tr><tr><td><code>isRequiredWeightView</code></td><td>bool</td><td>Set to false to hide the weight view.</td><td>true</td></tr><tr><td><code>isRequiredSleepView</code></td><td>bool</td><td>Set to false to hide the sleep view.</td><td>true</td></tr><tr><td><code>isShowCustomSymptomsOnly</code></td><td>bool</td><td>Set to true to show only custom symptoms list.</td><td>false</td></tr><tr><td><code>isRequiredMeditationView</code></td><td>bool</td><td>Set to false to hide the meditation view.</td><td>true</td></tr><tr><td><code>displaySymptomsData</code></td><td>DisplaySymptomsData</td><td>Set to false in the specific object to hide it from the symptoms view</td><td></td></tr></tbody></table>
