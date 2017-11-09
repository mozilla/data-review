# Appendix

This document contains additional information that data requesters and stewards may reference when either requesting or performing a review.

## Documentation.

All data collection should have documentation that is available publicly.  This is separate from the privacy notice, which should provide simple to understand language and will often link to the documentation. The purpose of of this documentation is to provide the details for those users who really want to dig in and understand the privacy risk of the data.

Documentation should describe the schema for the ultimate data, including explanatory text for each field. It should also describe how long the data will be retained. To keep this as up to date and accurate as possible, we advise keeping this data documentation with the rest of the source code (e.g. projects on Github should use Github for data documentation).

Here are three different examples:

* [Firefox Telemetry](http://gecko.readthedocs.io/en/latest/toolkit/components/telemetry/telemetry/data/main-ping.html).

* [Test Pilot’s Activity Stream experiment](https://github.com/mozilla/activity-stream/blob/master/docs/data_dictionary.md).

* Data collection for Firefox Focus, [describing](https://github.com/mozilla-mobile/focus/wiki/Install-and-event-tracking-with-the-Adjust-SDK) data sent to our third-party analytics provider.

## Control Mechanism.

For any data collection mechanism, we want to provide a way for the user to turn on and off the collection. For example, our users can turn off Firefox telemetry and crash reporting in the Firefox preferences (see [here](https://support.mozilla.org/t5/Manage-preferences-and-add-ons/Share-telemetry-data-with-Mozilla-to-help-improve-Firefox/ta-p/7803)). We make an security features where the collection provides an immediate benefit to the user and where allowing the user to turn off the collection would place her/him at greater risk.

## Identifiers.

Identifier refers here to a string of numbers or characters that is tied to a unique user or the user’s device. We are using this term broadly to include identifiers that can be used to identify a specific person (such as a name ) as well as random identifiers.  This includes things like:

* Email address

* Names or Usernames

* Social Security Numbers

* A device Fingerprints

* Randomly Generated IDs

* A hash of of the above.

For any data collection tool, we want to call out and and discuss the use of any new identifiers. This is because inclusion of a new identifier often changes the privacy properties of the system, either by making the data more identifiable or by allowing us to combine disparate data sets into a larger user profile. We want to avoid both of those if possible.

For example, Firefox Telemetry includes a clientID that is used to identify the data from specific users. However, we have attempted to keep Firefox telemetry as de-identified as possible and avoided collecting sensitive data in telemetry that could be used to identify a specific person. We have similarly avoided adding the Firefox Account ID or any identifier associated with Firefox Accounts because inclusion of that ID would mean we could easily tie all telemetry data back to a specific person.
