---
description: To use this plugins, follow below steps
---

# How to Use

1.  #### Installation <a href="#id-1-installation" id="id-1-installation"></a>

    Add this to your package's `pubspec.yaml` file:

```dart

dependencies:
  menstrual_cycle_widget: <latest_version>

```

2.  #### Install it <a href="#id-2-install-it" id="id-2-install-it"></a>

    You can install packages from the command line:

```dart
$ flutter packages get
```

3. #### Configuration <a href="#id-3-configuration" id="id-3-configuration"></a>
   1.  **Initialization**

       `MenstrualCycleWidget.init(secretKey: "<Your Secrey Key>", ivKey: "<Your ivKey>");`must be called before using the package:



       **For Example:**

       ```dart
       void main() {
         WidgetsFlutterBinding.ensureInitialized();
         // Make sure to add the required packages to pubspec.yaml:
         // * https://pub.dev/packages/menstrual_cycle_widget
         MenstrualCycleWidget.init(secretKey: "11a1215l0119a140409p0919", ivKey: "23a1dfr5lyhd9a1404845001");
         runApp(const MyApp());
       }
       ```


   2.  **Create a instance of `MenstrualCycleWidget`**

       This instance is use to update your configuration as well to access other functions of this package.



       ```dart
         final instance = MenstrualCycleWidget.instance!;
       ```


   3.  **Update configuration**

       Use `updateConfiguration` method to update your configuration.



       **For Example**

       ```dart
       instance.updateConfiguration(cycleLength: 28, periodDuration: 5, userId: "1");
       ```



<table><thead><tr><th width="202">Parameters</th><th width="120">Datatype</th><th width="288">Description</th><th align="center">Default Value</th></tr></thead><tbody><tr><td><code>cycleLength</code></td><td>int</td><td><strong>Required</strong>. Specifies the total number of cycle days in the menstrual cycle</td><td align="center">required*</td></tr><tr><td><code>periodDuration</code></td><td>int</td><td><strong>Required</strong>. Specifies the total number of period duration in the menstrual cycle</td><td align="center">required*</td></tr><tr><td><code>customerId</code></td><td>String</td><td>Specifies the user id to store data.</td><td align="center">0(Zero)</td></tr><tr><td><code>lastPeriodDate</code></td><td>DateTime</td><td>Specifies the last period date.</td><td align="center">Null</td></tr><tr><td><code>isClearData</code></td><td>bool</td><td>Specifies true if you want to clear past data</td><td align="center">false</td></tr><tr><td><code>defaultLanguage</code></td><td>Languages</td><td>Specifies the language which you want to use for widget.</td><td align="center">english</td></tr><tr><td><code>fontFamily</code></td><td>String</td><td>Specifies the font name.</td><td align="center"></td></tr></tbody></table>
