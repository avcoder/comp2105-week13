# Hand out Hiro markers

- Hand out Hiro markers to everyone

# What is AR?

- you have 2 sides of the spectrum
- left side is reality
- right side is virtual reality
- everything in between that is mixed reality
- AR fits in that category of MR, it's just closer to reality side
- so when you see thru you phone/browser, you see reality, but in addition to reality, you see additional objects that are displayed as well
- read it
- field is relatively new

# Ikea place app

- to show you some examples, Ikea has made this app
- play video
- if you download their app, you can see their furniture in your room so you can see how it looks on your carpet, you can turn it around, change colours
- so you're not surprised when you buy their furniture
- cool example to see if potential furniture fits in your decor

# ar.js - gaming

- this is a gaming one, forward to 1:20
- so here's a game, where you're viewing your table, but in addition your table, you're seeing supplemented objects
- you can manipulate those objects in order to win the game
- now it's using a marker and I've given you each a marker
- I think he's trying to get the laser to point to a certain location in order to get the missile to launch

# AR in edu

- pictures of what is happening right now
- left example uses markers. Right one doesn't

# AR for many fields

- can be used for many industries
- if you require safety , you can potentially wear these goggles so it gives you info about what you're about to touch so you don't explode the building
- or if you're shopping, it'll tell you more info about the product

# Waves

- this company has researched the different kinds of technologies that have propelled the tech industry
- so at first back in the 70s 80s, you have the PC - that's what revolutionized the computing world
- then you had the internet and that's what propelled it even further
- then you had mobile
- they think AR/VR is the next big thing, if that's true this is going to be huge

# gartner graph

- this is a company who annually tracks tech trends
- they can predict how long it will stabilize in the market, or if it will fall of the face of the earth never to be seen again
- this is called the hype cycle (for example...)
- everything on this down slope is on the decline
- but in order to stabilize in the market it has to reach here - the end of the line
- where is AR? it's here. that may concern you but it's not dropping of face of earth because if it were it would go down even further
- so it is making a turn
- some a predicting it will overtake VR

# ar.js

- history
- There's this guy named Jerome Etienne who created ar.js and his mission was to bring AR to the web
- because he didn't like the fact that AR required you to download something
- read the benefits
- so that was early 2017

# June 2017

- middle of 2017 Apple creaetd ARKit
- read it
- this was a bombshell because you didn't require markers anymore - this was the first that had markerless tracking
- hit testing - means this has the ability thru your phone, it'll scan the ground, it'll know that's the ground, and it'll place your object on the ground, in proportion
- was available for a monocular camera click next slide

# monocular camera

- thru glasses he's seeing additional info in order to do his job correctly
- this one was craeted by MS called Hololens
- all kinds of monocular glasses being created right now

# fast forward to Aug 2017

- Google replied back with ARCore
- read it

# Google's ARCore vs Apple ARKit

- so now you have 2 main competitors, Google's ARCore, vs Apple's ARKit
- both were very good
- Apple no longer had monopoly with AR, which is good due to more competition
- however, read it

# Google exposed AR on the Web

- Google did something nice. They exposed ARCore and ARKit to the web
- so google created WebARonARCore and WebARonARKit
- so now those 2 new technologies are open on the web
  -the following slides are examples

# ARCore example (portal)

- play video
- so here is an example of a door/portal where you magically step thru and you're in another location

# ARCore example (robots)

- play video

# As a resopnse ar.js has evolved

- so once all that happened within 2017
- the creator of ar.js asked deep questions - where does ar.js fit now?
- he made ar.js available in something called A-Frame which we'll look at in a moment
- read it
- a lot of the different AR platforms out there (either free/paid), they use ar.js

# A-Frame

- think of a-frame as a bunch of custom html tags that allow you to created 3D objects in the augmented world
- read it
- click link - cool thing is you can turn around, press return to toggle camera,
- take a look a their hello world - this example is kind of what we'll do in our in-class exercise today
- take a look at their docs - this is the special markup tags that a-frame has created
- so basically create a scene via `<a-scene>` and then place objects

# tracking

- there are 5 different kinds of tracking
- the one you'll play with today is marker tracking, that's when you have a piece of paper and the computer will recognize that pattern on that piece of paper and orient the object on that paper appropriately
- Geo tracking - pokemon
- face tracking - is totally different than face recognition - face tracking is simpler - it's locating your eyes/nose so you can place objects appropriately

# Intro to ar.js and A-frame

- your turn to play
- fork this codepen
- we'll go step by step, and hopefully you'll see something on your screen where you'll get a wow factor

# Step 1

- so what we're doing here, is we're adding a scene
- other libraries like three.js have a similar kind of thing
- A-frame is built on top of three.js

# Step 2

- add a-marker
- What are you saying thru this line is: preset='hiro' means
- hey camera i want you to recognize this hiro image and when it's flashed on screen then do something

# Step 3

- Add a-box
- notice the position has an x y z coordinate

# Step 4

- Final step, show the marker to your webcam
- now I created a link here tiny.cc/hiro - you can actually use your phone if the paper method isn't working
- so I can turn the cube
- play with that, I'll walk around to see if you got it working

# change colour

- next challenge - try changing the colour
- hint: I've given you a link here

# change opacity

- next challenge - try changing opacity

# for the next 20 minutes

- I want you to play by trying out these different objects
- so far you have experience by adding a box
- but check it out, you can add a sphere, cylinder, plane, text
- try replacing the box with one of these
- try a combo of objects
- try changing attributes
- try adding your own image
- add your initials or name

# Glossary

- click link "Quick dirty guide to AR terms you need to know"
- "Extended Reality" encapsulates AR/Vr
- focus on glTF - read it, this is the one you want to gravitate toward which will allow you to export your models like this
- click link "3d content on fb" - fb announces support for glTF 2.0 on their fb feeds
- so this is glTF which you can import in A-frame

# webxr.io

-

# visually update purple page

- topic: Performance
- If you are going to animate something, you should use these 2 props: transform and opacity
- whenever the browser has to update its look, it has to do 3 to 4 things:
- 1. calculate styles
- 2. layout (Read it)
- 3. (read it)
- 4. composite (read it)
- So when you animate, be aware that some props require going through all of these steps when they're changed, and some don't
- so the fewer steps the better, more performant

# Performance

- [click link] csstriggers.com
- this website shows you a comparison of Chrome(blink), Firefox(Gecko), Safari(WebKit), Edge(EdgeHTML)
- it's showing you the different phases that the browser uses
- so take the 1st one: align-content; for Chrome it's very expensive if align-content changes
- how about background-position
- let's take a look at the best 2: transform here it's only affecting the composite layer, so it's the least amount of work for the browser - which makes it better for performance. For opacity it's 2, or 1 for if it was already changed before
- so that's something to keep in mind when you're doing animations

# Val Head quote

- read it

# cat codepen exercise

- so with that in mind
- I want you to optimize this sprite animation
- To do that I want you to replace the background-position, with a transform
- instead of having a `<div class="tuna"></div>`, add an img tag then do a transform on that img tag

  1. Create an img tag inside div whose src replaces the background img
  1. No longer need CSS background prop
  1. Hide other cats `overflow: hidden` (make it obvious via `border: 1px solid black`)
  1. Modify keyframe from `background-position` to `transform: translateY(-2400px)`
  1. remove `animation` statement from .tuna block, paste to new img { animation: ... }

  ```css
  .tuna {
    /* use the timing function steps() to chunk the animation into 12 equal pieces */
    /*   background: url(http://stash.rachelnabors.com/animation-workshop/sprite_catwalk.png) 0 0 no-repeat;  */
    height: 200px;
    width: 400px;
    margin: 100px auto 0;
    border: 1px solid black;
    overflow: hidden;
  }

  img {
    animation: 1s walk steps(12) infinite;
  }

  /_ Don't forget: You'll need an @keyframes block to change the background image's position! _/

  @keyframes walk {
    to { transform: translateY(-2400px) }
  }
  ```

# 4 things browser animate cheap

- read it
- What's the 1 thing missing from that list of transforms?
- translate3d() is a hack and is replaced by the prop will-change

# youtube vid side-by-side

- this is in slow motion, they recorded it in 240 frames per second
- so on left side, it's very jerky because browser is expensively calculating everything

# Chrome Devtools

- Performance tab
- Try Firefox for waterfall
