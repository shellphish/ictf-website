# iCTF: the International Capture The Flag Competition

The International Capture The Flag ("iCTF") is a distributed, wide-area security exercise, which aims to test the security skills of the participants.
The iCTF is one of the world's largest and longest-running educational hacking competitions, and integrates both attack and defense aspects in a live setting.

The iCTF is usually held once a year, but the dates sometimes move around to accommodate the needs of the Shellphish team. 
You can find the schedule of the iCTF on [ctftime](https://ctftime.org/ctf/5).

iCTF 2021
---------

The iCTF 2021 took place on December 3, 2021 from 10am Pacific Time to 7pm Pacific Time.

***UPDATE: iCTF 2021 is officially over, thanks to everyone organizing and all of you playing, we hope you had a blast! Archived artifacts of the competition (scoreboard, competition website) can be found at the [iCTF 2021 Archive](archive/ictf_2021)!***

Overview
--------

The Shellphish iCTF contest is multi-site, multi-team hacking contest in which a number of teams compete independently against each other.

In traditional editions of the iCTF competition, the goal of each team is to maintain a set of services so that they remain available and uncompromised throughout the contest. 
Each team also has to attempt to compromise the other teams' services. 
Since all the teams have access to an identical copy of the virtual host containing the vulnerable services, each team has to find vulnerabilities in their copy of the hosts and possibly fix the vulnerabilities without disrupting the services. 
At the same time, the teams have to leverage their knowledge about the vulnerabilities they found to compromise the servers run by other teams.  
Compromising a service allows a team to bypass the service's security mechanisms and to "capture the flag" associated with the service.
These flags are then presented to the organizers as "proof of compromise" to receive "attack" points.
The teams also receive "defense" points if they can keep their services functional and uncompromised.

At the end of competition, the team with the most points wins.

The iCTF Framework
------------------

Shellphish has made available to the public the iCTF framework, which is the software infrastructure used to run the competition.

The framework is available for download on GitHub: [https://github.com/shellphish/ictf-framework](https://github.com/shellphish/ictf-framework)

The iCTF framework is free for both commercial and non-commercial use (donations are welcome!). 
The iCTF competition is based on the iCTF framework and similar competitions can leverage the framework to create other educational security competitions.


History and Background
----------------------

The iCTF evolved from a number of security "live exercises" that were carried out locally by Prof. [Giovanni Vigna](http://www.cs.ucsb.edu/~vigna/) at UC Santa Barbara, in 2001 and 2002. 

Motivated by the student's enthusiasm for security competitions, Prof. Vigna carried out the first wide-area edition of the iCTF in December 2003.
In that CTF, fourteen teams from around the United States competed in a contest to compromise other teams' network services while trying to protect their own services from attacks. 
This historical contest included teams from UC Santa Barbara, North Carolina State University, the Naval Postgraduate School in Monterey, the West Point Academy, Georgia Tech, University of Texas at Austin, and University of Illinois, Urbana-Champaign.

In 2004, the iCTF evolved into a truly *international* exercise (hence, the name "iCTF"), which included teams from the United States, Austria, Germany, Italy, and Norway.

For many years, the iCTF was the world's largest educational security competition, and helped popularizing this type of event.

Throughout the years, new competition designs have been introduced that innovated the more "traditional" designs followed in the early editions of the competition.

More precisely, in 2008 the iCTF featured a separate virtual network for each team. 
The goal was to attack a terrorist network and defuse a bomb after compromising a number of hosts. 
This competition allowed for the recording of several parallel multi-stage attacks against the same network. 
The resulting dataset has been used as the basis for correlation and attack prediction research.

In 2009, the participants had to compromise the browsers of a large group of simulated users, steal their money, and create a botnet. 
This design focused particularly on the concept of drive-by attacks, in which users are lured into visiting web sites that deliver attacks silently.

In 2010, the participants were part of a coalition that had to attack the rogue nation of Litya, ruled by the evil Lisvoy Bironulesk. 
A new design forced the team to attack the services supporting Litya's infrastructure only at specific times, when certain activities were in progress. 
In addition, an intrusion detection system would temporarily firewall out the teams whose attacks were detected.

In 2011, the participants had to "launder" their money through the execution of exploits, which had some risks associated with them. 
This created an interesting exercise in evaluating the risk/reward trade-offs in network security.

In both 2012 and 2013, teams had to "weaponize" their exploit and give them to the organizer, who would then schedule their execution. 
This last design was a first step towards the creation of a "cyber-range" where interesting network datasets (with ground truth) can be created to support security research.

In 2014, the competition was used as a way to publicize the iCTF Framework. 
To this end, the vulnerable virtual machine contained 42 services from previous iCTF editions, which forced the participants to effectively triage their efforts.

In 2015, the iCTF followed a novel design: in order to participate, the teams had to provide a vulnerable service that would become part of the competition.
As a result, the 2015 iCTF featured 35 new services (and 35 teams) and tested a new set of skills, in addition to attack and defense: the ability to create a well-balanced vulnerable service.

In 2016, the we decided to permanently move the competition to March (and since the decision was made in October, there was no iCTF event in that year).

In March 2017, the iCTF was run using Amazon Web Services (Amazon's cloud).
All components were run in an enclave, and the competition, for the first time, was open to the world, resulting in more than 280 teams participating.
Until then, only academic teams were allowed to participate.

In March 2019, the iCTF competition continued to be hosted on Amazon AWS infrastructure and introduced a new way of creating and deploying services using containers.
The competition was held on March 15th, 2019 with almost 400 teams participating.

In March 2020, the iCTF competition featured a novel component-based deployment mode, that allowed for greater scalability.

Archive
-------

An archive with resources for previous years can be found here:

* [Archive](archive/)

This is a port of an older archive so data is often missing for older entries.

Publications
------------

The organizers of the iCTF have published a number of papers about various aspects of designing and organizing security competitions:

* "How Shall We Play a Game: A Game-Theoretical Model for Cyber-warfare Games," by Tiffany Bao, Yan Shoshitaishvili, Ruoyu Wang, Christopher Kruegel, Giovanni Vigna, and David Brumley, in *Proceedings of the IEEE Computer Security Foundations Symposium (CSF)*, Santa Barbara, CA, August 2017.

* "Shell We Play A Game? CTF-as-a-service for Security Education," by Erik Trickel, Francesco Disperati, Eric Gustafson, Faezeh Kalantari, Mike Mabey, Naveen Tiwari, Yeganeh Safaei, Adam Doupe, and Giovanni Vigna, in *Proceedings of the USENIX Workshop on Advances in Security Education (ASE)*, Vancouver, BC, August 2017.

* "Ten Years of iCTF: The Good, The Bad, and The Ugly," by Giovanni Vigna, Kevin Borgolte, Jacopo Corbetta, Adam Doupe, Yanick Fratantonio, Luca Invernizzi, Dhilung Kirat, and Yan Shoshitaishvili, in *Proceedings of the USENIX Summit on Gaming, Games and Gamification in Security Education (3GSE)*, San Diego, CA, August 2014. 

* "Do You Feel Lucky? A Large-Scale Analysis of Risk-Rewards Trade-Offs in Cyber Security," by Yan Shoshitaishvili, Luca Invernizzi, Adam Doupe, and Giovanni Vigna, in *Proceedings of the ACM Symposium on Applied Computing (SAC)*, Gyeongju, Korea, March 2014.

* "Formulating Cyber-Security as Convex Optimization Problems," by Kyriakos Vamvoudakis, Joao Hespanha, Richard Kemmerer, Giovanni Vigna in *Control of Cyber-Physical Systems*, Lecture Notes in Control and Information Sciences, July 2013.

* "Influence of team communication and coordination on the performance of teams at the iCTF competition," by S. Jariwala, M. Champion, P. Rajivan, and N. Cooke, in *Proceedings of the Annual Conference of the Human Factors and Ergonomics Society*, Santa Monica, CA, 2012.

* "Hit 'em Where it Hurts: A Live Security Exercise on Cyber Situational Awareness," by Adam Doupe, Manuel Egele, Benjamin Caillat, Gianluca Stringhini, Gorkem Yakin, Ali Zand, Ludovico Cavedon, Giovanni Vigna, in *Proceedings of the Annual Computer Security Applications Conference (ACSAC)*, Orlando, FL, December 2011. 

* "Organizing Large Scale Hacking Competitions," by Nicholas Childers, Bryce Boe, Lorenzo Cavallaro, Ludovico Cavedon, Marco Cova, Manuel Egele, Giovanni Vigna, in *Proceedings of the Conference on Detection of Intrusions and Malware and Vulnerability Assessment (DIMVA)*, Bonn, Germany, July 2010.

* "Teaching Network Security Through Live Exercises," by Giovanni Vigna, in *Proceedings of the Third Annual World Conference on Information Security Education (WISE)*, Monterey, CA, June 2003.

* "Teaching Hands-On Network Security: Testbeds and Live Exercises," by Giovanni Vigna, in *Journal of Information Warfare*, vol. 3, no. 2, February 2003.  

Point Of Contact
----------------

The International Capture The Flag (iCTF) is organized by [Shellphish](https://shellphish.net).

For information contact [ictf@shellphish.net](mailto:ictf@shellphish.net).

