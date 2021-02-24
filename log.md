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

### Day 7 though 9: 15 December 2019, Sunday ... 27 December 2019 Friday

**Today's Progress**: Worked on stuff 3 days out of this entire time period. Blew the challenge. Going to keep going, keep working, keep logging anyway.

Day 7:  Went back over documentation to find statuses and created state classes for them. Looked at doing transitions. Read the code for @spatie_be‘s state & transition package. Went down a 'maybe I should be a product manager' rabbit hole...

Day 8:  Did something stupid and lost all my model files. Ouch. Looked into doing recovery. Fn00b stepped in when I was tearing my hair out and helped out. She found slightly old by a few days versions of them. Definitely lost some stuff, but couldn't at the time figure out what it was.

Many days pass here... Depression... Got kicked out of band... Holidays... etc.

Day 9:  Returned to working on stuff. Wrote a tweet about getting back on the horse, but it sounded like a pity party, so I deleted it. The upshot is I'm going to keep going despite missing days and too bad if people don't like it. It's not our failures that define us, it's how quickly we pick our selves up and keep going. This was a major drop that I hope to not repeat.

**Thoughts** Too numerous to mention.

**Link(s) to work** None

More days pass here... Getting past the depression... Found a new band...

### What I'm Calling Day 10: 5 January 2020, Satruday

Did my first CTF... Lots of problem solving. Writing scripts in Powershell which I've never done.

**Link(s) to work**
1. [Update tweet](https://twitter.com/phillipsharring/status/1214064680978829312)
1. [Windows Log Analysis: Determine Attacker Technique](https://twitter.com/phillipsharring/status/1213614098090463234)
1. [Windows Log Analysis: Evaluate Attack Outcome](https://twitter.com/phillipsharring/status/1213614071330885633)
1. [Escape Ed Challenge](https://twitter.com/phillipsharring/status/1213614046106267653)
1. [Found the Turtle Doves](https://twitter.com/phillipsharring/status/1213614019283685376) Not really a challenge, you just walk around and find them... but I _did it!_
1. [Linux Path Challenge](https://twitter.com/phillipsharring/status/1213583414982524928)
1. [X-Mas Cheer Laser Challenge](https://twitter.com/phillipsharring/status/1214066937707343872) INSANELY difficult, took many hints
1. [Frosty Keypad Challenge](https://twitter.com/phillipsharring/status/1213583346942533633) I guessed
1. [GreyLog Challenge](https://twitter.com/phillipsharring/status/1213583138628210688?s=20) super difficult for me

### Day 11: 6 January 2020, Sunday

**Today's Progress**: Re-ran my seeders and my requests that were saved in Postman and discovered some of the things that I lost when the model files got rolled back. Re-created most of it. Continued to work. Added a few more endpoints. Fixed a bunch of little things that I disovered through testing. Cleaned up the Seed data and the Postman requests so they kind of compliment each other. Postman stuff picks up where they seeds leave off.

Unrelated to that project, I was looking around in GitHub and found a weird pull request. It's from their Dependabot. Notified me of some security vulnerabilities and outdated versions. Pretty neat. Merged one and resolved the other myself.

**Thoughts** Was frustrated by having to recreate stuff, which is part of what I was depressed about up there... but I think I'm past that now and back to where I was and then some. Yeah, I missed more days in there. But I'm just going to go forward and count the next day when I get to it. I'm still shooting to get to 100 and I'm still going to try and do them consecutively. I have an intense urge to finish this dang thing and put it in front of people. Maybe it could be a product and I could quit the old day job eventually. I love where I'm working now, but I don't want to be at the whims of an employer any longer than necessary. I feel like for the work I've been doing I haven't made a lot of visible progress, since it's all API, which makes it feel like I'm not really accomplishing anything... but I know I am, and it will pay off when putting the front-end together. Just keep swimming...

**Link(s) to work**
1. Proprietary hustle, still. [Here's the update tweet, though](https://twitter.com/phillipsharring/status/1214065125512155136)

## 2020... Kind of a blur

**Progress**: At least 200+ days of code at the day job in here. I wish I could say 50 good days of side hustle coding, but I don't think that's true, sadly. 30, maybe? Made slow, slow progress on that front. Was shooting for a working demo by April... annnd I'm still working on that. Got a new job in August, which was a _HUGE_ relief. Have really been challenged and grown as a developer since starting there. Got _way_ into containers. Got deeper into front-end. Learned some basic ReactJS. Got deeper into Symfony. Started seriously on AppSec w/ some books, esp. at Christmas time. Got _really_ into containers and finally grocked it. Basically I've stopped using Laragon all together.

**Thoughts**: I mean, The Pandemic, am I right? Still hate Doctrine with a blind passion. Rough year. Got through it. Got married along the way, yay!

## 2021

**Progress this year so far**:  Finally figured out WSL, docker on WSL, and all that jazz. Loving it. Loving it loving it loving it. Will never go back. Fell out of love w/ InertiaJS and TailwindCSS (sorry, folks!) Learned NuxtJS. Been using it to revamp the side hustle and my personal site. Launched the personal site, hooray! Went back to having a separate front-end and a _real_ API for the side project. So, obviously, I'm leaving out a _lot_ of detail here, but that kind of brings us up to...

Day...? I don't know? Let's call it... (checks notes) 12?!

### Day 12: 23 February 2021, Tuesday

**Today's Progress** Good day, and welcome to day twelve. Was sick today; didn't do the day job. Wanted to stay in bed. Tooth broke, though, so I had to hit the dentist :-( boo. I was kind of awake after that so I ended up doing some coding. I slapped together a landing page for a sort of "family/team" domain I have w/ my wife, and added a view source page to my shiny new personal NuxtJS website rebuild that I launched recently. I want to do an obligatory "how I redid my blog" post w/ info on what/how/why I did things the way I did. Anyways. Good to dust this off again, again, again for the upmteenth time...

**Link(s) to work**
1. The view source commit [36f9bbec](https://gitlab.com/phillipsharring/phillipharrington.com/-/commit/36f9bbecd02b265372069521cc8c1dd920b3a741).

