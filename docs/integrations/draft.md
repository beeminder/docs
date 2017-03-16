#### What can I beemind with Draft?
The Draft integration tracks your words **edited** each day.  This includes words written as well as words deleted.

#### I've written words in Draft, but Beeminder isn't picking them up.
Usually this happens when you've copied & pasted text from another application directly into Draft.  Those words normally don't get counted as part of your writing for the day.

There is a workaround, however!  If you open the document, start typing a few words, and *then* paste your text, it will count normally, and Beeminder should pick it up.

#### My Draft writing is showing up on the wrong day in Beeminder.
Check your timezones!  If they don't align between Beeminder and Draft, data may get assigned to the wrong day.

#### I edited my datapoint in Beeminder, but it was changed back!
(TODO: confirm this) When Beeminder checks for data, we'll look at the last 7 days of Draft data and update any datapoints that are out of sync with Draft.  
