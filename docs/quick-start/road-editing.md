There are a bunch of ways to edit your yellow brick road once you've created a goal - you're not committed to that initial rate until the end of time (unless you want to bee)!  Here we'll walk you through how to use all the different road-modifying features.  As always, if anything goes haywire or does not do what you wanted it to, [contact support](https://www.beeminder.com/contact) and we'll help make it right!


#### Commit To: The Road Dial
This is the first option in the 'Commitment' tab below the graph.  You can use this field to change your goal rate.  All changes are "dialed in" starting 7 days in the future (todo: 8?), even those that make the goal _harder_ rather than easier.

To change your rate, change the number in between the -/+ buttons and press 'Update'!  You can also update the time unit being used (for example, you may prefer to switch your 1 time per day goal to 5 times per week, rather than 0.714 times per day).  The time unit field is purely for your convenience; switching it without changing the rate value will not impact your graph in any way.

You also have the option to describe your goal using a goal date and/or a goal value.  For example, reaching a goal value of 120 pounds by October 28th, rather than losing 1 pound per week.  To open up those fields for editing, click the 'Change goal date and goal total' link.  

You must choose 2 of the 3 fields to edit when using this form of the road dial.  Edit the 2 fields you want and make sure their backgrounds are still white when you hit 'Update'!  (Otherwise you might submit values that you didn't want to.)   

#### Retroratchet: Reduce Safety Buffer
This is the second option in the 'Commitment' tab below the graph.  You can use this field to reduce the number of safety buffer days you have on your goal.  This change happens _immediately_ and cannot be undone, so retroratchet wisely!  

To retroratchet, enter the desired number of safe days into the box, then press 'Retroratchet!'  Entering a 0 will immediately make your goal an eep day, but you can't do it right after a derailment (unsolved technical debt - email support and we'll do it manually).  

**A note on do-less goals**: this 'safe days' field is expressed in terms of 'safe units' instead.  When retroratcheting a do-less, enter the number of _units_ of your goal that you'd like to have as buffer.  For example, if I want to retroratchet my "eat less calories" goal that currently has a rate of 2000/day to 1 safe day, I need to enter _2000_ in the retroratchet field, _not 1_.  Entering 1 means that you will give yourself 1 calorie allowed for the rest of the day!  Probably not what you wanted :) 

If you are a Bee Plus or Beemium [subscriber](https://www.beeminder.com/premium), you will have a setting called 'Max Safe Days' right underneath the Retroratchet section.  If you check the box to 'Automatically trim safety buffer,' Beeminder will retroratchet your goal daily at your deadline time if it exceeds the number of max safe days you set in the box below.  Automatic retroratcheting works the same way as regular retroratcheting; it just happens automatically! 

#### Take a Break
This is the second (or third, if you are a Bee Plus or Beemium [subscriber](https://www.beeminder.com/premium)) option in the 'Stop/Pause' tab below the graph.  You can use this field to schedule temporary changes to your goal rate.  Usually folks want to make it easier for a spell (e.g. I don't want to study during winter holidays), so we named the feature Take a Break.  But you can also use it to make the goal _harder_ for a period as well (e.g. I want to study extra hours during the week before final exams)!

To take a break, first input the dates that you want this modified rate to be active.  **The start date should be the day _before_ you want the break to begin**.  (TODO: arghhh!!!) The end date is the date you want the break to end.  Choose the rate you want to have during the break in the box below the dates, then press 'Schedule' to submit the changes to the road.

The akrasia horizon is strictly enforced: a break cannot start earlier than 7 days from now - even if you're trying to make the goal harder (contact support if you want us to make that change for you!).  

**A note on do-less goals**: the easiest way to take a break on _manual_ do-less goals is to disable the PPRs while you're away, then turn them back on & retroratchet the goal when you return.  For do-less goals with _automatic_ data sources, set the road rate to a _higher_ value than your regular rate to have a break.  Unlike the other goal types, a rate of 0 during your break will actually make the goal harder and more likely to derail!

#### Road Editor 

