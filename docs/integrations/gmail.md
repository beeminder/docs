#### How does GmailZero work?
GmailZero uses a [whittle down](../goals/whittle-down/whittle-down.md) goal to reduce or maintain the size of your inbox over time.  By default, we count up the number of **read** messages in your inbox, but you can use different criteria if you want. 

#### Why are you asking for permission to read my emails?
We need to know what's in your email in order to count the number of qualifying items in your email.  We don't access, read, use, save, analyze, sell, or fill-in-the-blank your information beyond that.

#### How do I change the query Beeminder counts?
When creating the goal, you have the option to choose a different query.  (TODO: link to gmail query syntax) 

If you want to change it after creating the goal, you can find it in the goal settings.  Note that changing the query will *not* move the road.  If you're going from a small count to a large count by changing the query, you may have a lot of work to do before the day ends!

#### I'm pressing the fetch button, but my datapoint and graph don't appear to be updating with new data.
Refresh the goal page and check the comment on your most recent datapoint.  If the timestamp and value in the comment are accurate, the right thing is happening!

GmailZero goals use the *lowest* datapoint of the day, which might not be the *most recent*.  (You can change this by converting to a [custom goal](../goals/custom/custom.md) and changing the aggday setting.)  This is more lenient beehavior than many of the other goals have!  If you get below the road once during the day & make sure Beeminder fetches the count while you're there, you can let the emails pile up again until tomorrow.

#### I'm pressing the fetch button and my datapoint is updating, but it doesn't match what I see in my inbox.
Some emails with blank snippets are counted differently between the Gmail UI and the Gmail API.  Right now, we're not sure entirely why this is happening.  But in almost every case (TODO: every case?) Beeminder has ended up counting a smaller number than the Gmail UI, so you probably won't derail because of this.  If you do, please let us know!

#### My GmailZero goal is telling me I need to reach a negative number of emails!
See 'What happens when I reach 0?' on [whittle down](../goals/whittle-down/whittle-down.md) (TODO: anchor links.  or helpscout) goals.
