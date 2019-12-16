# 100 Days Of Code - Log

<!--
### Day 0: February 30, 2016 (Example 1)
##### (delete me or comment me out)

**Today's Progress**: Fixed CSS, worked on canvas functionality for the app.

**Thoughts:** I really struggled with CSS, but, overall, I feel like I am slowly getting better at it. Canvas is still new for me, but I managed to figure out some basic functionality.

**Link to work:** [Calculator App](http://www.example.com)

### Day 0: February 30, 2016 (Example 2)
##### (delete me or comment me out)

**Today's Progress**: Fixed CSS, worked on canvas functionality for the app.

**Thoughts**: I really struggled with CSS, but, overall, I feel like I am slowly getting better at it. Canvas is still new for me, but I managed to figure out some basic functionality.

**Link(s) to work**: [Calculator App](http://www.example.com)
-->


### Day 1: 10 December 2019, Tuesday

**Today's Progress**: I figured out what was wonky w/ the route model binding in API routes. I fleshed out some basic endpoints for the orgs. There's index, store, show & update now. I also debugged and finished the add-employee endpoint.

**Thoughts** I didn't realize Route::bind _doesn't work at all_ w/o the SubstituteBindings middleware. My band unexpectedly kicked me out, so maybe this is a good time to have 100 days of code in my life, too :) Going to try and figure out if there's any way I can share code from what I'm working on when it's the proprietary hustle thing.

**Link(s) to work**
1. Proprietary hustle. [Here's the update tweet, though](https://twitter.com/phillipsharring/status/1204625328532000768)


### Day 2: 11 December 2019, Wednesday

**Today's Progress**: I extended the basic User class in App\User into App\Models\Employee, moved all of the custom relationships from App\User to App\Model\Employee, and updated any reference to App\User to App\Models\Employee in the relationships in other Models. Tweaked the relationship functions inside Employee so they work (since some key assumptions changed now that the class name changed; and some were just plain wrong). Made an endpoint for employees/{id}/reports to post a new report along w/ the Request, Dto & Action.

**Thoughts** It's weird how Larave's compound routes something/{id}/child get named automatically, or I'm doing it wrong (likely), but it's appending the ".child" and leaving out the "something." But if you add 'as' => 'something.child' then it ends up 'something.child.child' so you just have to say 'as' => 'something,' which is somewhat unintuitive.

**Link(s) to work**
1. Proprietary hustle, still. [Here's the update tweet, though](https://twitter.com/phillipsharring/status/1204970946848870401)

### Day 3: 12 December 2019, Thursday

**Today's Progress**: Worked day job until the afternoon, then me and the soon-to-be mrs. got dolled up and drove the 3 hours to Charlotte for the day job company holiday party. Was a success. Grabbed dinner. Headed back the 3 hours. Got in around 1:40 and to sleep by about 2am. Upshot:  missed today.

### Day 4: 13 December 2019, Friday

**Today's Progress**: Super "jet lagged" from being up til 2 last night and back at work this morning. I created one and a half end-points. One for 'set manager' (the inverse of 'add report') and started work on 'create thought' endpoint, which will have some moving parts due to the multiple models that are rouched. Went almost an hour. Pooped out. Brain tracks could not hold trains of thought...

**Thoughts** Very few at the moment :)

**Link(s) to work**
1. Proprietary hustle, still. [Here's the update tweet, though](https://twitter.com/phillipsharring/status/1205725144922112000)

### Day 5: 14 December 2019, Saturday

**Today's Progress**: Finished 'create thought'. Did 'add verison of thought' end point.

**Thoughts** If we added demographics to "employees" in this thing, we could run queries like breakdowns of problems validated/rejected, positive/negative feedback, etc. by the demographics. Wondering how to make that work. If it should be optional or what. Definitely should be invisible in the interface except to the user filling out the demographic info and in the aggregate data. Could be an interesting tool for some conversations.

**Link(s) to work**
1. Proprietary hustle, still. [Here's the update tweet, though](https://twitter.com/phillipsharring/status/1206084938975592448)

### Day 6: 15 December 2019, Sunday

**Today's Progress**: Finished 'add version of thought'. Completed 'Add development to thought'. Realized the model/code for adding a development assumed the "sender" would always be who created the thought and fixed that.

**Thoughts** Realized I didn't need a couple of the endpoints I had in my list. Don't need 'send thought' - because it's basically an alias of 'send development on thought,' and I don't need 'add verion of element' because that's handled in 'add version of thought...' Nice to not have to do those, but I want to go through the UI docs and see if I'm missing API endpoints. Had some innter turmoil about having the 'add a development' endpoint be just POST developments OR POST thoughts/{thought id}/developments and went with the latter because that URL space can have a few other HTTP verbs on it for stuff we'll need, like a list of developments on a given thought.

**Link(s) to work**
1. Proprietary hustle, still. [Here's the update tweet, though](https://twitter.com/phillipsharring/status/1206438698830749696)
