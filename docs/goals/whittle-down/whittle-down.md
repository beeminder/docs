The canonical Whittle Down goal is reaching Inbox Zero - this goal type was even once called Inbox Fewer.  But it's so much more than that!

#### When should I use a Whittle Down?
Whittle Down goals are best used when you're trying to whittle down a backlog over time.  Similar to an Odometer, you'll want to know your daily total backlog size, which you want to be reducing over time.

Common examples: managing inbox size, reading Pocket articles, grading assignments, watching downloaded movies, completing lessons in a MOOC

#### How should I enter data for a Whittle Down?
Beeminder needs to know your current total Whatever as of each day.  

Let's say I have a goal to clear out my inbox over time - 100 emails per week, to bee exact, and I have 500 emails in my inbox today. I archived 20 emails today, putting me at 480 emails in my inbox, so I submit a 480 to my graph.  Tomorrow, when I archive 30 more emails and get to 450 remaining, I'll submit 450 to my graph.  The next day, I only do 5 emails, so I submit a 445.  And so on.

After those three points have been submitted, the graph will look like this:
(TODO: graph image, probably w/ data on the right)

I'm below my road - doing better than my goal rate!  Cool. 

#### What happens when I reach 0?
If your graph is configured to end at 0, the goal will end.  Yay!   You can restart the goal if you'd like to maintain a maximum value.

(TODO: rate vs. value config comparison)

If not, your graph may continue decreasing, eventually asking you to get to a negative total.  This is usually not possible. You can prevent that by configuring the goal to end at 0, or setting the rate to 0 at the backlog size you want to maintain.  If your graph is asking you to do something impossible, contact support and we'll fix it!

#### What happens if I need to restart my count at a higher number?
If the goal has ended or been archived, you'll be prompted for your current value when restarting.

If the goal is still active, you can use Take a Break or the Road Editor to schedule a road jump in the future.  

(TODO: same as do-less take-a-break example, but with whittle down)

#### I'm going on vacation and won't be working on my Whittle Down goal.  How can I pause it temporarily?
This is easy to do on a Whittle Down!  Using the 'Take a Break' section in the 'Stop/Pause' tab below the graph, first pick the dates that you'll be away, then set the break rate to 0.  This will make your road flat at that time, so you don't have to make any progress until it starts sloping down again.
(TODO: graph image w/ break)

You'll need to make sure that no data enters the graph while you're away.  If an automatic data source enters a value that lands above your road, even on your break, you will derail.  This is definitely not legit and we'll sort it out in support, but stopping the data source will prevent it from happening in the first place!

Note that you probably want the first date of the break to be the day *before* your break begins.  The first date is the last day you'll have to do work before the 0 rate section kicks in.
(TODO: I know it's legacy at this point but can we just fix this so we can axe this section?  it's so easy)

#### Yesterday my Whittle Down goal said I had 15 safe days, but I derailed today.  What happened?
You need to have at least one datapoint below the road during the day to avoid derailing, no matter where you were previously.  

Whittle Down goals are not incredibly forgiving when your data value can bounce up and down a lot.  The 'safe days' estimate Beeminder uses assumes that your data moves in one direction only.  But things like your inbox size can increase as well as decrease, so the 'safe days' estimate may be blown away if you receive an unexpected deluge of emails that takes you over the limit.
