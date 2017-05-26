#### What can I beemind with Apple Health?
  * steps
  * active energy
  * exercise time
  * weight
  * cycling distance
  * walking/running distance
  * Nike Fuel
  
#### How do I create an Apple Health goal?
First, create a regular, manual-input Beeminder goal [here](https://www.beeminder.com/new).  Make sure the goal type you use is the right one for the metric you want to beemind.  For example, a Do-More goal is the best for steps, but if you want to lose weight, make sure to choose the Weight Loss goal!

Then, open your Beeminder iOS app and refresh the data so that your new goal is found.  From there, tap the settings gear from the main screen of the app.  You’ll now see a line for “Health App integration”.  Tap the goal you just created, and then the metric you want to track.  That will pair the metric to the goal, and it should fetch the last 7 days of data.

#### My Beeminder goal isn't updating even though I have new data!
There's a couple small slightly-weird things about the data sync to check first!
  1. The background update only happens if the phone is unlocked, so try unlocking your phone for a couple minutes if you haven't been actively using it.
  2. The background update isn’t necessarily _immediate_, so you might not see the steps you did two minutes ago reflected on your goal on the website.  If you do want to know your exact up-to-the-minute count, you can always force a fetch of the latest data just by opening the Beeminder app!
