# Speaker README

Hey there! Thanks for speaking at ACM Hack's first-ever "Learn.js" spring event. We're super excited to have you present with us. Before you prepare your presentation though, let's go over the structure of the event and some helpful tips of the trade.

## Structure

So far, the workshops have been an hour long and in that case, the traditional schedule of time has gone as follows:

1. Introductions - *10 minutes*
   1. Event title and speaker name
   2. GitHub repo link (where to find the code for the demo (more on that later))
   3. Membership attendance code (ACM gives our members points for attending our events; don't worry we'll take care of that!)
   4. What the workshop is covering, a description of what it is, and what it's used for
2. Code-Along - *20 minutes*
   1. To introduce the subject being covered, we like to have our attendees follow along with our speaker as they go over all or most of the material used in the demo
   2. It's ideal that the material is covered in isolation from the demo *i.e.* none of the actual code in the code-along is repeated in the demo
   3. For example, for the first workshop covering a basic introduction to JavaScript syntax, we first went over declaring variables, then some basic data types, `if-else` statements, arrays, `for` loops, and finally functions and objects. 
   4. For the workshop on HTML Templating in Handlebars, our speaker had the attendees build a simpler web page than the demo, but using all the same concepts.
3. Kahoot - *10 minutes*
   1. [Kahoot](https://kahoot.com/) is a website that allows you to create short quizzes that people can join by entering a short code and compete against each other in real time. 
   2. Hack in particular likes to have 4 questions for each workshop with the questions being somewhere between easy enough to answer and hard enough to differentiate who paid attention to the code-along and who didn't. This is useful for...
   3. Prizes! We use Kahoot, yes, for seeing who paid attention, but mostly to get the top 3 of the crowd so we can give out prizes to the winners. For the remaining sessions, the first place winner will get a \$15 Amazon gift card and the second and third will get \$10.
4. Demo - *20 minutes*
   1. The heart of every workshop is the demo. This is where the attendees get to build something using the technology being taught. However, because the demo is so key, there's a bit more that goes into it, which I'll detail right below.
   2. First off is making sure to plan for the time given. Making something cool is, well, cool, but make sure to cater both to the time and the level of proficiency of the audience. For the first workshop, for example, we made a clock that changed color depending on the time. This is a good demo because it's really visual and colorful and something they could show their friends after and say "I built that!" But we only had them actually write the code to get the current time, format that depending on 12-/24-hour format, and then pass the data to a *boilerplated* function that did all the decimal to hexadecimal conversions. This brings us to the next point...
   3. Boilerplate code! To both save time and really cut down and focus **just** on the new material being covered, we like to boilerplate any code that's not relevant for the workshop. So, using the example above, all the HTML and CSS code, as well as the decimal to hex function, were boilerplated. Or, for our second workshop covering features introduced to JavaScript since ES6+, we built a game of tic-tac-toe. For this, all the code to display elements on the screen, as well as HTML and CSS, were boilerplated to save lots of time and really just focus on ES6+ and new features. (This also has the added benefit of giving everyone there more of a level playing field.)
   4. Explain, explain, explain! It really is the "little things" that make or break a workshop. Giving helpful analogies, explanations, or acknowledgments of complicated syntax or daunting undertakings help the attendees feel closer to the speaker and more likely to ask questions and participate. 
   5. You'll have two different folders: one with "starter" code and one with "final" code. This is so the attendees can troubleshoot and compare if they get stuck and have a guaranteed working copy to reference. 

However, even with all of that said, if you're reading this, then chances are your workshop won't be an hour, but actually an hour and a half. In this case, allocate the time as you see fit! If you want to spend more time in the code-along than the demo, feel free! Or if your demo is a little more ambitious, then spend your extra time there. You could even spend it in the introduction, going over a more high-level overview of the topic than a complex implementation. Whatever you decide, try to run it by us before you invest a lot of effort into it!

## Tips

- Since this document is intended for speakers with a bit more advanced topics, we at Hack have talked it over and decided that it would be better to spend more time discussing the high-level applications, overview, and explanations of your topic and build something cool, but not excessively complicated. Where the line is drawn between those two is up to you!
- Visual, practical, and enjoyable demos are heavily preferred! The first workshop was colorful and changed every second for a striking and enticing introduction to JavaScript (and programming in general for some!). The second workshop allowed attendees to interact and play along with a game they were all familiar with, something they could even play with their friends! The third workshop, the most advanced and perhaps distant to many, used Marvel's new movie *Infinity War* to make HTML templating seem more in the reach and applicable to our attendees than it was before. It's innovative and just plain **fun** projects like this that we really appreciate.
- ACM Hack always strives to be beginner-friendly and bridge the gap between computer science experts and the interested, but inexperienced. Keeping this in mind, try to speak and move along through the workshop as you would like someone to do if you were a newcomer as well!
- Pause and explain, pause and explain, explain and pause! We have a lot of beginners at workshops and the very last thing we want to do is leave our coders behind! I mentioned this previously, but try to make even the most complex and computer science-y topics seem approachable and useful in everyday life.
  - "Humanizing" the code can be helpful. Things like "So what this for loop is does is **say** '**hey**, we have this counter `i` that we use to…'" (examples bolded)
  - Analogies! It might be more understandable if you explain a server like a server at a restaurant. Maybe the client is the customer eating. Or could you compare React components to furniture in a living room? And you can make new rooms by changing the position or color or material of this furniture. These are not at all necessary, but can be something to keep in mind!
  - Applications. Does Facebook use this (*cough cough React*)? Is this how emails are personalized? Could you use this to broadcast pictures of your cat? Tell us all about how we can use this when this workshop is over!
- Introduce the mentors to our attendees and give frequent reminders that we are here to help and answer any and all questions they may have!

## Logistics

Every workshop will be given in Covel 227, which is a medium-sized auditorium-style room. There will be several rows of tables where attendees will sit and face a large projector screen. This is where your computer screen will be projected. 

You will have access to an additional computer up at the podium for you to read from for your speaker notes, should you choose to have them. We recommend speaker notes to keep you on track and note any helpful examples you think of before presenting. Speaker notes can cover everything from the introductions to the demo, but are especially useful during the code-along. If you would like an example, I have uploaded mine from the first workshop in this repo titled `ExampleSpeakerNotes.md`.

Every workshop requires a README, which are step-by-step instructions anybody could follow and create the exact demo shown in the "final code" folder. Screenshots, code snippets, and little progress check-ups are good!

I personally use a free application called "Typora" to create my Markdown READMEs. You can download it [here](https://typora.io/), but feel free obviously to use any method that works for you.

[See first workshop example here](https://github.com/acm-learnjs-sp18/intro-to-js-1/blob/master/README.md)

[See second workshop example here](https://github.com/acm-learnjs-sp18/new-javascript-features/blob/master/README.md)

After you create your project (with starter and final folders) please create a GitHub repo for it! We will then clone the repo, and add a remote titled `acm` so that the repo can be displayed on ACM Hack's official GitHub and the Learn.js organization. 
