# Data Review Form (to be filled by Data Stewards)

Instructions: Data Stewards will review a request for data collection and endorse responses to each question. **If the request does not provide answers to questions, reviewers give an r- and point to the questions that can’t be answered.**

1) Is there or will there be **documentation** that describes the schema for the ultimate data set in a public, complete, and accurate way? Click the documentation link provided in Q6 and ensure it is publicly accessible and does or will contain documentation for the data collection. (see [here](https://github.com/mozilla/activity-stream/blob/master/docs/v2-system-addon/data_dictionary.md), [here](https://github.com/mozilla-mobile/focus/wiki/Install-and-event-tracking-with-the-Adjust-SDK), and [here](https://firefox-source-docs.mozilla.org/toolkit/components/telemetry/telemetry/index.html) for examples).  Refer to the appendix for "documentation" if more detail about documentation standards is needed.

2) Is there a control mechanism that allows the user to turn the data collection on and off? (Note, for data collection not needed for security purposes, Mozilla provides such a control mechanism) Provide details as to the control mechanism available.

If the answer to either of the first two questions is no, reviewers give an r-. **Incremental changes to measurements or systems that have previously gone through analysis review may not require additional review.**

3) If the request is for permanent data collection, is there someone who will monitor the data over time?

4) Using the **[category system of data types](https://wiki.mozilla.org/Data_Collection)** on the Mozilla wiki, what collection type of data do the requested measurements fall under?

5) Is the data collection request for default-on or default-off?

6) Does the instrumentation include the addition of **any *new* identifiers** (whether anonymous or otherwise; e.g., username, random IDs, etc.  See the appendix for more details)?

7) Is the data collection covered by the existing Firefox privacy notice? **If unsure: escalate to legal if:**

* The data includes new identifiers; OR

* The data falls within the Web activity category AND is default-on.

8) Does the data collection use a third-party collection tool? **If yes, escalate to legal.**
