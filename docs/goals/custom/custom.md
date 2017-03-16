Custom goals let you create your own goal type by adjusting many of the back-end goal settings.  All of the default goal types are just specific combinations of the settings.  So if you've always wanted an Odometer goal that makes you stay *below* it rather than above it, a custom goal is the right answer!  

#### When should I use a custom goal?
If you're asking, you probably don't *need* a custom goal, but reading this page might give you new ideas for useful goals!

Use a custom goal when none of the other types quite fit what you're looking for.  You can also use custom goals to use autodata sources differently than the default goal types you get when creating them.  

For example, you might create a weight goal that automatically sources data from your Withings scale, then turn it custom to enable more settings.  If you change the settings appropriately, you can make it so instead of beeminding your weight, you're actually beeminding whether or not you used the scale today.  Really useful for avoiding the *very* common 'avoiding the scale' problem, and it takes just a couple minutes to set up with a Beeminder custom goal!

(If I just sold you on that goal, it's good side above, road direction up, odometer off, cumulative on, aggday = binary, noisy off.  Lane width 0 and rate = 7/wk for the most hardcore commitment!)

#### How should I enter data for a custom goal?
It depends on the settings you enable, mostly on whether the goal's data is auto-summing or not.  Auto-summing data is like a Do More or Do Less, while not auto-summing covers the rest of the goal types.

#### What do all the settings mean?
  - **Good side of the road**: whether you want to be above or below the yellow brick road.  Above is generally for things you want to do more frequently or increase over time, and below is for things to do less frequently or decrease.
  - **Direction of road**: whether the road should be going up or going down.  Going up means you should have a positive goal rate, and going down means you should have a negative goal rate.
  - **Exponential road**: see the next question for more info!  (TODO: link here)
  - **Cumulative**: whether your datapoints should be added together or not.  Do More and Do Less are cumulative; the other goal types are not.
  - **Resettable odometer**: whether a 0 datapoint resets your rolling total.  See the Odometer page for more information.  (TODO: link)
  - **Integery**: see the next question for more info!  (TODO: link to it, also what are the implications here again?)
  - **Aggregation**: how Beeminder plots your datapoints every day.  These are listed in the next question! (TODO: link here)
  - **Plotall**: whether Beeminder plots all your datapoints, or just the result of the aggregation method.
  - **Absolute lane width**: how wide your yellow brick road is.  This will change how frequently the colors change on your goal. (TODO: is this true) (SECOND TODO: this should go away with YBHP?)
  
You can find a more in-depth explanation (with even more hidden settings explained!), in the [Beeminder API docs](https://www.beeminder.com/api#goal).  

(TODO: maybe put graph images w/ explanations in here to exemplify differences)

#### How exactly do exponential goals work?
Use an exponential goal to change a value by a certain % each week.  The rate you enter is the % per week (e.g. -0.5 to decrease at 0.5% per week).

The simplest, most common use case is weight loss.  Rather than commit to losing 1 pound per week (which gets more difficult as you lose more weight), you can use an exponential road to commit to losing 0.5% of your bodyweight per week, so the difficulty stays a little more constant over time.

You can approximate an exponential road by paying attention to your goal rate and making changes with the road dial when it feels right to make the goal easier or harder. 
(TODO: confirm this, exproad blog link)

#### What does 'integery' mean?
(TODO: confirm this) 
Enabling the integery option tells Beeminder that fractional data doesn't make sense for this goal, and will conservatively round your reminders accordingly.

For example, let's say I have a goal to wake up before 9am five times per week.  Beeminder works on a daily basis, so by default, it'll tell me to do 0.71 wakeups to avoid derailment.  In this case, I can't actually do 0.71 wakeups; it's either 1 or 0.  Enabling integery will make Beeminder tell me to do 1 wakeup instead, so my goal and reminders make a little more sense.

#### What do each of the aggregation options do?
The aggday setting controls how Beeminder interprets all your data on each day, according to the chart below.  

|Option Name|Beehavior|
|:-:|-|
|last|Only most recent datapoint counts|
|first|Only first datapoint counts|
|min|Smallest datapoint counts|
|max|Largest datapoint counts|
|truemean|Mean of all datapoints|
|mean or uniqmean|Mean of all unique datapoints (TODO: deprecate b/c why bother?)|
|median|Median of all datapoints|
|mode|Mode of all datapoints|
|trimmean|(TODO: explain in english)|
|sum|Sum of all datapoints|
|binary|Plots a 1 if any datapoints have been entered, otherwise 0|
|nonzero|Plots a 1 if any nonzero datapoints have been entered, otherwise 0|
|triangle|(Sum of datapoints * sum of datapoints+1)/2 ([wut?](https://blog.beeminder.com/triangle))|
|square|Sum of datapoints squared|
|clocky|Sum of differences of pairs (TODO: example for wut)|
|count|Number of datapoints entered|
