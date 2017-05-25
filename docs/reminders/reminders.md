Before you derail on a goal, Beeminder will send you a bunch of reminders and tell you how much more work you need to do to avoid derailing.  Unless you turn them off... which we recommend you don't do!

#### What reminder methods are available?
Email, iOS and/or Android notifications, posting to a Slack channel, sending a Slack DM, and SMS (for Bee Plus and Beemium [subscribers](https://www.beeminder.com/premium)).  You can also set up an external webhook. (TODO: i don't understand this well enough to explain it)

For each goal, you can get notifications via any combination of these channels.

#### When do I get my reminders?
Beeminder sends the reminders starting at the **Start Alerts** time, with the **Lead Days** number of days before the goal derails at the **Deadline** time.

An example: if my **Start Alert** time is 6am, with 5 **Lead Days**, Beeminder will start sending me my reminder emails at 6am when I have 5 or fewer days until I derail on the goal.

The reminders come more and more frequently as the goal gets closer and closer to derailment.  

(TODO: I may not understand how this works/changes when data is added.  like if I add enough to non-eep but not enough to get in front of my lead days again.)

#### Do I have to set these for every goal?
When you make a new goal, we'll use your default [reminder settings](https://www.beeminder.com/reminders) for it.  You can modify them after creation if you want to be notified at a different time or using a different channel.

You can change your default settings anytime, but the changes won't automatically bee applied to existing goals.  

#### Can you just send me all the reminders in one message/notification instead?
The main reason we separate them is so it's easy to quickly reply to them with data!  This makes it really easy to treat your inbox of reminders like a to-do list, replying to cross things off your list by adding data to your goals.  

If you're getting reminder overwhelm, the quickest fix is to think about your settings and make modifications where necessary.  Perhaps you don't need 3 days notice for your tooth-brushing goal; that one might be fine to start at 8pm with 0 lead days.

If you're still dying for a batch/combined reminder, send us a [feature request](https://www.beeminder.com/contact) so we know the demand is out there!

#### How do I read the reminder notifications?
A standard reminder header will look something like this: **chelsea/recipes on 03/13 (~1 safe day)**  
For my (chelsea) goal 'recipes', on today (March 13), I have 1 safe day remaining before I derail!

On emergency days, the subject lines will be a little more dire: **chelsea/pages on 03/13 (Emergency Day!) at $5**  
For my (chelsea) goal 'pages', on today (March 13), I must get back on the road tonight or lose $5

Subsequent reminders after the first 'Emergency Day!' alert will read: **Eep! +1 by 00:00am for chelsea/pages ($5)**   
For my (chelsea) goal 'pages', I need to do 1 more unit before my deadline (midnight, 00:00am) to avoid derailing and losing $5!

This works a little bit differently for Do Less goals, but the concept is the same: do *less* than the amount Beeminder tells you, or else risk derailing.
(TODO: i might want to present this differently b/c there might be more gtype variance i am not remembering rn)

#### Do you support international SMS?
Sorry, USA only right now!  But if you've got access to the iOS or Android apps, those will give you all the features of SMS and then some!

####  I didn't get any reminders!
If you didn't get reminders and you had them turned on, that's *definitely* not a legit derailment, and we want to hear about it!

First, check your reminder settings to ensure that everything is configured the way you want.  If your start time is 11:59pm, with 0 lead days, and your goal deadline is 12:00am... you're not going to get many reminders!  Change those settings so we have time to notify you to get your stuff done :)

Second, check your spam folder if you're missing email reminders.  We do as much as we can to prevent spamboxing, but it does happen from time to time.  Marking those emails as not spam and adding the Beeminder bot to your contacts list may help stop this from happening, if it's been problematic for you in the past.  

Other users have found that email management services (e.g. unroll.me) sometimes hide or trash their Beeminder reminders unexpectedly.  

If none of the above surfaces the missing reminders, please [contact support](https://www.beeminder.com/contact) and we'll investigate to make sure they were sent as expected!


(general TODO: the Android app is hella outdated on this stuff, and other stuff.  what's the priority/roadmap on that?)
