pledges, when do i pay, shortcircuiting, stepdowns, pledge caps, subscriptions

#### How much does Beeminder cost?
You pay Beeminder for [derailments](../derailments/derailments.md) on your goals and/or for a monthly [subscription](https://www.beeminder.com/premium).

#### What are the derailment pledges?  Can I pledge anything I want?
No.  The pledge amounts are $0, $5, $10, $30, $90, $270, $810, and $2430.  Pledges increase (or decrease, if stepping down) along this sequence.

We put a lot of thought (and math) into this (TODO: pretty sure there's a blog post to link to but I can't remember it) if you're interested...

#### Do the pledges automatically get higher every time I derail?
Yes, if you have enabled increasing pledges on the goal.

To change this setting on a goal, click the pledge amount on the goal page to bring up a pledge control panel.  The 'Increase the pledge each time...' controls whether pledges increase or stay put upon each derailment.  

#### Can I limit how big my pledge gets?  I don't ever want to risk $90.
Of course!  You can set a pledge cap on each goal.  For example, if my pledge cap is $10, derailing at $10 will not raise my pledge to $30.  It will remain at $10.

Click the pledge amount on the goal page to bring up a pledge control panel.  To set the pledge cap, tick the 'Increase the pledge each time...' box, then pick the desired pledge cap using the +- arrows.  Click 'Update' to save changes.

You cannot select a pledge cap lower than the goal's current pledge.  If you want to do this, first step down the current pledge to that amount (or lower), and then the desired pledge cap value will become available.

(TODO: I went through several stages of WTF writing this.  this could definitely be more intuitive, although it all shook out in the end...)

#### Can I immediately increase my pledge?  $5 and $10 are meaningless to me; I want high stakes sooner.
We call this 'short-circuiting,' and it's a feature of the Beemium [subscription](https://www.beeminder.com/premium).

#### Can I lower a pledge that's already too high for me?
Yes.  You can step down the pledge one level at a time.  Like most changes that make the goal easier, each step takes 7 days to take effect.  

Click the pledge amount on the goal page to bring up a pledge control panel, then click the 'Decrease pledge to $X' button.  Your goal page will refresh, and the pledge amount will change to indicate the pending stepdown.

#### Can I have goals without pledges?  I prefer the motivation of the graphs to financial pressure.
With the Beemium [subscription](https://www.beeminder.com/premium), you can set a pledge cap of $0 on any goal.

#### How do I subscribe (or cancel my subscription)?
Visit the [subscription](https://www.beeminder.com/premium) page, linked in the top navigation under 'Premium'.

#### What is the slider on the subscription page for?
Pre-pay discount: pay more money less frequently, save a little bit!  You can also buy a lifetime subscription for a one-time charge.

#### What are these 'auto-canceling subscriptions' I've seen mentioned?
If you don't use Beeminder for 30 days in a row (TODO: clarify condition), we'll send you an email letting you know your subscription is on hold, and we'll stop charging you for it.  If you return and start beeminding again (TODO: clarify condition), your subscription will reactivate and the charges will begin at the same frequency as before.

#### What if I buy a lifetime subscription at one level, and then want to change levels?
We’ve thought of and coded for a ton of corner cases, so making your change via the subscription page should be sufficient.  If you encounter any problems or have questions about what will happen, please contact support!  We’ll make sure the exquisitely fair thing happens no matter what.

#### What payment methods can I use?
Credit card.  We use [Stripe](https://www.stripe.com) for payment processing.

#### How do I update my card information?
Visit the [Payments](https://www.beeminder.com/payment) page, linked in the top navigation dropdown.
