
### HTML/CSS Project 

This project is inspired by Scrimba's [HTML/CSS course](https://scrimba.com/learn/htmlandcss).

I already knew HTML/CSS but, besides the fact that I am constantly questioning my skills, I wanted to see if I was missing anything by not learning it "formally". I went through the whole course in about 4-5 hours including participating in some of the challenges to test my memory and improve my typing skills. Everything covered was something I had previously used, but I did happily learn some things about [centering items](https://stackoverflow.com/questions/114543/how-to-horizontally-center-an-element/46449757#:~:text=If%20the%20element%20is%20a,element%20to%20the%20centre%20horizontally.) and flexbox. 

I'd always kinda just played around with ```display: block``` and ```display:inline``` until it looked like how I wanted, but never really knew why somethings worked or didn't. I mean obviously it wasn't necessary to know, per se, since I eventually figured it out, but this will hopefully make things faster for me. 

* If you are using the ```margin:auto``` way to center things, then this assumes your item is a ```block``` type and has a fixed ```width``` [^1]
* Now some flexbox properties [^2]

```display:flex;``` Puts items in one row. Can also be inline or block  
```flex-direction: column; ```Default is row. Puts all items in one column.  

The below properties change based on flex-direction. If row then horizontally, vertically respectively. Vise versa if column.  

```justify-content: center; ``` Centers the item horizontally. Can also be start, end, space-between, space-around   
```align-items: center; ``` Aligns an item vertically. 
						Default is stretch (will make the item take up the whole vertical space of its container). 

All in all, I think the course is good (I actually really like the platform) and am definitely considering taking other courses and its **free!!**

[^1]: https://scrimba.com/learn/htmlandcss/centering-our-content-coc8f40f3ba676d118f92dd90
[^2]: https://scrimba.com/learn/htmlandcss/aside-align-items-co18d42cea92baec20fc830af


# Project Goal

The **final project** for this course is to make a site advertising your hometown. I don't particularly care about my hometown but I would love to travel more. I also want to challenge myself a little. 

Currently I have two ideas:
* Make a site advertising somewhere I want to go (e.g. Peru, Colombia) and 
* Make a site documenting my Trip to Tanzania

I'm kind of leaning towards the latter at the moment because I think it would be fun to recount and, also, my professor wanted something like this so he could advertise the trip to interested students (it was an abroad semester).

I love reading travel blogs and here are some that I like:
[Peru - Salt in our Hair](https://www.saltinourhair.com/peru/), [Peru - A Blonde Abroad](https://www.theblondeabroad.com/ultimate-peru-travel-guide/), [Peru - Along Dusty Roads](https://www.alongdustyroads.com/peru), and [Peru - Nomadic Matt](https://www.nomadicmatt.com/travel-guides/peru-travel-tips/) (if you can't tell, I'd really like to go to Peru).

I also want to document this experience, I tend to be very forgetful. I can't remember projects I worked on for class from under a year ago -- at all. Of course, if I go back and I look at the code, I'll get flashback to working on it and the people I worked on it with, but I can't remember specifics. When I talk about these projects, or put them on my resume, I just look silly or like I didn't do what I said I did, which isn't the case at all (very long hours on those projects let me tell you). 

Everyday that I work on this, I'm going to document my **goal for the day, anything I got stuck on, and if I finished the goal**. If I finish the goal, then I'll iterate. I also tend to get analysis paralysis, so I'll document any of that too.

Update: I've realized that I had already named the repo travel-tanzania so I suppose I've made my choice

## day by day

### Jul 11, 2022

I [picked out](https://www.figma.com/file/Amzww2cEqJLnrUdIniNzjS/travel-tanzania?node-id=0%3A1) different features I liked from the inspo and so it's time to start... woo

So... I didn't really set a goal... but I did the hero banner thing. I'm just doing a simple one: a background image and a title. 

- [ ] Eventually I'd like to be able to do the shape masks like the Salt in our Hair blog

 but that's a little out of my scope right now. 



This next section I'm not really sure what I want to put in it or how I want to arrange it.

I would like to have   
- [x] A **table of contents** since I predict this is going to be a pretty long page  
- [ ] I want the little **interactive world map**,   
- [x]  **My itinerary**  
- [x]  Maybe like a **list of different regions** in TZ. 

but thats a bit much for one screen I think. Oh! idea 

- [ ]  The interactive world map could be a map of Tanzania separated by region, each region could be highlighted.  
- [ ] I think I would have to make my own SVG of Tanzania + its regions (i doubt it already exists)
    - [ ] OR I don't need to  separate by region, just have a PIN that shows up when you hover...

Ok I'm trying to just get a picture of a map to look like a polaroid and I don't know how to get it so that the border proportionally scales with the size of the map. 

- [ ] look up how to make a polaroid in css?
-- I actually decided I don't want to do this.

Alright I blocked out the content for the second page. 

- [ ] Make the flex box better responsive for smaller screens. Maybe ```flex-dir: column``` if screen too small?

Good lord, every time I work with flex boxes I get this problem. Theres left/right scrolling because it overflows and I never remember how I fix it. 😑  
-- Oh, oops I got it I just had a weird margin somewhere.

- [ ] Ew the pins are ugly. Get some icon to replace that rip

Ok... she's kinda ugly, honestly the only thing **really** bothering me is the map. Its a bit crammed I think...

- [x] Un-cram map
- [ ] Write the overview paragraphs ...
- [x] learn how to put elements on top of each other? (e.g. the list of regions on top of map)  
-- 😯 You can have ```negative margins```!! Is this the best way to do it? Ok now how do I bring to front... Ok to do **stacking** you have to use ```z-index``` and specify the ```position: relative```
- [x] Small irritation either Kilimanjaro shouldn't be underlined

I'm actually fairly happy with how it looks right now. I mean its not the prettiest, but its pretty good? 

- [ ] Eventually make all of the list stuff clickable anchors

Should I be linking pictures of my updates ? TBD

Ok my next **goal** is literally just to type, I wish VS Code had spell check 😩 (just installed one). I remember when I was working with react I could just type in a "data" page or something and then import but I'm not sure if this is possible with just HTML/CSS ?

- [ ] I'd like to have my color theme be variables in case i want to change it i don't have to manually change it everywhere

- [ ] I can't figure out how to get text on the baseline for the top things to do
- [ ] Eventually animate the cards to flip

Its technically the next day, but I haven't pushed yesterdays changes yet. 

Pictures to include (Dar)
- [x] rooftop bar sunset picture
- [x] city picture
- [x] village museum
- [x] ugali
- [x] war games 1
- [x] tuk tuk picture

### Jul 12, 2022

I need to commit to git more. What is standard ? I tend to only commit when I finish a page/would be ready to push...

Alright todays goal is:
> import the pictures you need for Dar (and formatting) [done!]

> iv decided that I want the locations to alternate alignment (Dar: left, Z: right, A: left) and every other section on the left so fix that formatting 
-- actually i lied, I don't mind them all being the same

- [ ] Add a scroll to top button that directs to table of contents

Pictures for Zanzibar:
- [x]  of the hotel 
- [x] (maybe a sunset/rise picture)
- [x] stone town architecture
- [x] jozani forest 
- [x] horses
- [x] turtles

Time for Arusha + National Parks Content. Writing takes so long ;-; and I need to go back and edit because i'm sure some things are wrong. 

At this point this has become more of a writing challenge than an HTML/CSS challenge...


I suppose once I finish the content I can go back and spruce it up? I do have things marked that I want to do... We'll see

- [ ] add carousel for each region of cool places
- [ ] add list of everything you packed? a
    - [ ] a cute like animated backpack would be adorable like you hover and it shows 
- [ ] the about page/content (i hat writing about myself !!!)
- [ ] add a footer with socials and idk what else is usually in the footer?

 Next goal? Check off all the things I haven't done yet ! Lol ok 

 realistically ? idk. I'm going to go eat.

 OMG I wanna cry what is this **MESS** I just [deployed](https://n-buckley.github.io/travel-tanzania/) it on GitHub pages and for 1 half of my images aren't showing up on google chrome and on safari the css isn't even being applied to them?? cuz they're not scaled at all!! I'm literally so mad idk what to do.

 Ok the safari page and chrome page look the same now, I didn't really change much or anything really. I think it was just glitching... but why aren't my pictures showing up??

 Another thing I've noticed is when I reload the page I can just see "Tanzania" with the shadow before the image loads... I guess is there a way to have a default background? 
 - [x] Look up how to fix this
 -- looks like it was just a [github pages problem](https://stackoverflow.com/questions/60048977/github-pages-images-wont-load-the-server-responded-with-a-404-for-the-image) (both issues the weird css and the images loading) I guess i should have had some more patience 😬

 - [ ] Go back and annotate the page with emojis. Any time you had a big problem 😡 something you learned 😯. Or maybe Ill type an overview/synopsis of my experience about day by day and keep this as authentic as possible

 I just looked at it on mobile... not great. Because I did most of the height sizing based on **vh** and the proportions of a window and a phone window aren't the same,,,, everything is very long.

 I suppose that just means I shouldn't use vh but what should I use ? I'm going to try converting all the vh to vw (and change the sizing) Ok changing it to vw made it more proportional, I do want the hero page to take up the whole front page tho so Ill change that back to vh. But I still don't love it idk if its the spacing or what? maybe the padding should also still be vh?
 
 Also the background image looks horrible its too zoomed in idk why that is? (on mobile).

 ### Jul 13, 2022

 Collection of easy tasks from above
 - [x] Eventually make all of the list stuff clickable anchors
 - [x] Ew the pins are ugly. Get some icon to replace that rip
 - [ ] I can't figure out how to get text on the baseline for the top things to do
 - [x] add list of everything you packed?
 - [ ] Write the overview paragraphs ...
 - [x] the about page/content (i hat writing about myself !!!)
 - [ ] add a footer with socials and idk what else is usually in the footer?
    - [ ] socials, copy write, sitemap, email thingy

 Things I don't know how to do but shouldn't be hard
 - [x] Add a scroll to top button that directs to table of contents
 - [x] Eventually animate the cards to flip
 - [ ] add carousel for each region of cool places
 - [ ] I'd like to have my color theme be variables in case i want to change it i don't have to manually change it everywhere 

 Things that I feel like are going to be hard
 - [ ] Eventually I'd like to be able to do the shape masks like the Salt in our Hair blog
 - [ ] I want the little **interactive world map**,
    - [ ]  The interactive world map could be a map of Tanzania separated by region, each region could be highlighted.  
    - [ ] I think I would have to make my own SVG of Tanzania + its regions (i doubt it already exists)
        - [ ] OR I don't need to  separate by region, just have a PIN that shows up when you hover...
 - [ ] a cute like animated backpack would be adorable like you hover and it shows what I packed

Mobile stuff (hard?)
- [ ] Make the flex box better responsive for smaller screens. Maybe ```flex-dir: column``` if screen too small?


I'm going to do this at the beginning of every day (make a collection of all the things I want to do)


<br>

__Task: Eventually make all of the list stuff clickable anchors__

I knew how to make the anchors so that was easy. But it wasn't scrolling to where I wanted it to. 

I wanted the titles of the places, when scrolled to, to be near the bottom of the screen because I wanted the whole picture to be visible.  
-- To offset that you need to change ```* {scoll-padding-top: x}``` so I was playing around with it but there was no happy medium between what I wanted for the locations versus the other headers. 
-- I changed the anchor to the images with just a little bit of scroll-padding and that achieves the same kind of result that I wanted. 
-- There are different ways to do it [it seems] (https://getpublii.com/blog/one-line-css-solution-to-prevent-anchor-links-from-scrolling-behind-a-sticky-header.html)

I also didn't like the harsh scroll
-- this was fixed by ```* {scoll-behavior:smooth}``` automatically, it just does a harsh jump.


<br>

__Task: Ew the pins are ugly. Get some icon to replace that rip__

Ok so I found an svg icon online thats nice enough.

- [ ] I cant get the pins on the baseline of the link
- [ ] id like for the svg to also change color when the anchor is hovered over

This is my second time not being able to find a baseline solution, so I'm going to move on.  


__Task: add list of everything you packed?__

I'm not really sure how I want to do this, so I'm just going to do it and see what happens.

Ok my computer's going to die but I just made lists of several categories. 

When I realized they were too big I wanted to limit the size of the containers so just made it a fixed height. That looked silly for the really small boxes so I found something called ```max-height: x;```

I don't love this solutions, it's just kind of basic, but at least the information is there

What I would like:
- [ ] just not this design think of something else

- [x] the background of the scroll thingy not to be white that's really annoying
- [ ] To have check boxes for each item so that users can check stuff off (it wouldn't disappear just become checked)
- [ ] Also you need to write about things that you needed like more warm clothes, more pants, explain about the detergent situation


I'm not sure if this is my impatience with Pages again, but the smooth scrolling isn't working on Safari (it is working on chrome).
On safari you also cant see the background color or scroll feature (max-heigh i'd assume) Uh... the pins are also like gigantic (for the regions....)
... again everything is working on chrome

<br>

__Task: the about page/content (i hat writing about myself !!!)__


Omg I discovered something :
```css 
width: 20%;
height: 20%;
border-radius: 50%;
padding-right: 5%;
```

Without the padding, its just a regular circle, but once I add the padding it makes like a weird oblong/triangle shape...  I'll look into this more later

I'm fine with this section, I don't really think it needs any changes but potentially add to my bio, it's kind of short. 


<br>
__Add a scroll to top button that directs to table of contents__

Ok yeah that was really easy. But better practice is to use JavaScript it seems. 
- [ ] Do the scroll to top in JavaScript  

<br>

__Task: (top things) animate the cards to flip__

Ok I need to get the pictures for each 

and write some text for when they flip ...


I've realized I'm just kind of hacking at this when looking it up would be easier...

I was trying to get the image for the cards behind the text, but ```z-index``` wasn't working by itself... So I ended up doing 
negative margins again. I don't know if this is best practice ? sigh

To do the cards I'm assuming there needs to be a hover property and there needs to be content _directly_ behind. So 
thats going to be another layering challenge if I do it the way I did before?

I ended up just [looking it up](https://www.w3schools.com/howto/tryit.asp?filename=tryhow_css_flip_card) even though I could have tried for a while that was definitely easier and faster.
Also it didn't involve any layering. 

Theres **4 divs** that need styling to get the card to flip :

The entire container for the whole card ```.flip-container```
Here you need to set the size for the card (so I just pasted what was previously my card container) but you also need ```perspective: 1000px;```
this animates the flip in 3d. It makes the card "stick out" like its an actual card flipping. Otherwise It kind of just rotates to the back) At small values it's really funny the card like sticks out of the screen (also takes longer to flip).

Then you need a div that contains the content for the front and back ```.flip-card``` which has two important things. 
```transition: transform 0.8s;``` which extends the time for the flip otherwise would just immediately flip to the back of the card  
```transform-style: preserve-3d;``` This actually flips to your back content. Otherwise it would just flip your front content by 180

Then theres a 180 flip on hover. And an important property is for the front/back content divs `backface-visibility: hidden;` which hides whatever the back for the card is and `position: absolute` or the cards would be stacked on each other like normal html. Other styling doesn't really matter

- [ ] I still need to write the back content but I don't want to rn

I'm tiring/getting burnt out with this project. Maybe its because i have no self regulation and I spent 10 hours on VS Code yesterday.

<br>

**Task: add carousel for each region of cool places**

You know what I started looking up how to do this and I found something a solution, but now that I think about it, I have about 20 places meant to be in one carousel ... 

i feel like thats not really practical for a user to shuffle through all of them. 

Ok. I thought of something, what if I do something like 'your books' in book reads where theres lots of tiny images and then you can hover over an image to see the title and maybe a very mini description... Yeah I'm going to roll with that.

_Task: Mini images with hover description_

Ok hm, I can store the description sin the title as a hack and it would automatically show it to me when I hovers. That would definitely be the easiest way. 

Ok.. Yeah I'm just going to do that a lot of the solutions I see make the text replace the image (kind of like the flip cards above, but I want it to hover off to the side (kind of like Goodreads does with book covers, if not exactly) which is pretty much what the title/tooltip does 

Actually I can just make a [tooltip class] (https://www.w3schools.com/css/css_tooltip.asp) instead of using title. This will also allow me to add more text.

- [ ] Oh! I remember now I wanted to be able to show a map where you could hover over all of the spots !! 

For now this is ok

Alright that was a lot of content 

- [ ] change the REALLy long links for something shorter

<br>

### Jul 22, 2022

I took a break for a little bit I wasn't really feeling great this past week (I can't believe its been a week)

Collection of easy tasks from above
 - [ ] I can't figure out how to get text on the baseline for the top things to do
 - [x] Write the overview paragraphs ...]
 - [x] add a footer with socials and idk what else is usually in the footer?
    - [x] socials, copyright, sitemap, email thingy
- [x] I still need to write the back card content but I don't want to rn
- [ ] change the REALLy long links for something shorter
- [x] Also you need to write about things that you needed like more warm clothes, more pants, explain about the detergent situation
- [x] add a favicon :)

 Things I don't know how to do but shouldn't be hard
- [ ] I'd like to have my color theme be variables in case i want to change it i don't have to manually change it everywhere 
- [ ] To have check boxes for each item so that users can check stuff off (it wouldn't disappear just become checked)
- [ ] id like for the svg to also change color when the anchor is hovered over
- [x] a lot of the % sized things, like the flip cards and the list of items to bring don't scale well 
-- the scroll boxes actually look fine on mobile after i fixed my spelling mistake and everything I've tried for the flip cards hasnt worked. ill try again when i specifically target mobile design

 Things that I feel like are going to be hard
 - [ ] Eventually I'd like to be able to do the shape masks like the Salt in our Hair blog
 - [ ] I want the little **interactive world map**,
    - [ ]  The interactive world map could be a map of Tanzania separated by region, each region could be highlighted.  
    - [ ] I think I would have to make my own SVG of Tanzania + its regions (i doubt it already exists)
        - [ ] OR I don't need to  separate by region, just have a PIN that shows up when you hover...
 - [ ] a cute like animated backpack would be adorable like you hover and it shows what I packed
 - for the other places to go:
    - [ ] show a map where you could hover over all of the spots/pins
    - or create a gallery of places that instead of overflowing vertical overflows horizontal and you can scroll
- [ ] Do the scroll to top in JavaScript  

Mobile stuff
- [ ] make the hero backgroundimage scroll if on mobile (otherwise gets blown out)
- [ ] try and get the text of the top things o do to be more easily readable on mobile


Making to dos like this is really annoying, I don't like having to collect them at the end of every day

I mostly just worked on content tonight I just wanted some content to get checked off, I will not be rewriting these tasks for tomorrow

### Jul 23, 2022

Just fixed a lot of spelling errors woo!