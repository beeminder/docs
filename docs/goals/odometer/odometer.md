Odometer goals are relatively uncommon in vanilla beeminding, but a fair number of the autodata integrations use Odometers at heart.

#### When should I use an Odometer?
Odometers are very similar to Do Mores, but the data needs to be entered a little differently.  Use an Odometer when it's easier to know your total progress than it is to calculate today's progress, or when the data you're tracking *shouldn't* be added together over time.

Common examples: tracking pages read in a book, daily revenue, miles ridden on your bike (could be tracked by an actual physical odometer!)

#### How should I enter data for an Odometer?
Beeminder needs to know your current total Whatever as of each day.  

Let's say I have a goal to read more often - 100 pages per week, to bee exact. I read 20 pages today, putting me on page 20 in my book, so I submit a 20 to my graph.  Tomorrow, when I read 30 more pages and get to page 50, I'll submit 50 to my graph.  The next day, I only get to page 55, so I submit a 55.  And so on.

After those three points have been submitted, the graph will look like this:
(TODO: graph image, probably w/ data on the right)

I'm above my road - doing better than my goal rate!  Cool.  And Beeminder's keeping a running total of all my progress for me, so I know I've read 55 total pages since starting my goal.  
(TODO: stats panel image)

#### How is that different than a Do More?  
The graphs will look exactly the same, but the data you enter needs to be different.  
(TODO: insert side-by-side of do-more vs. odometer)

#### What happens if I need to restart my count at 0?
To continue my book example - what happens when I finish my book?  It would be irritating to have to remember the pages in my previous book and then add them to my new book page, and then again for a third book...

Beeminder interprets a datapoint of 0 as a 'reset' of the odometer.  After a 0 datapoint has been entered, you can start your page count from 0 again without losing ground.
(TODO: insert side-by-side of no-reset vs. reset)

All of your statistics will include the total number of pages read, without you having to maintain that count yourself!

#### I'm still confused on the difference between Odometer and Do More.
Do More is the right choice almost all of the time, so try that first.  If you have questions or objections, contact support, and we'll be happy to recommend a good goal setup for you.

#### I made an Odometer, but I should've made a Do More (or vice versa).  Can I change the goal type?
Because of the fundamental difference in how Beeminder handles the data, it's usually not trivial to change the goal type.  It's easiest to archive or delete the Odometer goal and start a new Do More.

#### I'm going on vacation and won't be working on my Odometer goal.  How can I pause it temporarily?
This is super easy to do on an Odometer!  Using the 'Take a Break' section in the 'Stop/Pause' tab below the graph, first pick the dates that you'll be away, then set the break rate to 0.  This will make your road flat at that time, so you don't have to make any progress until it starts sloping up again.
(TODO: graph image w/ break)

Note that you probably want the first date of the break to be the day *before* your break begins.  The first date is the last day you'll have to do work before the 0 rate section kicks in.
(TODO: I know it's legacy at this point but can we just fix this so we can axe this section?  it's so easy)
