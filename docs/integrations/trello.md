#### What can I beemind with Trello?
Trello goals track the number of cards in one or more lists on a particular board.  

#### Can I beemind private Trello boards?
Yes.  At goal creation, we'll ask you to authenticate with a Trello account that has permission to view the board.

#### How do I change the lists my goal is tracking?
In the 'Settings' tab below the graph image on the goal page, you can pick and choose the right lists in the 'Trello Lists' section.  Click 'Update' to save the change and refresh the graph.

This will not rewrite any goal history, but it will change your current datapoint and may trigger an emergency day if your list count decreases.

#### Can I change the board my goal is tracking?
Nope.  You'll need to make a separate goal to track a different board.

#### I didn't change any settings, but my Beeminder datapoint just dropped a lot, and now my goal is about to derail!
Usually this happens when you've deleted cards, or you archived cards but are not beeminding the Archived list.  Beeminder always uses the current total count in all tracked lists, so moving cards *out* of those lists will drop the number down.

To resolve this immediately, you can empty the lists on Trello (see the next question) or add the Archived list to your tracked lists in the Beeminder goal.  Contact support if neither of those options is a good one for your case.

#### Can I start over from scratch on an already-existing goal?
You can [reset the odometer](https://github.com/beeminder/docs/blob/master/docs/goals/odometer/odometer.md#what-happens-if-i-need-to-restart-my-count-at-0) by clearing out all the tracked Trello lists and pressing the 'Fetch Data' button on Beeminder.  This will add a 0 datapoint to your graph, allowing you to start fresh without losing your previous progress.
