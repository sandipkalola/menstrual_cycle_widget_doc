---
description: >-
  To get the last period date using the function and return it as a DateTime
  object. The last period date is not available. Defaulting to January 1, 1971.
---

# Get last period date



```dart
  final instance = MenstrualCycleWidget.instance!;
  DateTime lastPeriodDate = _instance.getPreviousPeriodDate();
  
  if (lastPeriodDate!.year == 1971) {
    print("No last period date was provided. Returning default date: 1971-01-01.");
  } else {
    print("Last period date is: ${lastPeriodDate!.toLocal()}");
  }
```
