#### I'm confused.  What numbers does Beeminder want from me?  What is 'my data'?
Beeminder just needs to know how much progress you made on your goal today!  The way it's represented is a pair of numbers: < date > < value > "any optional comment or note about today's data".

For example, let's say I have a goal to read 100 pages per week.  I would tell Beeminder that I read 10 pages on the 8th by saying "8 10".  

You can also expand the date format further if you want to enter older data: "2014 08 10 10" would add a datapoint of 10 on August 10, 2014 to my goal.  We've carefully written code to infer the right date almost every single time, but if we infer incorrectly, you can also edit the data after submitting it.  

#### What do I do to enter data?
There are a bunch of ways to submit info!
  - dashboard
  - goal page
  - apps
  - email
  - sms
  - have it automatically fed from another service
  - write your own automatic service using the Beeminder API
  
The date-value-comment format described above is used in most cases.  
  
#### Do I have to enter data every day?  
Nope!  We do recommend that you try and enter the data shortly after you've done the work, but you can enter data for any day in the past anytime.  If you forgot to enter data yesterday, just do it today, and make sure you use yesterday as the date!

The one semi-exception to this exists on Do Less goals: a pessimistic presumptive datapoint is entered if you don't enter data for the day, which can cause your goal to derail, even if you were previously safe!  See the [Do Less docs](https://github.com/beeminder/docs/blob/master/docs/goals/do-less/do-less.md) for more information.

#### I entered my data wrong.  How do I fix it?
Update the incorrect point in the 'Data' tab below the graph, then press the 'Update' button on the right side of the line.

You can also delete datapoints using the 'Delete' button, though you should do this with **extreme caution** - it may trigger an immediate derailment on your graph, if you are no longer on track after the data is removed.

#### Can anybody else add or edit my data?
No, only you and the Beeminder team can modify your data.

If an unrecognized email address tries to submit data to your goal via email, we'll automatically send you an email asking if the address is valid and data should be accepted.  This happened 3 times in all of 2016, so it's pretty rare, but we've got you covered!  

#### Can I export all my data?
Yup!  You can find .csv and .tsv export links near the bottom of the 'Data' tab below the graph.

#### I started my goal in minutes, but now I want to switch to hours.  Help!
The easiest way to fix this is to scale your current graph into hours!  Use the 'Scale Datapoints' section at the bottom of the 'Data' tab below the graph to scale everything by 1/60 (dividing by 60) and press 'Scale It!'  Beeminder will adjust all the data and road values accordingly, so you can start using hours.

Note that if you already have data added to your graph that uses the new unit, you will want to **remove** that data **before** scaling your goal.  Otherwise, that point will get scaled to the new unit (even though it's already using the new unit), and that progress won't be represented accurately on the goal.

If anything goes wrong or these instructions are terribly confusing, [contact support](https://www.beeminder.com/contact)!
