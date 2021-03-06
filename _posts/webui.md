---
title: "The web as a GUI toolkit"
date: 2020-02-13
tags: ['Web']
updated: 2020-04-02
hatnote: |
    Discussions:
      [Lobsters](https://lobste.rs/s/vrb7qh/web_as_gui_toolkit),
      [Hacker News](https://news.ycombinator.com/item?id=22319489).
---

The web is kinda weird because it was originally created as a typesetting
system, rather than a GUI toolkit. While this definitely has its drawbacks[^1]
and isn't suitable for *everything*, I personally rather like the "web as a GUI
toolkit" exactly *because* of its typesetting roots; it provides some features
that few other GUI environments give us.

[^1]: Are there problems too? Yeah, of course. But everyone else is already
      complaining about them, so I'll omit them here 😅

Some things that work really well that are often hard in native GUI toolkits:

- You can zoom pretty much any content as large or small as you like. Doing this
  in native UI involves either editing obscure config files, or mucking about
  with the system's DPI settings (not easy to zoom per-app or changing zoom
  levels depending on mood or screen you're using).

- More cross-platform than pretty much anything else.

- Open anything in a new context (tab or window).

- Copy/paste anything.

- Search any text with e.g. Ctrl+F.

- Back button.

- Modifying anything easily; even if you're not doing this directly yourself
  this has huge benefits in the form of e.g. [some simple
  bookmarklets](/bookmarklets.html) or your adblocker.

- Unlike desktop applications, everything is sandboxed. If you think persistent
  tracking and fingerprinting on the web is bad: it's even easier on the
  desktop. Something like hash(/etc/passwd) should do the trick to generate a
  persistent unique device ID.

- Very compatible; the [first website][first] last modified somewhere in the
  early 90s still works in your Firefox or Chrome today.

These are all things that aren't available in your standard GTK/Qt/Cocoa/MFC
applications unless you specifically program them, which most apps don't. The
web gives them by default.

[first]: http://info.cern.ch/hypertext/WWW/TheProject.html

---

But the most important reason I like it requires some background: I started
programming on the MSX, a machine roughly similar to the Commodore 64 or BBC
Micro: you turn it on and you're dropped to [BASIC][b] environment.

[b]: https://en.wikipedia.org/wiki/BASIC

After we got a Windows machine things were a lot harder; remember, this is
around 1999[^2] and I was 14-year old non-native English speaker. Things like
Pascal and Python and whatnot were all around, but I didn't know about them.
Programming your computer on your own was kinda hard and non-obvious, at least
for me. This was a very different experience from the MSX, which you can program
immediately after booting by using the manual you got with the computer.

[^2]: I'm really too young to have grown up on BASIC; our MSX2 was from 1985,
      my birthyear. I remember programming on it when some of my friends already
      had a Pentium III.

I tried mucking about with some pirated copy of Visual Studio I got somewhere (I
thought this was the only way you could program) and after some failed attempts
with C++ I gave up. It probably didn't help that *Teach yourself C++ in 10
minutes* isn't a very good programming book, at least not for beginners.

So, I stopped programming for a few years and it wasn't until I installed Linux
(which got replaced by FreeBSD fairly quickly) around 2004 that I really got
back in programming. Just like the MSX, my FreeBSD machine was programmable out
of the box, which made it much easier to get started. Soon I was mucking
about with shell scripts, Python, Perl, and C – all tools available by default.

With the web there's a happy medium: you're not dropped to a BASIC or Unix
shell, but programming your browser is as easy as opening the web inspector, and
while JavaScript isn't perfect, it's fairly easy to get started with.

With the web almost everyone has a machine that has a programmable environment
by default again. I feel this is a very important and powerful advantage that's
often overlooked. I appreciate that a lot of people have zero interest in
programming their machines – just like many don't have any interest in modifying
their cars – but many *do* have this interest, and I think there's value in
empowering that.
