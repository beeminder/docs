descriptions of non-custom goal settings / features

#### What does 'no mercy' mean?
By default, Beeminder gives you a "week off" when you derail, in case you want to adjust the goal parameters.  Tick this box and we won't give you that week off.

A common confusion is that 'no mercy' truly means *no mercy*, and it will immediately be an emergency day again.  It doesn't quite work that way for technical reasons.  If you really want *no mercy*, contact support and we'll adjust your goal manually.

#### What does 'weaselproofing' do?
Tick this box if you don't trust yourself not to weasel (TODO: link) and you want us to hold you to it!  (But bee **really sure** you want to do it, because it's undoable.)  If you derail on a weaselproofed goal, support will ask you for proof of your excuse.

For example:
  - "I was sick!" --> can you show us a prescription, or an email to your boss, or a text to your friend complaining about being sick?
  - "I really was awake by 8am, I just forgot to enter data!" --> can you show us steps on your Fitbit before 8, or a receipt from the gas station, or a message sent?
  
Also acceptable: a Tweet or Facebook post or *insert-social-media-of-your-choice-here* that says "I didn't enter data on my Beeminder goal in time, and this is what I'm doing to get out of the penalty!"

#### How does 'weekends off' work?
Beeminder will automatically schedule weekend breaks one week in advance, so you don't have to work on weekends, and you don't have to remember to do it yourself!  This is a feature of the Bee Plus [subscription](https://www.beeminder.com/premium).

#### How does 'max safe days' work?
Beeminder will automatically trim your safety buffer if it's above a maximum value you set, once per day (after the goal deadline time).  This is a feature of the Bee Plus [subscription](https://www.beeminder.com/premium).

(TODO: b&a example)

For Do Less goals, this works in *units* rather than *days*.  If you're beeminding calories available, don't trim to 3 safe days!  You'll end up allowing yourself 3 calories, which is Not Enough Calories.  Use do 3 * *daily calories allowed* instead.

#### Can I change my goal URL?
Yup, that's the 'Goal Name' field in the settings.  Note that Beeminder does not do redirects, so if you've linked to your goal anywhere, those links will break if the goal name changes.

#### Can I hide sections of the graph?
Yup!  Use the x-min and x-max settings to show specific dates (change horizontal range), and y-min and y-max settings to show specific data valuse (change vertical range).

This is a great, fast way to get a "fresh start" on a goal, without having to wait out an archive or ruining your history by removing datapoints (which will also totally derail your goal).  It's also helpful if your goal is getting really cramped by having lots of data - change the x-min closer to the present to space things out again!

#### Is my goal publicly accessible?  Is my data?
By default, goal pages are publicly viewable, but data is not.  You can change either of those settings anytime, as well as change your own default settings (TODO: link to q).

You can also choose to [feature](https://www.beeminder.com/featured) your goal, which allows it to show up in the Featured gallery from time to time.  Aside from that, we don't disseminate or display user goal information anywhere, though you're certainly welcome to share your own goals anywhere as much as you'd like!
