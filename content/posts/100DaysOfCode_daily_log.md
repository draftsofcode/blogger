---
title: "100 Days of Code Daily Log"
date: 2021-03-29T23:15:10-04:00
draft: false
listable: false
menu: main
---

# 100 Days Of Code - Log

### Day 1: Monday, March 29, 2021

**Today's Progress:** Wrote blog post announcing [#100DaysOfCode](https://www.100daysofcode.com/rules/).

**Thoughts:** Getting Hugo set up was pretty straightforward. However, I ran into challenges hosting on Render.com and decided to switch over to Netlify. My biggest challenge on Render.com is that after a few commits, it stopped watching the github repository and wouldn't rebuild the site. So, I switched over to Netlify which has, so far, rebuilt the site on every commit. 

The other interesting thing is that there is no way to change an image's size in generic Markdown. So, I ended up using the [figure](https://gohugo.io/content-management/shortcodes/#figure) shortcode which made this possible.

One other thing is that I wasn't able to get Google Analytics working yet. But, will definitely figure it out. May just need to modify the theme that I have been using.

Getting going and keeping going will likely be challenging. I just hope to get a straightforward playable version of the game going.

### Day 2: Tuesday, March 30, 2021

**Today's Progress:** Added Google Analytics and Newsletter signup to the blog homepage

**Thoughts:** Originally, I installed the [Mainroad](https://themes.gohugo.io/mainroad/) theme as a git submodule. However, there were some changes that I needed to make which worked better if I just copied the theme and included it as a subdirectory in my theme folder. This added it to my repository so that all of my changes would be included. Below is a list of a few of the changes:

1. Google Analytics v4 -- the hugo default was not working properly. So, I added my own partial that included the [Google Analytics](https://analytics.google.com) tag. I modified the Mainroad theme to include the partial. There is likely a more Hugo way of doing it that could override default behavior.

2. [TinyLetter](https://tinyletter.com/) Newsletter form -- I wanted to include a newsletter to make it easier for people to keep up with my progress. TinyLetter provides email capture for free and it also handles unsubscribes. This is awesome. I created a widget and then included it in the right nav.

3. I modified the template so that just the logo and subtitle would be in the header. The default Mainroad theme would only show the subtitle if the main title was also available. Additionally, the logo was too small whenever the title and subtitle were enabled. So, I modified the template to show just the logo and the subtitle without a requirement for a main text-based title.

### Day 3: Wednesday, March 31, 2021

**Today's Progress:** Started Apple SwiftUI Tutorial

**Thoughts:** Today, I started Apple's [SwiftUI Tutorial](https://developer.apple.com/tutorials/swiftui) just so that I could get acclimated to the process of developing interfaces with the framework. In the summer of 2019, while traveling with my daugther to volleyball camps, I did [The Complete 2021 Flutter Development Bootcamp with Dart](https://www.udemy.com/course/flutter-bootcamp-with-dart/) that was created by Dr. Angela Yu from the [The App Brewery](https://www.appbrewery.co). I enjoyed the declarative style to user interface development. So, when SwiftUI was announced, I immediately noticed the similarities and I knew that my Flutter experience would translate quite well to SwiftUI. This has proven to be the case.

I chose to focus my attention on SwiftUI because I wanted to become more familiar with the iOS ecosystem; specifically, the emergent SwiftUI. If I make it far enough, I will likely build an Android version using Android Studio and Kotlin to become more familiar with that ecosystem. Eventually, I may spend some time in either React Native or Flutter to make my cross-platform journey easier. For now, SwiftUI and the iOS ecosystem is where I am starting. Somewhere along this journey, I will share tips and tricks to help you pick up these technologies.

I am very excited about this experience and hope to keep it going. That being said, I will likely have to switch to early mornings as my family is not used to me being unavailable and are having a slightly tough time adjusting. It definitely feels nice to be missed even if I am only 20 feet away :)

### Day 4: Thursday, April 1, 2021

**Today's Progress:** Continued Apple's SwiftUI Tutorial

**Thoughts:** Today, I am almost done with Chapter 1 of the Apple SwiftUI Tutorial. Next, is section 6 called [Set Up Navigation Between List and Detail](https://developer.apple.com/tutorials/swiftui/building-lists-and-navigation). The tutorial is pretty straightforward and is a good enough introduction to SwiftUI. You should have some experience with the Swift programming language and should be familiar with the Xcode environment. Fortunately, I spent the last few months going through the [iOS & Swift - The Complete iOS App Development Bootcamp](https://www.udemy.com/course/ios-13-app-development-bootcamp/) by Dr. Angela Yu. Through project-based learning, Dr. Yu introduces you to the Xcode environment and some of the practices of iOS development. Because of going through these courses, picking up SwiftUI has been a process of learning SwiftUI fairly straightforward. 

There are 4 Chapters to Apple's SwiftUI tutorial:

1. SwiftUI Essentials
2. Drawing and Animation
3. App Design and Layout
4. Framework Integration

Below is a sample from the tutorial. Even if you do not know SwiftUI, I am pretty sure you can figure out what the below code does:

{{< figure src="/img/SwiftUI_sample.png" title="SwiftUI Sample" height="600" width="600" >}}

Progress is good so far. Should be in a good place to start the app building once I have completed this tutorial. I will be sharing some code examples once I actually start building my app.

### Day 5 and 6: Friday, April 2, 2021 and Saturday, April 3rd

**Today's Progress:** Continued Apple's SwiftUI Tutorial. But only had 30 minutes

**Thoughts:** Using [NavigationView](https://developer.apple.com/documentation/swiftui/navigationview) and [NavigationLink](https://developer.apple.com/documentation/swiftui/navigationlink) to forward to another view is so much easier than the [func prepare(for: UIStoryboardSegue, sender: Any?)
](https://developer.apple.com/documentation/uikit/uiviewcontroller/1621490-prepare) and the [func performSegue(withIdentifier identifier: String, sender: Any?)](https://developer.apple.com/documentation/uikit/uiviewcontroller/1621413-performsegue) constructs. Definitely see how this will be useful for my Scrabble clone.

### Days 7, 8 and 9: Sunday, April 4th through Tuesday, April 6th

**The Progress:** Continuing to research but haven't coded much more

**Thoughts:** Sunday was Easter/Resurrection Day. So, not much coding on that they. I could have but just decided that spending time with family was more important.

On the other days (Monday and Tuesday) -- As an Engineering VP, I spend quite a bit of time helping other people be successful at delivering software and so my time and brain power gets used up. Couple that with the family responsibilities and I have little time to code. That being said, I have found some cool things about SwiftUI. Some examples include:

* Shapes
    1. [Rectangle](https://developer.apple.com/documentation/swiftui/rectangle)
    2. [Rounded Rectangle](https://developer.apple.com/documentation/swiftui/roundedrectangle)
    3. [Ellipse](https://developer.apple.com/documentation/swiftui/ellipse)
    4. [Circle](https://developer.apple.com/documentation/swiftui/circle)
    5. [Capsule](https://developer.apple.com/documentation/swiftui/capsule)
* Grids
    1. [LazyHGrid](https://developer.apple.com/documentation/swiftui/lazyhgrid)
    2. [LazyVGrid](https://developer.apple.com/documentation/swiftui/lazyvgrid)
    3. [GridItem](https://developer.apple.com/documentation/swiftui/griditem)