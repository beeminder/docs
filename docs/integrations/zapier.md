#### What can I beemind with Zapier?
Possibly literally (maybe not literally) *anything*.  They have hundreds of different channels you can use to send information to a Beeminder goal.  If the app you want isn't supported, you might be able to use its notifications, emails, or digests as the trigger instead.

#### How do I make a Zapier goal?
First, you'll want to bee sure you know what type of data Zapier will send - this has implications on the Beeminder goal type you want to use.  Do More and Do Less goals are by far the most common, but there are use cases for the other types as well.

Then create that type of Beeminder goal, and pick that goal to receive the Zapier action.

Once your zap is set up, Beeminder should receive a datapoint the next time your trigger is... triggered.

#### Can I start sending Zapier data to an existing goal?
Probably!  If the existing goal is already using a Beeminder autodata integration, contact support first so we can remove the current configuration.

If your existing goal has a different type than the one you want to use with Zapier, it may not be possible to convert the goal cleanly and retain its history.  It's most likely simpler to start a new goal, but you can contact support to check.

#### Why can't I enter manual data on the website anymore?
When we first receive a datapoint from Zapier, we change the 'Data Source' in your goal settings to indicate that it's been picked up as a Zapier goal.  Removing the entry boxes on the site makes it a little more difficult to enter non-automatic datapoints... since they should be coming only from your Zapier zap... right?

However, if you don't like this setting, or if your zap fails to run and you need to input missing information, you can switch that setting back to 'Manual' and the entry boxes will appear again.  (And we won't switch it back on you anymore!)

#### I did my goal right before the deadline, but Zapier sent my data too late and I derailed.
Not legit, it happens, contact us in support and we'll fix it.  

#### Beeminder isn't showing any of my data.
Check the task history in your Zapier dashboard to bee sure that the trigger is being recognized and acted on appropriately.  We receive data from Zapier; if we don't receive anything, we don't know that there's been a problem!  (TODO: is there an ifttt bzzt equivalent) 
