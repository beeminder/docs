#### What can I beemind with RescueTime?
You can choose to Do More or Do Less of Productive or Unproductive Time.  You can also choose to track a specific category, subcategory, or activity (e.g. facebook.com).  

FocusTime sessions are not available right now, but you can use [IFTTT](https://ifttt.com/rescuetime) to send them to a non-RescueTime-connected Beeminder goal!

#### Why can't I change my deadline from midnight?
RescueTime's API delivers data in day-level chunks, so we can't slice it up on our end to apply it to different Beeminder days.  

#### Can I just change my timezone instead?
Not really.  Even if Beeminder waits until 2am to call your goal derailed, RescueTime is not going to count the time you spent between midnight and 2am for the previous day.  Instead of derailing at midnight, you'll just derail 2 hours later with the same datapoint.

The same applies for pushing the deadline forward.  Beeminder might derail you at 5pm, but you could technically still keep working after the deadline to sync more data, ruining the point of having the 5pm deadline in the first place!

#### I was working late and I derailed because my data didn't sync in time.
This can definitely happen, if you're getting the last minutes done immediately before midnight.  It can take 15-30 minutes for the data to make its way from your computer to RescueTime to Beeminder.  Just reply to the legitimacy check and let us know the derailment was not legit and we'll fix it!

#### I edited some Beeminder datapoints and they all got changed back.
When Beeminder checks for data, we'll look at the last 7 days of RescueTime data and update any datapoints that are out of sync with RescueTime.  

#### My activities aren't getting categorized correctly.
You'll need to change this in RescueTime itself, obviously!  But because of the 7-day lookback, Beeminder will refresh any datapoints in the last week that changed once the new categorizations were made.

#### I restarted my RescueTime goal and immediately derailed.
Definitely not legit; contact support!  This usually happens on Do Less goals, when the first 7-day lookback adds more data than we were anticipating, sending you over the restarted road value.
