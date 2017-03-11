glossary of settings, exponential, examples

Custom goals let you pick and choose which settings to enable, while the regular goal types are all predefined.  

#### When should I use a custom goal?
If you're asking, you probably don't *need* a custom goal, but reading this page might give you new ideas for useful goals!

Use a custom goal when none of the other types quite fit what you're looking for.  You can also use custom goals to use autodata sources differently than the default goal types you get when creating them.  

For example, you might create a weight goal that automatically sources data from your Withings scale, then turn it custom to enable more settings.  If you change the settings appropriately, you can make it so instead of beeminding your weight, you're actually beeminding whether or not you used the scale today.  Really useful for avoiding the *very* common 'avoiding the scale' problem, and it takes just a couple minutes to set up with a Beeminder custom goal.

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

#### What does 'integery' mean?

#### What do each of the aggregation options do?

