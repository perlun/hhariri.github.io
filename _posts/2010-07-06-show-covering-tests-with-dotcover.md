---
layout: post
title: Show Covering Tests with dotCover
categories: []
tags:
- dotCover
status: publish
type: post
published: true
meta:
  _elasticsearch_indexed_on: '2010-07-06 21:50:00'
comments: true
---
<p>One of the new features <a href="http://www.jetbrains.com/dotcover">dotCover</a> has added is the ability to find tests that cover a certain piece of code. Something remotely similar has been available in <a href="http://www.jetbrains.com/resharper">ReSharper</a>, although it has been kind of an archaic solution (i.e. Find Usages on Method calls, locate Test assemblies in Result window).</p> <p>dotCover makes this easier by providing quick access to this information and extends it in functionality.</p> <p>Below we can see some tests from an MVC application. Let’s run Code Coverage on it using dotCover first.</p> <p><img style="border-bottom:0;border-left:0;display:inline;border-top:0;border-right:0;" title="a" border="0" alt="a" src="{{ site.images }}/covering-1.png" width="520" height="249"> </p> <p>Now let’s switch over to the Source Code and select some random source code, in this case the <strong>MembershipService.ChangePassword </strong>line in the <strong>ChangePassword </strong>action:</p> <p><img style="border-bottom:0;border-left:0;display:inline;border-top:0;border-right:0;" title="b" border="0" alt="b" src="{{ site.images }}/covering-2.png" width="550" height="249"> </p> <p>&nbsp;</p> <p>&nbsp;</p> <p>In order to see the tests that cover this line of code, we can either press the default key combination of Ctrl+Alt+K or select the option <strong>Show Covering Tests </strong>from the dotCover:</p> <p><img style="border-bottom:0;border-left:0;display:inline;border-top:0;border-right:0;" title="c" border="0" alt="c" src="{{ site.images }}/covering-3.png" width="248" height="156"></p> <p>dotCover will then display a small window showing all the different tests that cover that line of code.</p> <p><img style="border-bottom:0;border-left:0;display:inline;border-top:0;border-right:0;" title="d" border="0" alt="d" src="{{ site.images }}/covering-4.png" width="612" height="111"></p> <p>At this point, we can run the selected tests or add them to the existing ReSharper Test Runner session. This allows us to easily jump from specific sections of code to the corresponding tests and execute them instantly.</p> <p>One minor note: The default key mapping conflicts with KeePass, but you can easily re-assign it via Visual Studio Tools | Options | Keyboard, or do as I did and change KeePass to Ctrl+Alt+P (P as in Password…makes more sense).</p> <p><img style="border-bottom:0;border-left:0;display:inline;border-top:0;border-right:0;" title="e" border="0" alt="e" src="{{ site.images }}/covering-5.png" width="424" height="249"></p>
