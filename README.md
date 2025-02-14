# NSDateFormatter Locale Issue: Inconsistent Date Parsing Across Locale Changes

This repository demonstrates an uncommon bug in Objective-C related to `NSDateFormatter`'s handling of locale changes.  The provided code showcases how inconsistent date parsing can occur if the application's locale is changed during runtime without explicitly managing the date formatter's locale settings.

The `DateformatterBug.m` file contains the buggy code.  `DateformatterBugSolution.m` provides a corrected version that handles locale changes appropriately by explicitly setting the locale for the `NSDateFormatter` instance.  The solution ensures consistent date parsing and formatting regardless of locale changes.

This issue highlights the importance of explicitly setting the locale for date formatters, especially in applications where the locale might change dynamically.