++
draft = true
++

# How to Join an existing open source project

Lets assume you’re convinced that contributing to open source is something you want to do.  When I started, I had this assumption pretty drilled into me, but it’s hard to get started! And scary!  Let me just assure you: If you find it hard to know where to start, its not you; its hard for everyone! That said, working on Open Source Software is super rewarding!✨

This point aims to demystify the process by way of a story.  At Stride, we have an Open Source Club. At the club, we don’t just work on open source (although that’s part of it); we also work on the process of open source (how do you run a project, how can you be an effective member of a project).  A number of the members of the club are relatively new to OSS an were curious how they’d join a project, so we, as a group contributed to ESlint. This is the story of that contribution, framed as examples of general guidelines that could be applied to any project.

### Vetting 🤔
Assuming that you have a few projects in mind that you might want to contribute to, how do you evaluate whether its worth your time to break into the project. What are the signs of a good, healthy, worth-your-time project?
Here’s a general list of things to look for
- **Attention to the contributors time:** this shows up in Labelled issues (ESlint has issue labelled as `beginner` and `documentation`) a contribution. A working build step (this could be a makefile, steps documented in a readme or contributing.md
- **Tests:** This is not only just a good thing in terms of engineering practice, but tests act as documentation and guiderails when you’re adding things or changing the code
- **Active Community:** How fast do issues and questions get addressed?  ESlint has lots of issues, but questions get answered super fast.  They have a gitter (a slack-like chatroom) where I got questions answered really quickly; they even picked out some `beginner` issues for us to work on.
- **Welcoming Community:** This matters.  ESLint has a gitter chat room, and people on their were super friendly when we asked about beginner issues, even labelling a few for us to work on. Labelled issues like `beginner` or `first-time` or by familiarity level make it easy to pick something to start on.  A **Code of Conduct** is also a part of welcoming community, as it makes the standards of behavior clear and open.
- **Governance Model:** Is it OSS in name only (ie a product created in the open, but with only commercial concerns). This isn't inherently bad, but it'll likely effect how the project runs.

Some anti-patterns to consider:
  - Popularity:  Super popular projects can be frustrating to get started in as issues get snapped up really fastx
  - Rude people in issues
  - Tumbleweeds (super old issues, commits, etc) Not always bad, because you might be able to take ownership over an important project, but maybe not when you're starting out
  - Only core members in commits
  - Open in name only (basically its controlled by one company or its their product)
  - Super complicated build, or you can't build it all
  - No documentation or test
  
  ### What how? 🔍
Landing that first PR is an awesome experience, and if you can pick something that ultimately kinda simple, you'll also get to overcome the hurdles of learning the actual contribution process and not get too bogged down in the details of fixing code in an unfamiliar codebase; next time, you can focuse on something in the code, and the process itself won't be a blocker. Docs are often a good first step, because they force you to learn a little bit about the code, but working on them is mostly about writing and then getting through the contribution process.  On ESlint, we found an bug report, that turned out to be a result of some unclarity in the documentation. The actual change was rather minor, adding a few words and a sentence. Eslint provids a great `Contributing` section of their docs, which gives an overview to the process, so we had some idea what to expect.  That said we had to do a few things that are unfamiliar to new OSS folks.

Out contribution followed these steps:
1. **Fork**  I've done this a lot, and I still had to [look on Github](https://help.github.com/articles/fork-a-repo/) almost every time for about the first year.
2. **Write** docs or code that follow the style and conventions of the project.
3. **Commit** in the style of the project.  Some projects have commit templates that you need to follow
3. Make a **PR** in the style of the project. ESlint provides nice markdown templates and very clear instructions for PRs of various sorts (Docs, bug fixes, etc.) which all follow differant formats.
4. Sign a Contributors License Agreement(**CLA**). This basically certifies your right to contribute code. Many projects don't have this.
3. **More changes** to make the bots happy! 🤖 ESlint and other projects use bots to automatically enforce conventions in code, commits, and PRS. Usually these are a first gate to get through to getting a merge.
4. **Discussion** with the project maintainers and changes. This is often a decent back and forth, with tweaks and comments. Overwhelmingly on healthy projects this is a fun and productive exchange that drastically improves the quality of your contributions.
5. Das **Merge!** 🎉

Don't get too worried if you find yourself in the weeds.  That's a pretty long and potentially intimidating list! As I said earlier, this can be a challenging and confusing process - its not you! - so keep you chin up.  It'll be awesome!

In addition to docs, as I mentioned before, few other nice ways to help projects when you're just starting out: filing and fixing bugs you encounter yourself (you have the context so that can help); [Gardening](http://words.steveklabnik.com/how-to-be-an-open-source-gardener) which is a term coined by Steve Klabnik in an OSS context - basicaly it means going through issues, open PRs, etc. and commenting or doing what you can to try and get things in a better order; adding test coverage.

## In summary 🐙

Getting started in open source can be confusing, but its ultimately super rewarding. Picking a project and issues carefully can make the difference between frustration and fun. Hopefully the story of our contribution to ESlint and the general guidelines I provide give your some tools to make stepping into OSS less intimidating. If you have any questions about what I've written, please reach out. I'm on twitter @zandermackie or reachable by email zmackie@stridenyc.com.  Thanks for reading!
