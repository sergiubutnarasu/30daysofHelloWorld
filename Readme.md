### `#30xHelloworlds` `#codevember`
# 30 days of hello, world's
30 new things in 30 days to inspire a lasting curiosity & desire to experiment.

I believe the best way to improve, become well rounded, form better opinions, and enhance one's ability to choose the right tool for the occasion is through experience. 30 days of "Hello, world!" challenges one's self to dive into unfamiliar territory with an open mind and zero bias.

In 30 days, I'm challenging myself to experiment with different frameworks, language, libraries, patterns, API's and technology that are unfamiliar or new to me. The goal is simply to gain a better understanding of the tools of the web and tech landscape by getting hands on experience and having fun doing so.

Contents:
- [Day 1: Go lang](#day1)
- [Day 2: Hapi.js](#day2)
- [Day 3: Koa.js](#day3)
- [Day 4: Hug API framework](#day4)
- [Day 5: Django: scratching the surface](#day5)
- [Day 6: Architect: Dependency injection](#day6)
- [Day 7: Vue.js](#day7)
- [Day 8: TypeScript](#day8)

___

# <a name="day1"></a> Day 1: ready, set, GO lang.
To get `go`-ing, I chose to start with Go because I figured, if things go well, I could use it throughout the next 30 days as a platform on hosts like Heroku or Google App Engine.

## What I like after 1 day
The syntax seemed quickly familiar with the added difference/bonus of Type Declarations. However, the type interpolation is pretty nice in Go.

Importing dependencies is straight forward and clean.

## Learning curves:
Getting setup with the `$GOPATH` with ZSH for me took a bit of Googling and diving into Stack Overflow. After adding it to my `.zshrc` everything was fine.

The `struct` way of handling objects, and the lack of traditional classes, is a bit of a mind bend and takes time to understand, after only one day of Go, I haven't quite grasped it, yet.


Resources:
- [golang.org](https://golang.org/)
- [play.golang.org](play.golang.org)
- [Pluralsight Go fundamentals](https://app.pluralsight.com/library/courses/go-fundamentals)
- [Pluralsight Gin Go](https://app.pluralsight.com/library/courses/gin-go-web-app-framework/table-of-contents)


# <a name="day2"></a>Day 2: Hapi.js
In the spirit of setting up a web server with Go, I'm continuing the exploration around web servers with Hapi.js. Up until now, when I've needed to spin up a web server, I've almost exclusively reached for Express. Coming from Express, Getting started with Hapi was quite simple.

The setup and syntax are similar enough, and even without any familiarity with a web server platform, Hapi is quite straight forward and easy to use. I enjoy the speed and simplicity of Hapi and will likely use it in the future projects.

## Learning curves:
Some of the documentation and tutorials I was reading (unofficial) were for old versions of Hapi that had some plugins included in the "core" Hapi package, e.g., vision. Sorting that out was as quick as reading the official documentation. As with most things, reading the documentation is paramount to understanding exactly how each method should be configured; which in Hapi, can be exhaustive and will take some memorization.

Resources:
- [Hapijs.com official Tutorials](http://hapijs.com/tutorials)
- [Post example](https://github.com/paullang/hapi-post-example)
- [Pluralsight Building web applications w/ Hapi](https://app.pluralsight.com/library/courses/hapi-building-web-applications/table-of-contents)

# <a name="day3"></a>Day 3: Koa
Koa was designed by those who brought us Express and feels like Express 2.0, or how Express would have been built today. Koa is a light-weight, callback-less framework. Koa uses ES6 (ES2015) Generators for everything. There is no pre-bundled middle wear in Kia, which means everything is a plug-in—I’m noticing more and more people are adopting this bare-minimum platform pattern with plugins/modules/extensions, these days.

Koa vs. Hapi vs. Express? Numerous blogs do in-depth analysis on this topic ([Such as this one on AirPair](https://www.airpair.com/node.js/posts/nodejs-framework-comparison-express-koa-hapi)). In my opinion,  I don't think you can go wrong with any of the platforms; it depends on personal preference. Koa seems to be the "lightest" and being Generator based has advantages. Plus, Koa "Makes writing servers fast and enjoyable."

## Learning curves
Everything in Koa uses Generator functions, which, before this I hadn't  spent much time with in practical, real-world use. Koa is the first thing I’ve seen using Generators (and they utilized them way back before Node fully supported them) in a non-academic way. The whole architecture uses generators instead of callback functions to be light and clean; which Koa is. Once you understand how to work with Generators, and how to `yield`, building a project is straightforward and efficient. 

Resources:
[Koa homepage](http://koajs.com/)
[Pluralsight Intro to Koa Js](https://app.pluralsight.com/library/courses/javascript-koa-introduction/table-of-contents)
[Koa Examples](https://github.com/koajs/examples)


# <a name="day4"></a>Day 4 - Hug API framework

Hug + Python. It took some time to figure out what to design that was API only, but once I decided to build a simple random message app, things were easy. I didn’t get in too deep into all the features I would have liked to use in Hug, but I did see some parts that I would like to explore more of, mainly custom directives.

Hug makes writing API’s simple—as promised—once you know the syntax and how to use the decorators. The automatic documentation and error handling is very nice. I had planned to integrate swagger as part of day for documentation but found it wasn’t necessary (plus I was short on time)

## Learning curves
I struggled the most with creativity in trying to design an app “API first” Technically, the setup and installation process of Python 3.3, virtualenv, and hug took time and patience.

Resources:
Hug is not an easy framework to Google. Resources were a bit scarce compared to the larger frameworks I’m used to.
- [Hug.rest quickstart](http://www.hug.rest/website/quickstart)
- [Hug.rest Learn](http://www.hug.rest/website/learn/)
- [Hug examples code, Github](https://github.com/timothycrosley/hug/tree/develop/examples)

# <a name="day5"></a>Day 5 Django: The non-templating parts
Over the last year, I’ve used Jinja2 almost daily but never got around to checking out Django. Since I’m already familiar with the tempting _style_, the goal for today was to see all the other features Django has to offer.

The Django environment—at least from my minimal experience–is a fully considered development environment with all kinds of conveniences built in for developers; like a web server and simplified interactions and queries with databases.

Django aims to make developers more productive, and I think it does that well. I would say its similar to having a well-considered development environment built on Gulp, Grunt or similar tooling stack. The difference being that it has everything you need to get started writing your app without the overhead of installing and setting up your own tooling.

## Learning curves
Not a big deal, but in Django, the term “app” doesn’t refer to the entire application, but is more similar to “module.” The nature of the Django MVT(Model View Template, a variation of MVC–Model View Controller) architecture is to have a lot of files spread out, which is a bit cumbersome in the beginning. Fully comprehending which file needs which dependency takes practice and time.

Django has many proprietary commands that are required to work with Django, such as `python manage.py sqlmigrate` which are challenging to memorize right away. A cheatsheet or more time is needed (as is with most everything) to become fluent.

Resources
- [Official Django docs](https://docs.djangoproject.com/en/1.10/intro/overview/)
- [Pluralsight Django fundamentals](https://app.pluralsight.com/library/courses/django-fundamentals/table-of-contents)

#<a name="day6"></a> Day 6: Node Architect [Dependency injection]
I’ve been looking forward to trying Architect for Node for the last month. What I’ve read sounded promising, a lightweight, node-style framework for dependency injection. In other words, a simple framework for using plug-ins within an app. This type of application architecture would be perfect for allowing third-party plug-ins to be installed to different instances of an application—think Wordpress or Slack for example. Architect does make it easy to setup dependencies and create API's from one plug-in to another; called "consumes" and "provides" within the application. 

Project support for Architect is a bit lacking. While it’s still a viable framework, is not maintained in the official repository, but instead in the Coud9 core; as explained in this issue https://github.com/c9/architect/issues/48. Because of minimal support documentation is lacking. As easy and quick as Architect can be, without proper documentation, it’s hard to recommend it to someone who is looking for a speedy resolution. It takes time digging through the source code and an understanding of Node.js to figure out how to make it work. 

Given an abundance of free time, I would love to write documentation for Architect and solve some of the issues around getting started. I have to wonder if it would be a worthwhile project to write my own Architect inspired, modern, dependency injection/inversion of control type framework to solve my “plug-in store” application problem.

## Learning curves.
As mentions, Documentation is pretty scarce and limited to two examples in the official GitHub repo and a handful of blogs around the internet. There should be more support and better documentation! 

Resources:
- [c9/architect on Github](https://github.com/c9/architect)
- [Architecture Using Architect](https://medium.com/@ohbytheway/architecture-using-architect-8c8bb7d0277a#.lfbmvvax1)
- [Dependency injection in node js](https://mario.fyi/dependency-injection-in-node-js-and-other-architectural-patterns/)
- [Dependency injection in JS using architect](http://zedapp.org/2014/04/dependency-injection-in-javascript-using-architect/)

#<a name="day7"></a> Day 7: Vue.js!
Before jumping in to check out Vue.js, I had heard a lot of good things about the framework. After watching Evan You ([@youyuxi](https://twitter.com/youyuxi))’s talk on Vue.js, it seems that it is in line with my current thinking around how frameworks should work. In a nutshell, that is being less prescriptive, but extensible. The idea of a “progressive framework” sounds good–and in Vue.js’s case, works well. I haven’t formed a solid opinion on whether or not I like the idea of keeping all of the HTML, CSS, and JS of a component smushed in one file (in the past I’ve been against it), but so far in Vue, it works OK.

For my dip into Vue, I spent more time playing with the well-documented examples on the official site, watching the talk, and reading through the documentation and source code of Vue. I didn’t get too much hands on time with this, but it is something I look forward to re-visiting in the future. 

## Learning curves
As with every framework, there is a prescribed way to do things. Setting up a new Vue project is pretty painless. The biggest hurdle is probably learning what Vue can do, how it handles it and learning to write the code to execute it. 

Resources:
- [Vue.js Official guide](https://vuejs.org/v2/guide/)
- [Vue.js Talk by Evan You](https://www.youtube.com/watch?v=pBBSp_iIiVM&feature=youtu.be)

#<a name="day8"></a> Day 8: Typescript
Typescript is/can be used with Angular 2, so I wanted to spend some time working with TypeScript separate from A2.

TypeScript is essentially syntactic sugar for writing clean Javascript. An example is `namespace` and `export` which simply compile down to an immediately invoked function to keep namespaced items block scoped. This is the big take away, since TypeScript compiles to regular Javascript, the rules in TS are not held true at run time but are at compile time. TypeScript is largely (almost 100%) a developer tool for writing more descriptive code. It makes sense to reach for Typescript to keep code organized and "strict".

As a bonus, TypeScript development in VSCode is very nice.

## Learning curves
Most of what typescript offers is very straightforward. There are only a few new things to learn as far as syntax and definition go, to get started. A couple things still have me a bit confused (after only a couple of hours) and that is type declaration for Arrays and Generics–since I don’t come from a static typed language like C+ or Java.

Resources:
- [Lynda.com TypeScript essential training](https://www.lynda.com/Typescript-tutorials/TypeScript-Essential-Training/421807-2.html)
- [TypeScript in VSCode](https://code.visualstudio.com/Docs/languages/typescript)
- [TypeScript Playground](https://www.typescriptlang.org/play/index.html)
