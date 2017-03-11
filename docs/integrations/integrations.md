#### What is 'autodata'?  What are the integrations?
'Autodata' is what we call automatically entered data.  Instead of visiting Beeminder every day and updating your goal with your daily step count, you can authorize us to access your Fitbit data, so we can update your goal for you!  

You can see the full list of services we work with here in the help docs.  If the service you want isn't included, check Zapier or IFTTT.  Those two services create links between more than 500 different apps, so anything we don't have is *probably* supported by one or both of them.

And if you enjoy writing code, you can use the [Beeminder API](https://www.beeminder.com/api) to roll your own automatic updates!

#### How do I use an autodata integration?
Most autodata goals use a back-end connection that's set up when you create a goal, so Beeminder can 'pull' the latest data anytime.  Click on the logo of the service you want to beemind on the [New Goal](https://www.beeminder.com/new) page and continue normally through the goal creation process.

A subset of the integrations are 'push' integrations, where the services tell us what data to add to your goal.  For these goals, you'll need to first create a 'regular' Beeminder goal (almost always a Do More), and then tell the service which goal to update.

#### How often is my data updated?
We check your data at least once per day, at your deadline.  We'll also check right before we send you any reminders, so that we've got the most up-to-date info when we're telling you what you need to do today!

You can also force a data fetch for most integrations by pressing the ♻ button on your goal page or dashboard.  Beeminder will pull the most recent value and update your graph.  For integrations that 'push' data to us (IFTTT, Zapier, Complice), you'll need to visit that service and initiate the job yourself, if possible.

#### I forgot to sync my data in time, and my goal derailed.  Help?
Not a problem.  Just sync the data, reply to the legitimacy check email, and support will fix it for you.  

This is more likely to occur on push integrations, especially if you're working right up to the deadline and we receive the pushed information too late.  You can change the date on the data so it reflects when you were actually working, and let us know the derailment needs to be fixed.

#### Beeminder isn't fetching my data correctly!  Help?
First, double-check that the service itself has the correct data.  If your Fitbit account isn't synced correctly, Beeminder can't get your daily step counts!

Second, try removing and reauthorizing the service in question [here](https://www.beeminder.com/settings/account#account-permissions).  

Third, take a quick look at the help page for the integration and see if your problem is a known one or common question.  Most of the integrations have corner cases or specific exclusions, and you might have come across one.

If none of those solve it, contact support and we'll help you out.
