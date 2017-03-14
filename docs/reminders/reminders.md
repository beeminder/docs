Before you derail on a goal, Beeminder will send you a bunch of reminders and tell you how much more work you need to do to avoid derailing.  Unless you turn them off... which we recommend you don't do!

#### What reminder methods are available?
Email, iOS and/or Android notifications, posting to a Slack channel, sending a Slack DM, and SMS (for Bee Plus and Beemium subscribers).  You can also set up an external webhook. (TODO: i don't understand this well enough to explain it)

For each goal, you can get notifications via any combination of these channels.

#### When do I get my reminders?
Beeminder sends the reminders starting at the **Start Alerts** time, with the **Lead Days** number of days before the goal derails at the **Deadline** time.

Like most things, this is easier to understand with an example!  If my **Start Alert** time is 6am, with 5 **Lead Days**, Beeminder will start sending me my reminder emails at 6am when I have 5 or fewer days until I derail on the goal.

The reminders come more and more frequently as the goal gets closer and closer to derailment.  

(TODO: I may not understand how this works/changes when data is added.  like if I add enough to non-eep but not enough to get in front of my lead days again.)

#### Do I have to set these for every goal?
When you make a new goal, we'll use your default [reminder settings](https://www.beeminder.com/reminders) at first.  You can go in any time to modify them.

#### Can you just send me all the reminders in one message/notification instead?
The main reason we separate them is so it's easy to quickly reply to them with data!  This makes it really easy to treat your inbox of reminders like a to-do list, replying to cross things off.  

If you're getting reminder overwhelm, the quickest fix is to think about your settings and make modifications where necessary.  (Perhaps you don't need 3 days notice for your tooth-brushing goal; that one might be fine to start at 8pm with 0 lead days.) 

If you're still dying for a batch/combined reminder, send us a feature request so we know the demand is out there!

#### How do I read the reminder notifications?
chelsea/recipes on 03/13 (~1 safe day) = for my (chelsea) goal 'recipes', on today (March 13), I have 1 safe day remaining before I derail!

On emergency days, the subject lines will be a little more dire:
chelsea/pages on 03/13 (Emergency Day!) at $5 = for my (chelsea) goal 'pages', on today (March 13), I must get back on the road tonight or lose $5

Subsequent reminders after the first 'Emergency Day!' alert will read:
Eep! +1 by 00:00am for chelsea/pages ($5) = for my (chelsea) goal 'pages', I need to do 1 more unit before my deadline (midnight, 00:00am) to avoid derailing and losing $5!

This works a little bit differently for Do Less goals, but the concept is the same: do *less* than the amount Beeminder tells you, or else risk derailing.
(TODO: i might want to present this differently b/c there might be more gtype variance i am not remembering rn)

#### Do you support international SMS?
Sorry, USA only right now!  But if you've got access to the iOS or Android apps, those will give you all the features of SMS and then some!

####  I didn't get any reminders!
If you didn't get reminders and you had them turned on, that's *definitely* not a legit derailment, and we want to hear about it!

First, check your spam folder if you're missing email reminders.  It's the bane of our existence, but there's only so much we can do to prevent it and it happens sometimes.

If that doesn't surface them, contact support and we'll investigate.


(general TODO: the Android app is hella outdated on this stuff, and other stuff.  what's the priority/roadmap on that?)
