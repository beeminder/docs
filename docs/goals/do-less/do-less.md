Do Less goals are a feature of the [subscription](https://www.beeminder.com/premium) plans.  They have a few quirks, but if you're trying to wind down a bad habit, Do Less goals might bee the goal type you want.  (If you want to go cold turkey, use a Do More!)

#### When should I use a Do Less?
Use a Do Less goal for things you want to limit.  You're probably still going to do it sometimes, but you want to do it less often.

Common examples: eating sugary treats, smoking, spending time on Facebook, eating salty treats, oversleeping, watching reality TV shows, drinking coffee, engaging with internet trolls, biting your nails, spending money, using profanity at work, reading political Twitter, eating fewer calories...

#### What if I NEVER want to do something?  Can I still use a Do Less?
Technically, yes...

But we **strongly** recommend that you use a Do More goal to Not Do Something at a rate of 7 days/week.  Many users find that Do Less goals with 0 rate are more of a pain to manage.  You might also lose out on any extra motivation from watching the graph build over time - the goal just stays a boring flat line, and any lapses are really obvious!  
(TODO: graph comparison)

Instead of making a Do Less goal to "never eat potato chips," I would make a Do More goal to "go a day without buying potato chips," 7 days a week.

But yes, if you really want a 0-rate Do Less, you can do that.  

#### How should I enter data for a Do Less?
Beeminder needs to know how much Whatever you did that day.  Beehind the scenes, it adds up all your datapoints to show you how much Whatever you've done since starting the goal.  

Let's say I have a goal to drink less coffee - at most 4 cups per week, to bee exact. I drank 0 cups today, I submit a 0 to my graph.  Tomorrow, when I drink a cup, I'll submit 1 to my graph.  The next day, I abstain again, so I submit a 0.  And so on.

After those three points have been submitted, the graph will look like this:
(TODO: graph image, probably w/ data on the right)

I'm below my road - doing better than my goal rate!  Cool.  And Beeminder's keeping a running total of all my progress for me, so I know I've only had 1 cup of coffee since starting my goal.  
(TODO: stats panel image)

#### Why does that sound suspiciously similar to the Do More answer?
Do More and Do Less goals are like sisters (but not twins).  They work almost exactly the same way, but you want to be *above* the road on a Do More, and *below* it on a Do Less. 

#### What happens if I never enter data?  I'm already below the road and it's only getting higher...
Astute observation, young bee.  With a Do More, if you abandon the goal, you'll eventually crash into the road and derail.  But the Do Less goal has no power over you if you don't actually use it.  
(TODO: comparison graph image showing DM vs DL crash vs valley)

So we came up with the pessimistic presumptive report (PPR), an automatically-entered datapoint that assumes data if you don't enter any yourself.  Given enough time, the PPRs will eventually cross over the road, and you will derail.  This helps keep the goal effective: as the data climbs nearer and nearer to the road, Beeminder will start sending you more and more frequent reminders about the goal, which will hopefully remind you that you wanted to stop doing Whatever!
(TODO: graph image w/ data panel full of PPRs)

To get rid of PPRs that have already been entered, just enter your data for that day!  Beeminder will automatically delete the PPR datapoint, so that the only data for the day is the value you told us.

You can turn off the PPR in the goal settings at any time.

#### I'm going on vacation and won't be working on my Do Less goal.  How can I pause it temporarily?
For a Do Less goal, all you need to do is make sure the PPRs are turned off, and then enjoy your vacation!  If no data is entered while you're away, you cannot derail.  You can get rid of any unwanted safety buffer when you return, or enjoy your new allowance.

The more Quantified Self-inclined users might want to enter their data for the break period without being at risk of derailment.  You can use Take a Break to build a jump into the road, so that your vacation data still falls below the road.
(TODO: break config -> graph image showing a huge jump)

Bee Plus or Beemium subscribers who want even more fine-grained control might find the Road Editor (TODO: link to example) useful for redrawing history.

#### How do I get rid of extra safety buffer on my Do Less goal?
Use the 'Safety Buffer' section in the 'Commitment' tab below the graph to choose the number of **units** of safety buffer you want, then click 'Retroratchet!' to apply.  

(This is a small difference from all the other goal types, which use **days** of safety buffer, rather than **units**.  'Days' of buffer are a bit of an illusion for Do Less goals, because you might be able to use up all your buffer in 1 day, no matter where you started.)
(TODO: example of binging blowing up my spot)

#### My goal was red but it didn't derail!
This is a known Beeminder technicality, and we're okay with it (for now).  Even though you went over the limit one day, you didn't go over far enough to fall off the average pace... yet.  But you can't do it two days in a row, so bee extra careful today!
