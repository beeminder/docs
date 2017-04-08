#### What can I beemind with Duolingo?
Beeminder tracks your points in one (or more) of the 20+ available languages.  See [here](https://www.beeminder.com/new#duolingo) for a full list!

#### Can I track multiple languages?
Yup!  You will need a separate goal for each language, and you'll want to use the same native language for all courses.

#### Can I have a non-midnight deadline for this autodata goal?
Yes!  Change it in the reminder settings.  All the normal deadline restrictions and rules apply.

#### Beeminder just dropped all my points!
98% of the time, this is because you changed your Duolingo username or native language.  

If you've changed your username, contact Beeminder support and tell us your new username.  We'll update your goal with the new information.

If you've changed your native language, changing it back to its previous value should fix the points fetching.  (This happens because we don't get English -> French and Spanish -> French points when you track French points.  It only sends the points value for the course associated with your native language.)

If you want to restart your language progress, see the next question for how to do so safely.

If none of these sound right or solve your problem, send us a support email!

#### Can I restart my language progress in Duolingo without derailing my goal?
Yup!  First, restart the language in Duolingo, so that you have 0 points.  Then go to your Beeminder goal and force a data fetch, so Beeminder gets a 0 datapoint.  This will [reset the odometer](../goals/odometer/odometer.md), so Beeminder doesn't lose your progress thus far.  You can then start using Duolingo again normally!

Advanced Beeminder tip: the key to resetting the odometer is to have the 0 datapoint **in-between** the highest value and the smallest value.  If you started working on the language again before reading this question and already synced a low number, you can edit the tiny datapoint to 0, then force a new fetch to fix things.

#### I don't see the language I want on the list.  Can it be added?
Possibly!  Email us in support to get the feature request in.  Last time we did it in less than two days!
