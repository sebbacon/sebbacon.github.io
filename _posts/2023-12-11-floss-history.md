---
layout: post
title:  "FLOSS history: code as art"
date: 2023-12-11
categories: coding, history
---

Way back in 2006, I co-authored a paper with [Teresa Dillon](http://www.polarproduce.org/) on “The potential of open source approaches for education”. It was published by Nesta's FutureLab and appears to be unvailable online.

I was inspired to try to hunt it down. I couldn't find the whole thing, but I did find a final draft of the section on the history of the open source movement.

It's interesting to re-read it nearly 20 years later. Lurking behind all the facts, I can clearly make out some of my core beliefs about software engineering, and how I relate to it personally:

> Code, therefore, shares some superficial similarities with human language.  
>
> As a result it is considered by many working in this field as a form of expression: software that accomplishes exactly the same result (say, sorting a pack of cards) may theoretically be written in an infinite number of ways, depending on the particular intuitive or artistic preferences of the programmer.  
>
> It is not by chance, therefore, that many of the legal debates around software are couched in terms of artistic copyright or free speech, and it is in this conception of software, as expression rather than as a form of machine, that the origins of FLOSS software lie. 

In 2006, there was still debate about the term "FLOSS" versus "Open Source"; there was much talk of patent law fights, of Microsoft coopting and attacking the movement. 

In 2023, no-one uses the term "FLOSS" any more; I doubt younger programmers are aware of the deep ideological roots of the rise of Open Source; Microsoft are, in some limited respects, leaders in the Open Source field. 

The "pragmatist / libertarian" angle espoused by Eric Raymond now completely dominates the stories Open Source software engineers tell themselves about their work, and (I believe) this is only partly due to Stallman's [appalling comments](https://en.wikipedia.org/wiki/Richard_Stallman#Controversies) around the Epstein scandal and the Free Software Foundation's astonishingly poor judgement in reappointing him to their board.   

Accordingly, on re-reading my words from the past, I realise that stories I tell myself have also shifted: I no longer pay attention to the ideology (aside from a tendency to favour copyleft licenses). But it's helped me notice that I still think of software as poetry, as a creative act, a tool for making interventions in the real world that can be exciting, beautiful, and strange.

Anyway, for posterity, here's the historical overview I wrote back in 2006....

<!--more-->


**Historical Overview**

The following history provides readers new to the field with an outline map of some of the diverse and overlapping narratives which inter-relate in the history of the FLOSS movement.

It is a history which interweaves legal issues and licences with programming practices and technological developments and new forms of collaboration and communication.  All of these factors need to be considered in understanding the implications of FLOSS for educational practice.

In the early 1960s, before software development was a major industry, most code was created in an academic-style environment, albeit one often embedded in a commercial context. It was circulated around communities of experts, discussed, peer-reviewed, and built upon.  Computers were vast physical objects the size of rooms and the cost of running programs was expensive.

Consequently, all software was developed in well-funded organisations, often in technologically advanced academic institutions in collaboration with the military, security forces and large commercial enterprises. As the number of software producers and consumers was too small to allow for a commercial software ecology, source code was not considered a valuable commodity. As it had marginal economic value, it was natural to consider source code a public good.

Many of the enthusiasts who understood how to program were more interested in solving problems than making money.  In this environment, new software moved around quickly on magnetic tape, on punch cards or on paper printouts.



**UNIX and the birth of the internet**

In 1969, as part of their work with Bell Labs (a division of AT&T telephone company), software engineers Thompson and Richie developed a new Operating System, called UNIX (see Salus, 1994).  Since so few computers existed (all room-sized mainframes) UNIX wasn’t conceived as having potential commercial benefit.  In addition, anti-trust legislation forbade AT&T from entering the computer business[^1], so UNIX maintained its academic-style culture of free circulation and peer-review (McGowan, 2005).

The University of California at Berkeley started licensing UNIX from AT&T in 1975 and researchers developed the code further.  Recent changes to the software were packaged and released under the name Berkeley System Distribution (BSD) to anyone who requested it.  UNIX began to develop very fast until so much of the source code had been rewritten and extended that it was hard to see the BSD as the same as UNIX. 

In 1984 AT&T entered the computer business (McGowan, 2005) with UNIX. Initially, BSD was more successful, partly because it contained more desirable features, but the BSD project continued to share their work with the UNIX originators and this flow of innovation allowed UNIX to dominate a growing commercial marketplace.  Berkeley focused on academic research and exploring the next generation of technological developments. 

Under a contract with DARPA (United States Defence Advanced Research Projects Agency) the team at Berkeley added networking code to BSD so that it ran with other types of network.  This part of BSD, known as TCP/IP,[^2] became the building block of the Internet and allowed BSD (and consequently UNIX) users across the world to communicate using a single networking system. As the TCP/IP parts of BSD had been developed entirely without AT&T UNIX code, the BSD team decided to release those portions independently, under a very unrestrictive licence that stipulated that anyone could use and copy the code as long as they credited BSD.

This was the first instance of an Open Source License and is crucial to the later development of the FLOSS movement and to the further spread of the internet: much of the world’s internet software is derived from the original BSD TCP/IP and networking code, including some of the networking software inside Microsoft Windows.

Attention turned to the question of whether it might be possible to remove _all_ AT&T code from BSD to create a standalone release completely free of restrictive licences.  It was widely regarded as a nearly impossible feat, but in fact was made possible by an innovation enabled by BSD in the first place: the internet. 

Keith Bostic[^3], one of the creators of the BSD system, saw the potential of mass development of software using the internet whereby people who had never met each other could work together on a single project. The enthusiast culture that had grown up alongside BSD, combined with the unique collaborative potential of the internet, allowed the removal of nearly all of the AT&T code from BSD within two years (McKusick 1999).

The success of BSD, combined with how easily it could be copied and incorporated into commercial code, led to a dispute between the University of California at Berkeley with AT&T through its spin-off company USL (UNIX System Laboratories). The case was settled, with a crucial stipulation: USL would not sue anyone using the settled version of BSD as the basis for their own system.

Today, there are four major variants of BSD derived from the original BSD code    that are widely used including Darwin (the basis of Apple Mac systems) and NetBSD (an open-source project for building a BSD-based Operating System that is both free and available for many platforms).  These BSD licences are examples of ‘permissive’ licences that impose almost no conditions on what a user does with the software. This means that redistributors can use it for proprietary products, so derived works do not need to be open source.


**The Birth of GNU and copyleft**

The freedom offered by the licensing arrangements to use and modify BSD code were not considered ‘free’ enough by some. 

The hacker culture encompasses its own jargon, symbols and expressions, many of which explicitly oppose or subvert the ‘mainstream’ (defined in terms of ‘normal’ values and working habits) expressed in the proprietary software model to which the FLOSS paradigm is opposed.[^4] The most relevant aspect of the culture to the emergence of FLOSS is the ‘hacker ethic’: the idea that information sharing is a powerful and positive good, and that hackers have an ethical duty to increase the public information commons.  The ethic is often summed up in the humorous phrase ‘information wants to be free’  (Stallman, 1992). 

The most significant development that emerged from MIT’s hacker culture was Richard Stallman's GNU Project, in many ways a direct reaction to the increasing commoditisation of software.  Prior to this, hackers and others with programming knowledge were able to fix computing breakdowns because they had the ability to ‘get into the engine’ on the machine.  However, the explosion of the software market led to the closure of source code, which became a trade secret.  Users of software like Microsoft’s MS-DOS were no longer able to fix errors themselves.

Stallman's dictum that source code should be freely available began to take on a totemic quality and he decided to attempt to develop a complete UNIX-like operating system, to be called GNU.[^5]  In 1985, Stallman published the "GNU Manifesto", which aimed to "knit the diffuse post-1980 community of hackers into a coherent social machine for achieving a single revolutionary purpose".[^6] He labelled his philosophy "Free Software" and formed the "Free Software Foundation[^7]" (FSF) as a vehicle for implementing his manifesto.  In particular, Stallman developed the "Four Freedoms of free software”.[^8] These are:



* The freedom to use software however you wish (a freedom most programs give you)
* The freedom to change software to suit your needs.
* The freedom to distribute the software to anyone else, and in doing so the freedom to "help your neighbour". 
* The freedom to distribute altered version of the software, and in doing so cultivate a community based around the evolution of that software

In order to preserve these freedoms permanently, Stallman came up with a novel and inverted way of using the legal system of copyright – by developing what is known as copyleft (DiBona et al., 1999). 

To understand what Stallman achieved, it is necessary to first understand what we mean by copyright. Copyright is a form of intellectual property that allows the licence holder the sole legal right to copy their works of original expression, for a defined period of time. It is designed to protect the creator’s right to control copies and changes to a work, and by default, copyright is usually used by the originator of a work to _restrict_ how it is used. Stallman ingeniously used the restrictive capabilities of copyright in a novel way: he used it to restrict peoples' rights to distribute the GNU software _unless _they agreed to distribute it under exactly the same terms as they received it.  In short, where copyright protects the creator of the work, copyleft protects the right of users to copy and change a work in perpetuity.  In sum, by creating a licence that protects the commons from private appropriation, the concept of copyleft gave power back to the user and made various other forms of FLOSS licences and its derivatives such as the Creative Commons[^9] possible (Lessig, 2004).



**The growth of FLOSS**

In 1981 IBM’s personal home computer was launched and it became clear that software could also be viewed as a commodity.  Companies, such as Microsoft, started to appear that specialised in particular variants of software. The exceptional skills of the hackers at the MIT AI Lab became more valuable and, as public funding of the Lab tailed off, members of the Lab began to work in other commercial and non-commercial contexts. Many set up their own ‘spin-off’ companies, drawing on the fruits of their earlier research. Eventually the main research project at the lab, “the Lisp Machine”, [^10] was taken completely into the proprietary domain, and the source code was no longer distributed as a public good (Williams, 2002).

The internet provided a networked, global resource through which software could be shared. With the release of Stallman’s GNU code and GPL licence over the net, other programmers began to build and extend it. One key addition was made in 1991 by a young Finnish Computer Science graduate, Linus Torvalds.

Torvalds wanted to adapt the GNU system to run as a fully functional operating system on his home PC.  The part that was missing was the ‘kernel’, which he developed under the name “Linux.” Three key factors converged to make his vision possible: he was able to use the GPL to ensure that his work would remain fully free; he was able to use the internet to distribute his code; and affordable home computers meant that development was in reach of people without access to expensive mainframe computers.

With Linux[^11], the phenomenon of Free Software took on a new characteristic.  The movement had always been about collaboration, but typically this collaboration took the form of swapping ideas between individuals or small teams.  The combination of circumstances that led to the fast spread and development of Linux was mainly characterised by the sheer size of the developer community.

In 1999, Eric Raymond, self-styled “tribal historian and resident ethnographer” of hacker culture, published The Cathedral and the Bazaar, an essay examining the importance of the “scale” phenomenon on the successful development of Linux  (Raymond, 1999). Raymond was astonished to find, associated with Linux, a complete and usable system – he had been an enthusiastic user of free software for some years without ever seeing the movement create complete systems (the GNU Operating System had been a decade in the making).

His analysis was that the “old” model of software development, typified in projects like GNU, was top-down: run by a small number of key hackers, who acted as the gatekeepers to the source code.  Contributors submitted their software changes to the gate keepers, who then made a decision on whether or not to incorporate those changes into the central source code.  Raymond (1999) compares this to the construction of medieval cathedrals.

By contrast, Linux had developed in a similar way to the nascent free market represented by the medieval bazaar, where order arose spontaneously where enough people met to exchange and socialise.  In this account, Linux evolved in an organic, even chaotic manner.  Developers exchanged and contributed source code without any direction from above.  Software releases were frequent, and new features were tested by large numbers of people as soon as they had been sketched out.  A process of natural selection eventually allowed the good ideas to thrive. 

For Raymond, this insight is the key to the phenomenal success of Linux.  By spreading the ideas and software as far as possible, an emergent, evolutionary process ensured the progression and quality of the software.  Raymond coined the phrase “many eyes make bugs shallow” to express one advantage of the distributed FLOSS approach: when the source code is available to all, the software becomes more robust and secure.  This phenomenon is counterintuitive to many from outside the FLOSS community: surely a piece of encryption software, for example, is far more secure if its internal details are effectively locked away?  However, there is a wide consensus that exactly the opposite is true when it comes to cryptographic software, and many in the FLOSS world believe this same principle applies to all software.



**Free versus Open Source**

Raymond’s account of the software culture that emerged from the early UNIX and MIT camps, is informed by an anarcho-capitalist, market-oriented worldview.  This is in strong contrast to Stallman’s** **adherence to his understanding of the principle of freedom.  Indeed, Stallman’s ‘viral’ Free Software definition of FLOSS has been argued in America to be restrictive, anticompetitive, and even un-American, and has been subject to sustained challenge by Microsoft (Raymond, 2001).  Stallman, however, strongly refutes the charge of economic leftism, claiming that the four freedoms of the GNU manifesto encourage true competition rather than closed monopolies (Stallman, 2002).  Nevertheless, there is a strong suspicion across all FLOSS subcultures that commercial interests tend to co-opt the socially-oriented goals of the developers – a suspicion which is strongest amongst the GNU/FSF advocates.

Raymond formulated a plan to move the free software movement towards a more business-friendly arena and took the position that in order to maintain and extend the success of the free software approach, it was necessary to package it in a format palatable to business and the media. The phrase “free software” was felt to be ambiguous: it confuses free (unhindered) with free (gratis).  The phrase “Open Source” was picked to represent the movement, and a foundation was set up to certify licences as Open Source.  Both BSD-style licences and GPL-style copyleft licences are “Open Source” in that they permit the programmer to read and modify the source code of a piece of software to which they apply.  The ideas expressed in the Cathedral and the Bazaar helped the software industry understand how free software could actually help them in achieving high quality, secure software.

The first high-profile Open Source convert was Netscape Communications, who had effectively lost the “browser wars” of the 1990s to Microsoft’s Internet Explorer software.  They decided their best strategy for preventing Microsoft from using its position to dominate the web was to release the entire Source Code for the Netscape Communicator web suite to the community.  It took far longer than anyone imagined, but the seed they planted is now growing in the form of the Firefox[^12] web browser.  Other companies are also exploring the open source route: IBM[^13] is now an open-source consulting firm and Intel are moving towards releasing their latest chip specifications under an open-source-inspired licence.


**Internal controversy - coining the FLOSS term**

The two major camps of free software (on one side the FSF/GNU community voiced by Stallman, and on the other Raymond’s OSI and the BSD communities) often engage in vigorous, sometimes acrimonious debate. In particular, Stallman argues that non-copyleft licences inherently undermine the principle of freedom in allowing third parties to co-opt and close the source code, where the BSD and OSI sides claim that the restrictions of copyleft are themselves not commensurate with the goal of freedom. Others (Berry, 2004; Collman & Hill, 2004) have argued that the philosophy is politically agnostic, and analyse the competing interpretations as “iconic practices” which lend themselves to multiple meanings that belie the political inclinations of those who espouse them. 

_Table 1: Difference between Free and Open source software_


<table>
  <tr>
   <td>
   </td>
   <td>Free Software culture
   </td>
   <td>Open Source Software culture
   </td>
  </tr>
  <tr>
   <td>Organisation
   </td>
   <td>Free Software Foundation
   </td>
   <td>Open Source Initiative
   </td>
  </tr>
  <tr>
   <td>Figurehead
   </td>
   <td>Richard Stallman
   </td>
   <td>Eric Raymond
   </td>
  </tr>
  <tr>
   <td>Favoured license type
   </td>
   <td>Gnu Public License: “viral”, ensuring openness of code in perpetuity
   </td>
   <td>BSD-style licenses: not placing any restrictions on use of software
   </td>
  </tr>
  <tr>
   <td>Perceived benefits of FLOSS
   </td>
   <td>Freedom of information
   </td>
   <td>Better quality software
   </td>
  </tr>
  <tr>
   <td>Values outside software
   </td>
   <td>Leftist; communitarian; idealist
   </td>
   <td>Libertarian; laissez-faire; pragmatist
   </td>
  </tr>
</table>


At the present time, while acknowledging the difference between free and open source software, many people have chosen to use the encompassing term FLOSS. This is a compromise term but it encapsulates all possible meanings that have evolved from the free software movement: Free, Libre Open Source Software.



**Widening influence of FLOSS approaches**

The development of a strong hacker subculture in parallel with the emergence of the proprietary software model from an initially heavily regulated sector was a major factor in the evolution of FLOSS from a quasi-academic way of developing Operating Systems to a movement with global influence. Linux, for example, is the fastest-growing sector in the server market (Gould, Barnett, Kimberly, Dowling, & Hogan, 2005) and has become a longstanding, major player in this area; and the arrival of software such as OpenOffice, and the web browser Firefox, has meant that the world of FLOSS has begun to penetrate the edges of the public consciousness and to challenge for the consumer software market (Fisher, 2004).

The FLOSS movement is beginning to have implications outside the world of software. Despite the sometimes profound disagreements within the community, one issue has become a totem for the entire movement: that of Patent law. As hackers see software as a form of expression, the application of patent law to software is seen as absurd, just as it would be ridiculous to patent the music of Beethoven.  The anti-software patent position is widely held across all FLOSS subcultures (for example Lessig, 2004).

Many in the movement, spearheaded by Stallman, have taken the argument about patents further, to encompass all “Intellectual Property” issues  (Stallman, 2002).  The hacker ethic has started to spread beyond software.  Further inspired by technological developments that have made the circulation of mass media artefacts (such as films and music) as simple as pressing a button, proponents claim that technology has rendered the old IP system redundant, and that the music and film industries are going to have to adapt or die out. 

Even further from software, FLOSS licences like the GPL have inspired a slew of licences that can be applied to forms of expression other than software – in particular, the “Creative Commons” project, aimed at “building a layer of reasonable copyright”.  Perhaps the most significant recent developments along these lines are the “open content” encyclopaedia, Wikipedia, edited by any visitor who cares to do so, and which aims to constantly improve following the Bazaar principle described by Raymond; and the BBC iCan website, which aims to create a platform for cooperation between people to get information about and address ‘issues that concern them’ (eg starting local campaigns). iCan is an example of an open model that allows individuals to pursue hobbies of interest or in order to develop social capital (Davis, 2004).




<!-- Footnotes themselves at the bottom. -->
## Notes

[^1]:
     Regulatory Keynesian models of economy were the norm, and strict regulations were designed to hold back large corporations from the monopolistic excesses of the utility industries of the 1920s and 1930s.

[^2]:
     TCP/IP (Transmission Control Protocol/Internet Protocol) refers to the suite of [communications protocols](http://www.webopedia.com/TERM/T/communications_protocol.htm) (ie the set of rules which defines how devices communicate to each other) used to connect [hosts](http://www.webopedia.com/TERM/T/host.htm) on the [Internet](http://www.webopedia.com/TERM/T/Internet.htm). TCP/IP uses several [protocols](http://www.webopedia.com/TERM/T/protocol.htm), the two main ones being [TCP](http://www.webopedia.com/TERM/T/TCP.htm) and [IP](http://www.webopedia.com/TERM/T/IP.htm). [TCP/IP](http://www.webopedia.com/TERM/T/TCP_IP.html) is built into the [UNIX](http://www.webopedia.com/TERM/T/UNIX.htm) [operating system](http://www.webopedia.com/TERM/T/operating_system.htm) and is used by [the Internet](http://www.webopedia.com/TERM/T/TCP_IP.html), making it the [de facto standard](http://www.webopedia.com/TERM/T/de_facto_standard.htm) for transmitting [data](http://www.webopedia.com/TERM/T/data.htm) over [networks](http://www.webopedia.com/TERM/T/network.htm). Even [network operating systems](http://www.webopedia.com/TERM/T/network_operating_system_NOS.htm) that have their own protocols, such as [Netware](http://www.webopedia.com/TERM/T/NetWare.htm), also [support](http://www.webopedia.com/TERM/T/support.htm) TCP/IP (definition taken from [http://www.webopedia.com/TERM/T/TCP_IP.html](http://www.webopedia.com/TERM/T/TCP_IP.html), Retrieved date 31<sup>st</sup> May 2005)

[^3]:
     One of the senior technical members of the Computer Systems Research Group at the University of California, Berkeley, who joined in 1986 and is now the founder member of Sleepycat [http://www.sleepycat.com/](http://www.sleepycat.com/). (retrieved 11<sup>th</sup> November 2005)

[^4]:
     The hacker culture which has become central to the Open Source philosophy grew out of early mainframe users at MIT who had an ethos of sharing and co-development (Levy, 1984). Within MIT hacking had a variety of connotations and was used to describe someone who pulled clever pranks and got away with it; someone who explored undocumented or unauthorised areas in buildings; as well as someone who created elegant solutions to a computing problem.

[^5]:
     Refer to the GNU Operating System site: [http://www.gnu.org/](http://www.gnu.org/). Retrieved on 31<sup>st</sup> May 2005.

[^6]:
     See [http://www.gnu.org/gnu/manifesto.html](http://www.gnu.org/gnu/manifesto.html)

[^7]:
     Free Software Foundation: [http://www.fsf.org/](http://www.fsf.org/). Retrieved on 31<sup>st</sup> May 2005.

[^8]:
     Taken from [http://www.gnu.org/gnu/thegnuproject.html](http://www.gnu.org/gnu/thegnuproject.html). Retrieved on 8th August 2005.

[^9]:
     http://creativecommons.org/

[^10]:
     LISP is a functional programming language, developed at MIT by John McCarty, 1958 and is used today in a variety of programs and considered one of the most elegant and flexible computing languages. For history of LISP refer to [http://en.wikipedia.org/wiki/LISP#History](http://en.wikipedia.org/wiki/LISP%23History)

[^11]:
     http://www.linux.org/

[^12]:
     Mozilla, Firefox: [http://www.mozilla.org/products/firefox/](http://www.mozilla.org/products/firefox/)

[^13]:
     Intel, Open Source Products: [http://www.intel.com/software/products/opensource/](http://www.intel.com/software/products/opensource/)
