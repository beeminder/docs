Weight Loss and Weight Gain goals are incredibly simple: enter your weight every day, which should be going down (or going up) over time.  

#### I reached my goal weight!  Can I keep the goal going, but switch to maintaining?
Awesome, and absolutely!  Set a goal date and the goal rate to 0 to flatten out the road until the goal ends.

#### Can I set a goal that keeps me within a certain range?
No.  The Weight Loss goal sets a daily maximum; the Weight Gain goal sets a daily minimum.  If you want to stay within a range of values, you could use one of each goal to enforce both limits.  But most people care about one side of the range far more than the other, so they beemind that goal accordingly.

#### Can I hide the numbers on my graph?  I want to show it off, but I want to hide my true weight value.
We built a feature just for this use case!  In the graph settings, tick the 'Hide the numbers on the y-axis of the graph' box and click the 'Update Graph' button.  This will remove all datapoint values from your publicly-accessible goal page, so you can share it without sharing *everything*.

#### The number shown on my countdown doesn't seem to make sense when I look at my graph.
#### My countdown color is different than my datapoint colors.
TL;DR: We built a lot of crazy complicated rules for weight goals that usually are more confusing than valuable, and we're going to deprecate them someday.

Longer explanation:
On weight goals, the countdown value shown counts down to when the goal changes lanes, rather than when the goal derails.  The datapoints get colored differently on the graph based on the lane they're in.  If you're on the good side of the road (blue or green datapoints), the countdown value will bee counting down toward the date when your datapoints would fall on the *bad* side of the road (orange or red).  If nothing changes before the countdown expires, your latest datapoint would cross into the *bad* lane.  The countdown would actually *go up* at that point, but now it'd be counting down to when you *actually* derail (switching lanes into the red *off the road* territory!).

Isn't that terrible?  

#### I was safe yesterday, but after weighing in today, I immediately derailed?
#### I was on the good side of the road yesterday, and today I had a *crazy* high weigh-in, and now my road is super wide?
TL;DR: We built a lot of crazy complicated rules for weight goals that usually are more confusing than valuable, and we're going to deprecate them someday.

Longer explanation:
The width of the road is dynamic for weight loss goals, and is calculated based off of all your previous data.  Adding a new datapoint can change the road width, which might trigger an insta-derailment.  

The reason it auto-updates is to account for Unexplained Unexpected Weight Fluctuations<sup>TM</sup>.  If you've been doing well on your weight loss goal and staying below the road, it feels unfair to penalize you for having a randomly high weigh-in that throws you above the road, so we wrote a lot of code to prevent that.  *But* you only get that exception when you've weighed in two days in a row (e.g. yesterday was great, today was awful), to incentivize people to actually weigh in daily rather than avoid the scale.  *But* it was all undocumented except through arcane [blog posts](http://blog.beeminder.com/tag/weight-loss/) and email threads with support when you got surprised or stung by this secret beehavior.

Isn't that terrible?
