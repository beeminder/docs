pledges, when do i pay, shortcircuiting, stepdowns, pledge caps, subscriptions

#### How much does Beeminder cost?
You pay Beeminder for [derailments](../derailments/derailments.md) on your goals and/or for a monthly [subscription](https://www.beeminder.com/premium).  Derailment costs are 100% variable and controlled by you and your actions!  Subscription fees are listed on the linked page above - check out the slider if you're interested in a [pre-pay discount](http://blog.beeminder.com/fair/)!

#### What are the derailment pledges?  Can I pledge anything I want?
No.  The pledge amounts are $0, $5, $10, $30, $90, $270, $810, and $2430.  Pledges increase (or decrease, if stepping down) along this sequence.

We put a lot of thought (and math) into this (TODO: pretty sure there's a blog post to link to but I can't remember it) if you're interested...

#### Do the pledges automatically get higher every time I derail?
Yes, if you have enabled increasing pledges on the goal.  

This setting is included at goal creation, but you can also adjust the setting after the goal's been created.  To change this setting on a goal, click the pledge amount on the goal page to bring up the pledge settings.  The 'Increase the pledge each time...' checkbox controls whether pledges increase or stay put upon each derailment.  

#### Can I limit how big my pledge gets?  I don't ever want to risk $90.
Of course!  You can set a pledge cap on each goal.  For example, if my pledge cap is $10, derailing at $10 will not raise my pledge to $30.  It will remain at $10.

Click the pledge amount on the goal page to bring up the pledge settings.  To set the pledge cap, tick the 'Increase the pledge each time...' box, then pick the desired pledge cap using the +- arrows.  Click 'Update' to save changes.

You cannot select a pledge cap lower than the goal's current pledge.  If you want to do this, first step down the current pledge to that amount (or lower), and then the desired pledge cap value will become available.

(TODO: I went through several stages of WTF writing this.  this could definitely be more intuitive, although it all shook out in the end...)

#### Can I immediately increase my pledge?  $5 and $10 are meaningless to me; I want high stakes sooner.
We call this 'short-circuiting,' and it's a feature of the Beemium [subscription](https://www.beeminder.com/premium).

To short-circuit a goal, click the pledge amount in the top line of the goal page to open the pledge settings.  Press the button to "increase pledge" - this will take effect immediately but can't bee undone immediately, so bee sure you're ready!

#### Can I lower a pledge that's already too high for me?
Yes.  You can step down the pledge one level at a time.  Like most changes that make the goal easier, each step takes 7 days to take effect.  

Click the pledge amount in the top line of on the goal page to bring up the pledge settings, then click the "decrease pledge" button.  Your goal page will refresh, and the pledge amount will change to indicate the pending stepdown.

#### Can I have goals without pledges?  I prefer the motivation of the graphs to financial pressure.
With the Beemium [subscription](https://www.beeminder.com/premium), you can set a pledge cap of $0 on any goal.  While these goals still technically _have_ pledges, a $0 derailment costs $0, so you won't bee charged for any of the goal's derailments!

Of course, you can adjust the $0 pledge cap to put a "real" pledge on the goal anytime, if you change your mind later.  The reverse is also true -- you can step down an existing goal's pledge to $0, then cap it there.

#### How do I subscribe (or cancel my subscription)?
Visit the [subscription](https://www.beeminder.com/premium) page, linked in the top navigation under 'Premium'.

#### What is the slider on the subscription page for?
You can use the slider to get a [discounted](http://blog.beeminder.com/fair/) subscription cost.  If you opt to pay larger amounts less frequently, we'll give you a discount over what you'd end up paying on a regular monthly subscription.  Longer payment interval = larger discount!  You can also buy a lifetime subscription for a one-time charge.

#### What are these 'auto-canceling subscriptions' I've seen mentioned?
If you don't use Beeminder for 30 days in a row (TODO: clarify condition), we'll send you an email letting you know your subscription is on hold, and we'll stop charging you for it.  If you return and start beeminding again (TODO: clarify condition), your subscription will reactivate and the charges will begin at the same frequency as before.

#### What if I buy a lifetime subscription at one level, and then want to change levels?
We’ve thought of and coded for a ton of corner cases, so making your change via the subscription page should be sufficient.  If you encounter any problems or have questions about what will happen, please [contact support](https://www.beeminder.com/contact)!  We’ll make sure the exquisitely fair thing happens no matter what.

#### What payment methods can I use?
Credit card or PayPal.  We use [Stripe](https://www.stripe.com) for processing credit card transactions.  

You can store information for one or both methods.  If you've entered both, we'll ask you to pick a default that will be used for any charges made.

#### How do I update my payment information?
Visit the [Payments](https://www.beeminder.com/payment) page, linked in the top navigation dropdown.

#### Beeminder charged my credit card, but I don't know why.
Also on the [Payments](https://www.beeminder.com/payment) page, you can see all the past charges we've made, from all sources - derailments, subscriptions, GTBee, IFTTT charge action, and the charge endpoint of the Beeminder API.  Each charge is either paid, failed, or refunded.  Failed charges may be listed multiple times - once it's failed, it won't update to paid; a new charge with the same information is created & tried.

Note that derailment charges are usually listed for one day _after_ you actually derailed on the goal, due to the 24-hour legitimacy check lag between the derailment & the charge being processed.

#### What happens if the charge fails?
First thing, we'll send you an email about it, which you can reply to.  We get those replies in support and can take the conversation from there!

We'll also place a flag on your account that hides the graph images (**BUT DOES NOT DEACTIVATE YOUR GOALS**) until the failed charge succeeds.  We automatically retry the charge one more time 24 hours later.  If the second try succeeds, the flag is lifted and you're back to beesness as usual.  If not, the flag remains.

After that, the only way to clear the flag is to update your card info.  If your card info is still valid and the charge failed for other mysterious reasons (which does happen!), [send us an email](https://www.beeminder.com/contact) in support and we'll help out.
