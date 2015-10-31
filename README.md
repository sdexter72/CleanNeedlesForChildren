# Purpose

The purpose of this repository is to provide high level instructions for a class
leader to set up a modern cpp IDE on stuudent computers that is both free and 
runs on Windows.

# What's with the name?

Windows is terrible. Proprietary software is worse.  This project
should be viewed through the lens of 'harm reduction programs.' The 
best thing by far is to implore students to get off windows like 
they were getting off of Heroin.

However most Computer Science students (girls as well as boys) come to
us after a decade of gaming. Can I play Halo if I switch to Ubuntu? Is there
a version of Grand Theft Auto or Call of Duty for Debian?  Explaining the 
virtues of Free Software has not worked for me.  I even showed students
Richard Stallman's excellent (and brief) TedX talk available at the url below:

<https://www.youtube.com/watch?v=Ag1AKIl_2GM>

The reactions I received were simmilar to exposing them to a Bernie
Sander's rally. "That is a cool old dude. Am I going to change my life? No."

# What's wrong with other alternatives?

## The professional solution

Visual Studio costs $800.  Although one can use the AStyle plugin to
write styled code. On our lab computers this was never installed, let
alone configured.

## What students use

To save money, many students use Bloodshed's Dev-C++.  This has not been
maintained for 10 years and there are more than 340 known unfixed bugs. See
the url below for more detail.

<http://clicktobegin.net/programming/why-you-shouldnt-use-dev-c/>

# Clean Needles

If students will not leave proprietary software alone. I still want
them to learn posix style command line driven development. Here is my
zero cost and Free Solution.  These are not self study directions for
students. This requires using elisp to load packages and configure
packages and python to run cpplint.  This is directed at the grad
student adjunct or instructor teaching them.

# Emacs

The hacker's editor.  You can use if for 30 years. It is not really and editor.
It is a REPL.  The best way for windows users to get it is via:

<http://vgoulet.act.ulaval.ca/en/emacs/windows/>

If you are a VIM afficianado, you can use Evil mode.

# Google C++ Style Guide

This has been operationalized in a python package (library) called
cpplint that is freely available.  Now Google's style guide is
somewhat controversial in the C++ community.  See
<https://news.ycombinator.com/item?id=7900238> for a critique of the
guide ane the video <https://www.youtube.com/watch?v=NOCElcMcFik> for
its philosophy.  What is not in doubt is that successful projects
adhere to a style.  If you check out only one of these references
watch, Greg Hartman-Kroah's "I Don't Want Your Code",
<https://www.youtube.com/watch?v=fMeH7wqOwXA>.

# Semantic Auto-Complete

We install auto-complete with semantic parsing for a back end. We also make 
auto-complete aware of our compiler include files.

# Benefit

Students learn to be comortable on the command line and can add
familiarity with many open source tools incrementally such as gdb and
valgrind.

# Installation