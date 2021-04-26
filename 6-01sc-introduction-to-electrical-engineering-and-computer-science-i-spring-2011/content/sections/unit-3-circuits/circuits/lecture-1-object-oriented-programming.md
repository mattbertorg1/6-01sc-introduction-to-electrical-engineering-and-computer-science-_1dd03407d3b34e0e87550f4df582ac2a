---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: 5sLFTc10kg8
  parent_uid: 9fe057844e7944c539f15aa427f7e263
  title: Video-YouTube-Stream
  type: Video
  uid: 5a9a52215d9d3c499b1a14625dc3a048
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/lecture-7-circuits/id490181666?i=109416118
  parent_uid: 9fe057844e7944c539f15aa427f7e263
  title: Video-iTunes U-MP4
  type: Video
  uid: 1a4e9fea3dbb6617586861570aa5a563
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_S11_lec07_300k.mp4
  parent_uid: 9fe057844e7944c539f15aa427f7e263
  title: Video-Internet Archive-MP4
  type: Video
  uid: 6aeb57a8182eb9d9417b16dc2facf272
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/5sLFTc10kg8/default.jpg
  parent_uid: 9fe057844e7944c539f15aa427f7e263
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 4e365678867deedebdb3f75e98c886d6
- id: MIT6_01SC_S11_lec07_300k.srt
  parent_uid: 9fe057844e7944c539f15aa427f7e263
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuits/lecture-1-object-oriented-programming/MIT6_01SC_S11_lec07_300k.srt
  title: MIT6_01SC_S11_lec07_300k.srt
  type: null
  uid: 7fb2c13cd37aab019846d2667ced5edd
- id: Caption-OCW-SRT
  parent_uid: 9fe057844e7944c539f15aa427f7e263
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: f5a85c57a58122742be2ea34f4c1c435
- id: MIT6_01SC_S11_lec07_300k.pdf
  parent_uid: 9fe057844e7944c539f15aa427f7e263
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuits/lecture-1-object-oriented-programming/MIT6_01SC_S11_lec07_300k.pdf
  title: 'MIT 6.01SC S11 Lecture 7: Circuits Transcript'
  type: null
  uid: 033e66a16c383b3d09015848094e4fe9
- id: Transcript-OCW-PDF
  parent_uid: 9fe057844e7944c539f15aa427f7e263
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: 0158e7060f058561eca7dad295b568b6
inline_embed_id: 96590364lecture7:circuits48262529
layout: video
order_index: null
parent_uid: c1a11356f20d61ecdbf385a0ade29169
related_resources_text: ''
short_url: lecture-1-object-oriented-programming
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuits/lecture-1-object-oriented-programming
template_type: popup
title: 'Lecture 7: Circuits'
transcript: '<p>The following content is provided under a Creative Commons license.
  Your support will help MIT OpenCourseWare continue to offer high-quality educational
  resources for free. To make a donation or view additional materials from hundreds
  of MIT courses, visit MIT OpenCourseWare at ocw.mit.edu.</p><p>PROFESSOR: So today
  I want to start a new topic, circuits. No, that''s good. That''s good. Circuits
  are good.</p><p>AUDIENCE: Yay.</p><p>PROFESSOR: Thank you, thank you. Much better.
  So just to provide some perspective, I want to remind you where we are, how we got
  here, and where we''re going. So at the beginning of the course, we promised that
  there were several intellectual themes that we would talk about. Probably the most
  important one there is designing complex systems. That''s what we''re really about.
  We would like you to be able to make very complicated systems. How do you think
  about parts? How do you think about connecting them? How do you think about things
  when you want to make something that''s very complicated?</p><p>Part of that is
  modeling. We just finished a module on modeling. So in order to make a complex system,
  we''d like to be able to predict how it will behave before we completely build it.
  Sometimes it''s impossible to build the entire system before. Sometimes it''s impossible
  to build prototypes. Sometimes you''re stuck with going with the design at launch,
  and figuring out how it works. In those cases in specific, it''s very important
  to be able to model it, to have some confidence that the thing''s going to work.</p><p>We''re
  going to talk about augmenting physical systems with computation. That''s the module
  we''re about to begin. And we''ll conclude by talking about how to build systems
  that are robust to change. So we started with the idea of, how do you make complicated
  systems? And we introduced this notion of primitives, combination, abstraction,
  and pattern in terms of software engineering. We did that because that''s the simplest
  possible way of getting started. It provided a very good illustration of PCAP at
  the low level by thinking about Python, by thinking about the primitive structures
  that Python gives you, how those can be combined, how you can abstract, how you
  can recognize patterns. But then we also built a higher level abstraction, which
  was the state machine idea.</p><p>There the idea was you didn''t have to have state
  machines in order to build the brain for a robot, but it actually turns out to be
  easy if you do because there''s a modularity there. You can figure out if each part
  works independent of the other parts. And then you can be pretty sure when you put
  it together the whole thing''s going to work. So that was kind of our introduction
  to this notion of PCAP.</p><p>Then we went on to think about signals and systems.
  And that was kind of our introduction to modeling. How do you make a model of something
  that predicts behavior? So we transitioned from thinking about, how do you structure
  a design to how do you think about behavior.</p><p>Today we''re going to start to
  think about circuits. Circuits are really going to a more primitive physical layer.
  How do you think about actually making a device? So the device that we''ll think
  about is a thing to augment the capabilities -- the sensor capabilities of the robot.
  We''ll think about making a light tracking system. And the idea is going to be that
  you''ll build a head. The head has a neck, so you''ll have to control the neck.
  The head has eyes. It will mount on top of the robot, and that''ll let you drive
  the robot around looking for light. And you''ll do that by designing a circuit.
  So that''s kind of the game plan for the next three weeks.</p><p>So today, what
  I want to do is introduce the notion of circuits, introduce the theory for how we
  think about circuits. And then in the two labs this week, the idea will be to become
  familiar with the practice of circuits. How do you actually build something? How
  do you actually make something work?</p><p>So today''s the theory. So the theory,
  the idea in circuits is to think about a physical system as the interconnection
  of parts and rules that connect them. In fact, the rules fall into two categories.
  We''re going to think about the currents that go through parts and the voltage that
  develops across parts. And we''ll see that there''s a way of thinking about the
  behavior of the entire circuit that integrates all of those three pieces. How does
  the part work? How do the currents that go through the part work? And how do the
  voltages that are produced across the part -- how do they work?</p><p>So I''ll just
  start with two very simple examples. The first is the most trivial example you can
  think about. You can think about a flashlight as a circuit. You close the switch,
  current flows. Very simple idea. We will make a model of that that looks like this.
  We''ll think about the battery being a source. In this case, a voltage source. We''ll
  think about the light bulb being a resistor. We''ll have two parts. We''ll have
  to know the current-voltage relationships for both of the parts. And we''ll have
  to know the ramifications for those currents and voltages when you put them together.
  Very, very simple.</p><p>The other simple example that I want to illustrate is this
  idea of a leaky tank. Here the idea that I want to get across is that the circuit
  idea is quite general. When we talk about circuits, we almost always talk about
  electronic circuits. But the theory is by no means limited to electronics.</p><p>So
  for example, if we think about a leaky tank, we think about a pipe spewing water
  into a reservoir. Maybe that''s the Cambridge Reservoir. Maybe that''s the water
  coming out of the Woburn Reservoir. Maybe that''s the demand put on by the Cambridge
  people trying to take showers in the morning -- I don''t know. So we think about
  flow into a tank, a reservoir, and flow out. And we can make a model for that in
  terms of a circuit.</p><p>In the circuit there are through variables and across
  variables. In an electronic circuit, the through variable is current. Here the through
  variable is the flow rate. So it''s the flow of water in and the flow of water out,
  represented here by these things that look like currents. And the across variable
  for an electronic device is voltage. The across variable for this kind of a fluidic
  device, the across variable is pressure. So we think as this thing gets ahead of
  that thing, as there''s more stuff coming in than going out, the height goes up
  and the pressure builds.</p><p>Same idea. So the point is that we''ll develop the
  theory for circuits in terms of electronics. But you should keep in the back of
  your mind that it''s a lot more general idea than just electronics. In fact, there
  are two completely distinct reasons why we even bother with circuits.</p><p>One
  is that they''re very important to physical systems. If you''re designing a power
  network, of course you have to think about the way the power network, the power
  grid works as a circuit. That''s obvious. In electronics, of course, if you''re
  going to build a cell phone, you have to know how the parts interconnect electronically.
  That''s obvious.</p><p>But probably the biggest use for circuits these days is not
  those applications, although those are very important. Circuits are also used as
  models of things. So many models for complex behaviors are in fact circuit models.
  So in terms of electronics, the idea is that we want to get on top of electronics.
  We want to understand how circuits work, so we can understand things like that.</p><p>If
  you look at how complex processors have got over my professional life, we start
  with my professional life down at about 1,000 transistors per processor. And today,
  we''re up at about a billion. That''s enormous. Even in the stone ages when we were
  designing things that had a thousand parts, we still had trouble thinking about
  those thousands parts all at once. We still need PCAP. We still needed ways of combining
  the activities of many things into a conceptual unit that was bigger. Here, it''s
  just impossible if you don''t have that. So that''s one of the reasons we study
  circuits.</p><p>And the other reason is here. So here I''m showing a model for the
  way a nerve cell works. This model is taken from 6.021. The idea, this comes from
  the study of the Hodgkin-Huxley model for neural conduction, arguably the most successful
  mathematical theory in biophysics. Which explains the completely non-trivial relationship
  between how the parts from biology works and the behavior in terms of propagated
  action potentials works. So the idea is that we understand how this biological system
  works because we think about it in terms of a circuit. That''s the only successful
  way we have to think about that.</p><p>So what I want to do then is spend today
  figuring out circuits At the very most primitive level. The level that I''m going
  to talk about in terms of circuits is roughly analogous to the level that we talked
  about with Python when we were thinking about how Python provides utilities for
  primitives, combinations, abstractions, and patterns.</p><p>So I''m going to start
  at the very lowest level and think about, what are the basic primitives, the smallest
  units we''ll ever think about in terms of circuits? And what are the rules by which
  we combine them? So I''ll start with the very simplest ideas, the very simplest
  elements. We will oversimplify things and think about the very simplest kind of
  electronic elements as resistors that obey Ohm''s Law, V equals iR. Voltage sources,
  things that maintain a constant voltage regardless of what you do. And current sources,
  things that maintain a constant current regardless of what you do. These things
  are, as I said, analogous to the primitive things that we looked at in Python. They''re
  also analogous to the primitive things that we looked at in system functions.</p><p>Can
  somebody think of, when we were doing difference equations, what were the primitives
  that we started with -- when we started to study difference equations? What''s the
  most primitive elements that we thought about?</p><p>AUDIENCE: Delay.</p><p>PROFESSOR:
  Delay, yeah. So we thought about things like-- so we had delay. Anything else?</p><p>AUDIENCE:
  Gain.</p><p>PROFESSOR: Gain. Anything else? Add. So we had exactly three primitives.
  And we got pretty far with those three primitives. We learned the rules for interconnection.
  We didn''t really make a big deal out of it. We didn''t formalize it, but the rules
  for interconnection were something like every node has to have exactly one generator.
  You can''t connect the output of this to this, that''s illegal. Every node has to
  have one source. And every node can source lots of inputs. That was kind of the
  rules of the interconnect. The interconnects here will be a little bit more complicated.
  So those are the elements that we''ll think about.</p><p>And the first step''s going
  to be to think about, how do they interconnect? The simplest possible interconnections
  are trivial. In the case of the battery, you hook up the voltage source to the resistor.
  The voltage source makes the voltage across this resistor 1 Volt. If we say the
  resistor is 1 Ohm, then there''s 1 Amp current period. Done. Easy.</p><p>Similarly,
  if we were to hook up the resistor to a current source, we would get something equally
  easy. Except now the current source would guarantee that the current through the
  resistor is an amp. Therefore, the voltage across the resistor, by Ohm''s law, would
  be a Volt. So we would end up with the same solution for a completely different
  reason.</p><p>Here the voltage is constrained. Here the current''s constrained.
  Just to make sure everybody''s with me, figure out, what''s the current i that goes
  through this resistor? Slightly more complicated system. Take 20 seconds, talk to
  your neighbor, figure out a number between (1) and (5).</p><p>OK, so what''s the
  answer? Everybody raise your hand with a number (1) through (5). Come on, everybody
  vote. Come on. You can blame it on your neighbor, that''s the rules. You talk to
  your neighbor, then you can blame dumb answers on your neighbor.</p><p>OK, about
  80% correct I''d say. So how do you think about this? What''s going to be the current?
  How would you calculate the current? What do I do first? Shout. If you shout, and
  especially if my head''s turned away I don''t know who you are.</p><p>AUDIENCE:
  Kirchhoff''s law.</p><p>PROFESSOR: Kirchoff''s law, wonderful. Which one? There''s
  two of them.</p><p>AUDIENCE: [UNINTELLIGIBLE].</p><p>PROFESSOR: [UNINTELLIGIBLE].
  What loop do you want to use?</p><p>AUDIENCE: Left.</p><p>PROFESSOR: Left side.
  So if we use the left side loop, we would conclude that there''s a volt across the
  resistor. So the current would be?</p><p>AUDIENCE: 1 Amp.</p><p>PROFESSOR: An amp.
  Where''s the current come from?</p><p>AUDIENCE: The voltage.</p><p>PROFESSOR: The
  voltage source just like before. So not quite. So the voltage source establishes
  this voltage would be 1. That makes this current be 1. That would be consistent
  with the current coming out of here, except we have to also think about that 1 Amp
  source. So the question is, what''s does the 1 Amp source do? Nothing? It''s just
  there sort of for decoration or for [UNINTELLIGIBLE] so that we can make an interesting
  question to ask in lecture? Maybe.</p><p>So where''s the current? Where''s the 1
  Amp that goes through the resistor come from?</p><p>AUDIENCE: [UNINTELLIGIBLE] on
  the right.</p><p>PROFESSOR: It comes from the right. It comes from the current over
  here. So the idea is that if this current, ignore the voltage over here for the
  moment. If this current flowed through the resistor, then you''d have 1 Amp going
  through there, and you''d have 1 Volt generated by that current which just happens
  to be exactly the right voltage to match the voltage from the voltage source.</p><p>So
  if you think about this, the voltage guarantees that this is 1 Volt, but so does
  the current. In order to simultaneously satisfy everything, all you need to do is
  have all of this current go around and come down through that resistor. That will
  generate the volt, so there''s no propensity for more current to flow out of the
  source because the source is 1 Volt and it''s facing a circuit that''s already 1
  Volt. So the idea was to try to give you something that''s relatively simple that
  you can think through on your own, but not trivial. So the answer was 1 Amp. But
  the 1 Amp was not for the trivial reason. The 1 Amp is because the current from
  the right flows through the resistor and makes the voltage be 1. So the right answer
  is 1. But for the reason that you might not have originally thought.</p><p>But more
  importantly, I wanted to use that as a motivation for thinking about, how do we
  think about bigger circuits? So when the simple circuit, like two parts, it''s no
  problem figuring out what the answer''s going to be. But when the circuit has even
  three parts, it may require more thinking. And you may want to have a more structured
  way of thinking about the solution. Yes?</p><p>AUDIENCE: What would have occurred
  if the current provider on the right side was 2 Amps?</p><p>PROFESSOR: Great question.
  Had this been 2 Amps, you can''t violate this voltage. So that would have been 1
  Volt. So that would have been 1 Amp through the resistor. So then you''re left with
  the problem with this guy''s pushing 2 and that guy''s only eating 1. But the rules
  for the voltage source say eat or source however much current is necessary in order
  to make the voltage equal to 1. So the excess amp goes through the voltage source.
  So the voltage source is, in fact, being supplied power rather than supplying power
  itself.</p><p>Had this been 2 Amps, some of the power from this source would have
  gone into the resistor. And some of the power from this source would have actually
  gone into the voltage source. So if the voltage source were, for example, a model
  for a rechargeable battery, that rechargeable battery would be charging. Does that
  make sense? So if there had been a mismatch in the conditions, you still have to
  satisfy all the relationships from all of the sources.</p><p>AUDIENCE: What if the
  voltage was larger?</p><p>PROFESSOR: The same thing would have happened. Except
  now the flowing current would be in the opposite direction. Let''s say that if the
  voltage here had been 2 Volts, then the voltage would have required that there is
  2 Amps flowing here. 1 Amp would come from here, but another Amp would come from
  here. This voltage source will supply whatever current is necessary to make its
  voltage law real. Ok.  In fact, what we''ll do now is turn toward a discussion of
  more complicated systems that will let you go back and in retrospect, analyze all
  those cases that we just did. And you''ll be able to see trivially how that has
  to be the right answer.</p><p>So what I want to do now is generate a formal structure
  for how you would solve circuits. Yes?</p><p>AUDIENCE: So did we know of anything
  that could generate a current without generating a voltage, like in real life?</p><p>PROFESSOR:
  Can anything generate a current without generating a voltage? That''s a tricky question.
  If you think about something as generating a current, then the voltage is not necessarily
  determined by that part. So that''s kind of illustrated here. If this guy is generating
  a current, this guy is not actually the element that is controlling its own voltage.</p><p>In
  general, if you want to speak simultaneously about the current and voltage across
  the device, you have to know what it was connected to. Each part-- we''ll get to
  this in a moment in case some of you are worried about launching ahead. We will
  cover this. This is very good motivation for figuring out what''s going to happen
  in the next three slides.</p><p>So each part gets to tell you one relationship between
  voltage and current. Generally speaking, that''s not enough to solve for voltage
  and current. Voltage and current is like two unknowns. Each element relationship
  is one equation. So the current source gets to say current equals x, current equals
  1 Amp. It doesn''t get to tell you what the voltage is.</p><p>So being a little
  more physical to try to address your question more physically, there are processes
  that can be extremely well modeled as current generators. In fact, many electronic
  semiconductor parts, like transistors, work more like a current source than like
  anything else. So there are devices that behave as though they were current sources,
  but they don''t simultaneously get to tell you what is their current and what is
  their voltage. They only get to tell you what is their current.</p><p>So let''s
  think about now, if you had a more complicated system, how could you systematically
  go about finding the solution? As was mentioned earlier, there''s something called
  Kirchhoff''s law. And in fact, there''s two of them. Kirchhoff''s voltage law and
  Kirchhoff''s current law. Kirchhoff''s voltage law, in its most elementary form,
  says that if you trace the path around any closed path in a circuit, regardless
  of what the path is-- every closed path-- the sum of the voltages going around that
  closed path is 0.</p><p>So for example in this circuit, the red path illustrates
  one closed path through the circuit. It goes up through the voltage source, down
  through this resistor, and then down through that resistor. Kirchhoff''s voltage
  law says the sum of the voltages around that loop is 0. That''s written mathematically
  here, minus v1 for here, plus v2 for here, plus v4 for here is 0.</p><p>OK, where
  do the signs come from? The signs came from the reference directions that we assigned
  arbitrarily to the elements. Before I ever do a circuits question, I always assign
  a reference direction. Every voltage has a positive terminal and a negative terminal.
  And I must be consistent in order to apply these rules. These rules only work if
  I declare a reference direction and stick with it.</p><p>If midway through a problem
  I flip it, I''ll get the wrong answer. So the minus sign has to do with the fact
  that as I trace this path, I enter the minus part of this guy, but the plus part
  of that guy and that guy. So the sign of v1 is negated relative to the others.</p><p>A
  different way to think about that is here, we can think that v1 is the sum of v2
  and v4. That''s sometimes more intuitive because if you started here, going through
  this path you would end up with a voltage that is v1 higher than where you started.
  Whereas starting here, you would end up with a voltage here that''s v4 higher than
  where you started. And then by the time you got to here, it would be v2 plus v4
  higher than where you started.</p><p>You start one place and on one route, you end
  up v1 higher. And in the other route, you get v4 plus v2 higher. So it must be the
  case that v1 is the same as v2 plus v4. Those are absolutely equivalent ways of
  thinking about it. So those laws are equivalent. If you think about it  a path,
  you think about some of the paths-- no. The path coinciding with the negative direction
  of some of the elements and the positive direction of others.</p><p>OK, how many
  other paths are there? Take 20 seconds, talk to your neighbor. Figure out all of
  the possible paths for which KVL has to apply.</p><p>OK, so everybody raise your
  hand and show a number of fingers equal to the number of KVL equations less two.
  Oh, very good. Virtually 100% correct. Why do you all say (5)? Which is to say 7.
  Why do you all say 7?</p><p>So there''s 3 obvious ones. I was expecting a couple
  of 3''s. This was supposed to be-- OK, yeah, I do plot against you. I was expecting
  some 3''s. So there''s 3 obvious paths that are analogous to the first one we looked
  at. If I call the first path A, then there''s B and C which are the excursions around
  here. And you can write the equations just the same. They each involve three voltages.
  And they each go through, some starting at the negative side and some starting at
  the positive side. So those are in some sense, the obvious ones. But there are others
  too.</p><p>So one way to think about it, what I''d like you to do is enumerate all
  the paths through the circuit. I should have said all the paths through the circuit
  that go through each element one or fewer times. I don''t want you to go through
  the same element twice.</p><p>So here''s another path that would go through elements
  at most one time. So up through here, over through here, which didn''t go through
  any elements. Down through that element, across that, down through here, et cetera.
  And you get an equation for that. Here''s another. Here''s another. Here''s another.</p><p>And
  if you try to think about a general rule, a general rule is something like, how
  many of those panels can you make and piece together where the loop goes through
  the perimeter? You''re not allowed to go through an inner place because if you went
  through an inner node, you''d have to go through it twice. If you wanted the path
  to go through an inner element, you''d have to go through that element twice.</p><p>So
  in fact, the answer is 7. There are 7 different paths according to Kirchhoff''s
  voltage law, all of which the sum of the voltages around those paths has to be 0.</p><p>The
  problem is, of course, that those equations are not all linearly independent. So
  if you just had a general purpose equation solver-- and by the way, we''ll write
  one of those in week 8 for solving circuits. If you just passed those 7 equations
  into a general purpose equation solver, it would tell you there''s something awry
  with your equations because they''re not linearly independent.</p><p>So you can,
  however, think about linearly independent in particularly simple cases. This network
  is a particular kind of network that we call a planar network. A planar network
  is one that I can draw on a sheet of paper without crossing wires.</p><p>So I can
  draw this network without crossing wires. I''ll call it planar. And it turns out
  that Kirchhoff''s voltage laws for the innermost loops are always independent of
  each other. That''s kind of obvious because as you go to a -- so each loop contains
  at least one element that some other loop didn''t have. So that''s kind of the reasoning
  for why it works.</p><p>So if you think about this particular loop, which we included
  in the 7, you can think about that as being the sum of the loops this way, the A
  loop and the B loop. Because if you write KVL for the A loop and KVL for the B loop
  and add them, you end up deriving KVL for the more complicated path.</p><p>And if
  you think about what''s going on, it''s not anything terribly magical. This path
  is the same as the A path added to that path, where I went through this element
  down when I did the A path and up when I did the B path. So those parts canceled
  out. That was the rule that I was talking about how I don''t really want to go through
  the same element twice when I''m applying KVL.</p><p>So the idea then is that there''s
  a systematic way, an easy way to figure out all the KVL loops. You just think about
  all the possible paths through the circuit. You do have to worry about linearly
  independent. In the case of planar networks, that''s pretty straightforward. Planar
  networks, you can always figure out the linearly independent KVL equations by looking
  at the smallest possible loops. The loops with small area.</p><p>OK, so that''s
  half of it. That''s KVL. The other Kirchhoff''s law is KCL, Kirchhoff''s Current
  Law. There we are thinking of the flow of current. So the flow of current is analogous
  to the flow of incompressible fluid. Water, for example.</p><p>If you trace the
  amount of water that flows through a pipe that goes into a Y, then the sum of the
  flows out has to equal the flow in. If that weren''t true, the water would be building
  up.</p><p>So we think about pipes as transporting the flow of water without allowing
  it to build up anywhere. That''s precisely how we think about wires in electrical
  circuits. The wires allow the transport of electrons but don''t allow the buildup
  of electrons.</p><p>OK, do electrons build up? Sure. But in our idealized world,
  we say they don''t build up in the wires, they build up in a part. And we''ll have
  a special part that allows the electrons to build up. So we''re not excluding the
  possibility that they build up, we''re just saying that in this formalism, we don''t
  allow the electrons to build up in the wires. So for the purpose of the wires, current
  in is equal to the current out. The net current in is 0.</p><p>So we will think
  then, about the circuit having nodes. The nodes are the places where more than one
  element meets, two or more elements meet. And we will apply KCL at each node.</p><p>So
  for example, in this simple circuit where I would have three parts connected in
  what we would call parallel, they share a node at the top and they share a node
  at the bottom. So even though it looks like there''s multiple interconnects up here,
  we say that''s one node. And we would say that the sum of the currents into the
  node is equal to the sum of the currents out.</p><p>So if I lab all of the possible
  currents that come out of that node, I would have i1, i2, i3. i1 goes through the
  first one, the second one and the third one. And so I would conclude from Kirchhoff''s
  current law that the sum of i1, i2, and i3 is 0. OK. Easy, right?</p><p>As I said,
  we''re going to make an abstraction where the electrons don''t build up in the wires.
  They don''t even build up in the parts. They do get stored in the parts. That''s
  a little confusing, we''ll come back to that.</p><p>If they don''t build up in the
  parts, then the current that goes in this leg has to come out that leg. If that''s
  true, then i1 is i4, i2 is i5, i3 is i6, and we end up with another equation down
  here, which turns out to be precisely the same as the one at the top. Everybody''s
  happy with that?</p><p>So we''re thinking about this just the way we would think
  about water flow. If there''s water flow into a part, it better be coming out. If
  there''s water flow in a pipe, the water that goes into the pipe better come out
  of the pipe someplace.</p><p>So here is an arbitrary network made out of four parts.
  How many linearly independent KCL equations are there?</p><p>So how many linearly
  independent KCL equations are in that network? Everyone raise your hand, some number
  of KCL equations.</p><p>OK, I''m seeing a bigger variety. I see (1)''s, (2)''s,
  and (3)''s. I don''t see any (4)''s. That''s probably good.</p><p>So how do you
  think about the number of linearly independent KCL equations? So the first thing
  to do is to label things. So you have to have reference directions before you can
  sort of think about things.</p><p>So we have four elements. We would be expecting
  to see four element currents. The same current that goes into an element has to
  come out of it. So there''s element current 1, 2, 3, and 4. There are three nodes,
  so we might be expecting three KCL equations. Here''s one node from which you would
  conclude that the sum of i1 and i2 better be 0.</p><p>Here''s a node from which
  you would conclude that the current in i2 better be i3 plus i4.</p><p>And here is
  a node from which you would conclude that i1 plus i3 plus i4 is 0. So I can write
  one KCL equation for every node, that''s not surprising. But if you look at those
  equations, you''ll see that they''re not linearly independent. In fact, if you solve
  this one for i2-- it''s already solved for i2. Stick that answer up here, you get
  i3 plus i4 added to i1 is 0, which is just the same as that equation. So of those
  three equations, only two of them are linearly independent. The answer to that problem
  was (2).</p><p>And there''s a pattern. So think about the pattern in terms of figuring
  out the number of linearly independent KCL equations that are in a slightly more
  complicated network.</p><p>So what''s the answer here, how many KCL equations are
  in this network? Wow. Well, I''m not getting any of the answers I would have said.
  What does that mean? Ah, I''m forgetting to add 2. That''s my problem. OK, now I''m
  getting some of the answers that I would expect to get. OK, got it. I confused myself.</p><p>OK,
  the vast majority say (1). How do you get that? Which is 3. So again, you think
  of how in this circuit there are four nodes, A, B, C, D. So we can think about writing
  a KCL equation for each one. If we go to A, A has three currents coming out of it
  -- 1, 2, 3. So the sum of those has to be 0, et cetera. And if you think about those
  equations, they''re not linearly independent either.</p><p>If you work through the
  math, you see that there''s exactly one of those equations that you can eliminate.
  So you''re left with three linearly independent KCL equations. And so there''s a
  pattern emerging here. Somebody see the pattern?</p><p>1 minus. Can somebody prove
  the pattern?</p><p>So there''s a pattern here. The pattern is take the number of
  nodes and the number of independent KCL equations as one less. So the challenge
  is, can you prove it? And by the theory of lectures--</p><p>AUDIENCE: Yes.</p><p>PROFESSOR:
  Yes. And by a corollary of the theory of lectures, the way you would prove it is?</p><p>AUDIENCE:
  On the next slide.</p><p>PROFESSOR: On the next slide. Exactly. So how do I prove
  it? Yeah?</p><p>AUDIENCE: Whenever you take minus 1, you just add all the [UNINTELLIGIBLE]
  together [UNINTELLIGIBLE].</p><p>PROFESSOR: Yeah. So there''s something special
  about the last one. Why should there be something special about the last one.</p><p>AUDIENCE:
  Because the circuit''s closed.</p><p>PROFESSOR: Because the circuit''s closed. That''s
  right. So the idea is to sort of generalize the way we think about KCL. So we start
  with a circuit. We think about having four nodes here. It''s certainly the case
  that KCL holds for each node. So here''s KCL for that node. But now if you think
  about KCL for this node, and then add them, that looks like a KCL equation. But
  it applies to a super node.</p><p>Imagine the node defined by the black box, and
  think about the net currents into or out of the black node. This current i2, which
  leaves the red node, enters the green node, but doesn''t go through the surface
  of the black node at all. That''s exactly the current that''s subtracted out when
  we added the red equation to the green equation. Does that make sense? So KCL says,
  oh, if all the currents at a node have to sum to 0, and if elements have the same
  current coming out and going in, then if you draw a box around an element, what
  goes into the element is the same as what comes out of the element. It doesn''t
  change the net current through the surface. So the generalization of the KCL equation,
  KCL says the sum of the currents into a node is 0. The generalization says take
  any closed path in a circuit, the sum of the currents going across that closed path
  is 0.</p><p>So if we apply that rule again, think about node 3. If we add the result
  of node 3 to the black node, which was the sum of 1 and 2, we get the new green
  curve. We get the new green equation. And what that says is the sum of the currents
  going across the green super node-- OK, so what''s going on? i1 is coming out of
  it, i4 is coming out of it, i5 is coming out of it. So the sum of i1, i4, and i5
  has to be 0. Well, KCL says the sum of the currents coming out of a node must be
  0. The super KCL says the sum of the currents coming out of any closed region is
  also 0. But the interesting thing about this closed region is that it encloses all
  but one of the nodes. That''s always true. Regardless of the system, regardless
  of the circuit, you can always draw a line that will isolate one node from all the
  others. So what that proves is that you can always write KCL for this node in terms
  of KCL for those nodes. Ok.  So there''s a generalization then that says that you
  can always write KCL for every node. They will always be linearly dependent. So
  you can always throw away one.</p><p>So in some sense now, we''re done. We''ve just
  finished circuit theory. We talked about how every element has to have a law. A
  resistor is Ohm''s Law. A voltage source says that the voltage across the terminals
  is always a constant. A current source says that the current through the current
  source is always a constant. So every element tells you one law. We know how to
  think about KVL. So we know the rule for how the across variables behave.</p><p>What''s
  the aggregate behavior of all the across variables? Well, KVL has to be satisfied
  for every possible loop. The loops don''t have to be independent. You have to worry
  about whether they''re independent. The only simple rule we came up with-- we''ll
  come up with another one in a moment. The only simple rule that we came up with
  was for planar circuits, where the innermost loops were linearly independent of
  each other. And you have to write KCL for all the nodes, except one. One of them
  never matters.</p><p>So in some sense, we''re done. What we would do to solve the
  circuit, think about every element. For every element assign a voltage, a reference
  voltage. For every element, assign a current. Make sure they go in the right direction.
  We always define currents to go down the potential gradient. They always go in the
  directions through the element from the positive to the negative. So for every element,
  assign a current and a voltage.</p><p>We have 6 elements, that''s 12 unknowns. Now
  we dig and we find 12 equations. In this particular circuit, we found those 12 equations.
  There were three KCL equations, one for each of the inner loops. There were three
  KCL equations, one for each node except one. There were 5 Ohm''s law equations,
  one for each one of the resistors. There was one source equation for the voltage
  source. 12 equations, 12 unknowns, we''re done.</p><p>The only problem is a lot
  of equations. It''s not a very complicated circuit. We''ve only got 6 elements.
  I tried to motivate this in terms of studying networks that had 10 to the 9 elements.
  This technique is not particularly great at 10 to the 9. It would probably work.
  But we would probably be interested in finding simpler ways. So there are simpler
  ways you might imagine, and we''ll discuss two of them just very briefly.</p><p>The
  dumb way that I just talked about is what we call primitive variables, element variables.
  If you write all the element variables, v1, v2, v3, v4, v5 v6, all of the element
  currents, i1, i2, i3, i4, i5, i6, write all the equations, you can solve it. However,
  if you''re judicious, you can figure out a smaller number of unknowns and a correspondingly
  smaller number of equations. One method is called the node method.</p><p>When we''re
  thinking about the individual elements, the thing that matters is the voltage across
  the element. However, that''s not the easy way to write the circuit equations. A
  much easier way is not to tell me the voltage across an element, but instead tell
  me the voltage associated with each of the nodes.</p><p>If I tell you the voltage
  associated with every node, the important thing about that way of defining the variables
  is that you''re guaranteed that from those variables, you can tell me the voltage
  across every part. So for example, in this circuit, this voltage source-- so if
  I call this one ground, we''ll always have a magic node called ground. It is not
  special in the least. It''s just the reference voltage. I''ll come back to that.
  I''ll say words in a minute about what the reference is.</p><p>We always get to
  declare one node to be ground. We get one free node. It''s a node whose voltage
  we don''t care about because it''s the reference for all voltages. It''s a node
  whose current we don''t care about because we get to throw away one node when we
  do current equations. So we have one special mode called ground, about which we
  don''t care too much. Except that it''s the most important node in the circuit.
  Except for that, we don''t care about it. So this guy''s ground. We think about
  its voltage being 0. Then this voltage supply makes that node be v0. I don''t know
  what that is, so I''ll call it e1. And I don''t know what that is, so I''ll call
  it e2.</p><p>So if I tell you the voltage on all of those nodes, ground voltage
  is 0, the top voltage is v0, the left voltage is e1, the right voltage is e2. From
  those four numbers, 0 and 3 nontrivial numbers, you can find all of the component
  voltages.</p><p>So for example, the voltage v6, the voltage across R6 is e2 minus
  e1. The voltage v4, the voltage across the R4 resistor is e1 minus 0. So if I tell
  you all the node voltages, you can tell me all of the element voltages. And in general,
  there''s fewer nodes than there are components. OK, that''s great.</p><p>So instead
  of naming the volts across the elements, we''ll name the voltages at the nodes because
  there''s fewer of them.</p><p>Then, all we need to do in the node method is write
  the minimum number of KCL equations. We know we only have two unknowns, e1 and e2.
  And it turns out-- and you can prove this, but I won''t prove it today. It turns
  out that you need two KCL equations. Two unknowns, e1, e2, two KCL equations. And
  it turns out those two KCL equations are exactly the KCL equations associated with
  the two nodes.</p><p>So the current leaving e1, so KCL at e1 -- well, there''s a
  current that goes that way. Well, that''s the voltage drop in going from e1 to v0,
  e1 minus v0, divided by R2. That''s Ohm''s law. So this term represents the current
  going up that leg plus the current that goes through this leg, which is e1 minus
  e2 over R6. Plus the current going in that leg, which is e1 minus 0 over R4. The
  sum of those three currents better be 0. Analogously, the sum of the currents at
  this node must be 0, and the equation looks virtually the same. Because v0 is known,
  so it didn''t add an unknown. v0 was set by the voltage, by the voltage source.
  So I have two equations, two unknowns, solved. Done.</p><p>So rather than solving
  12 equations and 12 unknowns, I can do it with two equations and two unknowns. That''s
  called the node method. One of the most interesting theories about circuits is that
  every simplification that you can think about for voltage has an analogous simplification
  that you can think about in current. That''s called duality. We won''t do that because
  it''s kind of complicated. But it''s kind of a cute result.</p><p>If you can think
  of a simplification that works in voltage, then there is an analogous one, and you
  can prove it. In fact, you can formally derive what it must have been. This is a
  rule for how you can simplify things by thinking about voltages in aggregate. Rather
  than thinking about the element voltages, think about the node voltages.</p><p>The
  analogous current law is rather than thinking about the currents through the elements,
  the element currents, think about loop currents. OK, that''s a little bizarre. So
  we name the loop, the current that flows in this loop, IA, the current that flows
  in this loop, IB, and the current hat flows in this loop, IC. What on earth is he
  doing?</p><p>Well, the element voltages are some linear combination of those loop
  currents. And in fact, the coefficients in the linear combination are one and minus
  one. So the element current I4, the current that flows through the R4 resistor is
  the sum of IA coming down minus IC, which is going up. So there''s a way of thinking
  about each element current as a sum or difference of the loop currents. Everybody
  get that?</p><p>So instead of thinking about the individual element currents, I
  think about the loop currents. And now, I need to write three KVL equations. So
  in the node method, I named the nodes and had to write two KCL equations. Here,
  I named the loop currents and I have to write three KVL equations, one for each
  loop. It''s completely analogous. If you write out a sentence, what did you do?
  I assigned a voltage to every node, and I wrote KCL of all the nodes. Then if you
  turn the word &quot;current&quot; into the word &quot;voltage,&quot; the word &quot;node&quot;
  into the word &quot;loop,&quot; you derive this new method.</p><p>So this says that
  if I write KVL at the A loop, think about spinning around this loop, as I go up
  through the voltage source, so I go in the negative terminal here. So that''s minus
  v0. As I go down through this resistor, I have to use Ohm''s law, so that''s R2
  times the down current. Well, the down current is IA down minus IB up. So I went
  up through here, down through here. Now I go down through this one.</p><p>When I
  go down through that one, according to Ohm''s law, that''s R4 times the current
  through that element. That current-- well, it''s IA down and it''s IC up. So this
  is the KVL equation for that loop. I write two more of them, and I end up with three
  equations and three unknowns.</p><p>Both the node method and the loop method resulted
  in a lot fewer equations than the primitives did. I had 12 primitive unknowns, 6
  voltages and 6 currents. In the node method, I get the number of independent nodes
  as the number of equations and unknowns, which is less than the number of primitive
  variables. In the loop method, I have the number of independent loops. Which is
  again, smaller. So the idea then is that we have a couple of ways to think about
  solving circuits.</p><p>Fundamentally, all we have are the element relationships
  and the rules for combination. Oh, this is starting to sound like PCAP, primitives
  and combinations. So the primitives are, how does the element constrain the voltages
  and currents? We know three of those, Ohm''s law, voltage source, current source.
  And what are the rules for combination? Well, the currents add to the node, and
  the voltages add around loops.</p><p>OK, just to make sure you''ve absorb all that,
  figure out the current I for this circuit.</p><p>OK, what''s a good way to start?
  What should I do to start thinking about calculating I? OK, bad way. Assign voltages
  and currents to everything. 4 elements, that''s 4 voltages, 4 currents. That''s
  8 unknowns. Find 8 equations, solve. That''ll work. Bad way. What''s a better way?</p><p>OK,
  [UNINTELLIGIBLE PHRASE].</p><p>AUDIENCE: [UNINTELLIGIBLE PHRASE].</p><p>PROFESSOR:
  It was on the previous sheet. [UNINTELLIGIBLE PHRASE].</p><p>AUDIENCE: KVL [UNINTELLIGIBLE].</p><p>PROFESSOR:
  KVL for where?</p><p>AUDIENCE: Loops.</p><p>PROFESSOR: Which loop?</p><p>AUDIENCE:
  Left loop.</p><p>PROFESSOR: So do KVL on the left loop?</p><p>AUDIENCE: Yes.</p><p>PROFESSOR:
  OK, that''s good. But you have to tell me how to assign variables. Do you want 8
  primitive variables? 8 primitive variables are v1, i1, v2, i2, v3, i3, v4, i4. So
  that''s what I mean by primitive variables. Or element variables is another word
  for it.</p><p>What''s a better way than using element variables? Yeah.</p><p>AUDIENCE:
  Create 2 loop equations.</p><p>PROFESSOR: Create 2 loop equations, that''s fantastic.</p><p>AUDIENCE:
  I1 for the first loop, I2 for the second loop.</p><p>PROFESSOR: So if you do I1
  going around here, then I1 is actually I. And if you do I2 going around here, what''s
  I2?</p><p>AUDIENCE: [INAUDIBLE].</p><p>PROFESSOR: So if I think about I2 spinning
  around this loop, so the sum of I1 and I2 goes through that box. But the only current
  that goes through this box is?</p><p>AUDIENCE: [INAUDIBLE].</p><p>PROFESSOR: So
  the suggestion is that I think about-- so if I have I1 here, but I know that''s
  I. Then I can see immediately that since the only current that goes through here--
  so if I have I1 and I2. That was a very clever idea. If you have I1 and I2, the
  only current that goes through here is I. So I1 must''ve been I.</p><p>The only
  current that goes over here must''ve been this guy. So this must be minus 10. So
  I could redo that this way. I could say I''ve got 10 going that way. That make sense?
  So now I only have one unknown which is I. So that''s a very clever way of doing
  it. So what I could do is showed here.</p><p>I have I going around one loop and
  I have 10 going around that loop. That completely specifies all the currents. So
  now all I need to do is write KVL for these different cases.</p><p>So if I write
  KVL for the left loop, then I get going up through here, that''s minus 15, and going
  down through here, going to the right through this guy is 3I. Going down through
  this guy is 2 times I plus 10. Both of these are going down, so you have to add
  them. So I get one equation and one unknown. And when I solve it, I get minus one.
  That make sense?</p><p>There''s an analogous way you could have done it with one
  node. You could have said that the circuit has a single node and figured out KCL
  for that one node. KCL would be the sum of the currents here. There''s a current
  that goes that way, that way, and that way. And again, you end up with 1 equation
  and 1 unknown. Yes?</p><p>AUDIENCE: [UNINTELLIGIBLE PHRASE].</p><p>PROFESSOR: Correct.
  If I thought about this current going this way, it would be minus 10. If I flipped
  the direction, then it''s plus 10. So the loop current has the property that it''s
  the only current through this element. So that has to match. It''s one of two currents
  that go through this element.</p><p>AUDIENCE: You said that everything that [UNINTELLIGIBLE
  PHRASE].</p><p>PROFESSOR: This loop is [UNINTELLIGIBLE]. Yes.</p><p>AUDIENCE: So
  why is the [UNINTELLIGIBLE PHRASE].</p><p>PROFESSOR: Correct. I want to have this
  picture now.</p><p>So if I''m doing it with loops, I have two loops. The current
  through this element is just I. The current through this element is just I. The
  current through this element is just 10. The current through this element-- well,
  the sum of these two currents go through that element. Does that make sense?</p><p>AUDIENCE:
  [INAUDIBLE]</p><p>PROFESSOR: This loop current is just a fraction of the current
  in the whole system. So this loop current goes through this element and contributes
  to this element. But so does that one. OK, if you''re still confused, you should
  try to get it straightened out in one of the software labs or the hardware lab,
  or talk to me after lecture. But the idea is to decompose in the case of the node
  voltages. Think about the element voltages in terms of differences in the node voltages.</p><p>In
  the case of the loop currents, think about the element currents in terms of a sum
  of loop currents. OK, so the answer is minus 1 regardless of how you do it. Ok.  The
  remaining thing I want to do today is think about abstraction.</p><p>We''ve talked
  about the primitives, which are things like resistors, voltage sources, and current
  sources. Means of combinations, that''s KVL and KCL. Now we want to think about
  abstraction.</p><p>And the first abstraction that we''ll talk about is, how do you
  think about one element that represents more than one element? This is the same
  thing that we did when we thought about linear systems, when we did signals and
  systems. We started with R''s and K''s and pluses, and we made single boxes that
  had lots of R''s and pluses and gains in them.</p><p>What was the name of the thing
  that was inside the box? If we combined lots of R''s, gains, and pluses into a single
  box, what would we call the thing that''s in the box?</p><p>AUDIENCE: [INAUDIBLE].</p><p>PROFESSOR:
  Shout again.</p><p>AUDIENCE: System function.</p><p>PROFESSOR: System function.
  Right?  So we started with boxes that only had things like R''s in them. But eventually,
  we got boxes that looked like much more complicated things like that. We thought
  about a system function which was a generalized box, that could have lots of R''s,
  or lots of gains, or lots of pluses in it. And that was a way of abstracting complicated
  systems so they looked like simple systems. What we want to do here is the same
  thing for circuits.</p><p>We want to have a single element, a single circuit element,
  that represents many circuit elements. And the simplest case of that is for series
  in parallel combinations of resistors. It''s very simple to think about how if you
  had two Ohm''s law devices connected in series, you could replace those two with
  a single resistor. And the voltage-current relationships measured at the outside
  of the box would be the same. That''s how we think about an abstraction in circuits.</p><p>When
  is it that you can draw a box around a piece of a circuit and think about that as
  one element? The very simplest cases, the series combination of two resistors, same
  sort of thing happens for the parallel combination. And that simple abstraction
  makes some things very easy.</p><p>What would be the equivalent resistance for a
  complicated system like that? Well, that''s easy. All you need to do is think about
  successively reducing the pieces. Here I''m thinking about that having four resistors.
  I can just successively apply series and parallel in order to reduce that, make
  it less complicated.</p><p>So I can think about combining these two in series to
  get, instead of two 1 Ohm resistors, one 2 Ohm resistor.</p><p>Then I can think
  about these two 2 Ohm resistors being equivalently one parallel 1 Ohm resistor.
  And so this whole thing looks as though it''s just 2 Ohms from the outside world.
  That''s what we mean by an abstraction. What we''re trying to do and what we will
  do over the next two weeks, is we''ll think about ways of combining circuits so
  that we can reduce the complexity this way.</p><p>Another convenient way of thinking
  about reducing the work that you need to do is to think about common patterns that
  result. PCAP, Primitives, Combinations, Abstractions. So the series of parallel
  idea was an abstraction. A pattern, here''s a common pattern. If you''ve got two
  resistors in series, if the same current flows through two resistors, then there''s
  a way of very simply calculating the voltage that falls across each. So you can
  think about the sum resistor, R1 plus R2 since they''re in series. So that allows
  you then to compute the current from the voltage. Then the voltage that falls across
  this guy is by Ohm''s law, just the current times its resistor, which is like that.</p><p>And
  similarly with this one. So you can see that some fraction of this voltage v occurs
  across the v1 terminal. And some different fraction appears across the v2 terminal,
  such that the sum of the fractions is, of course, v. That''s what has to happen
  for the two. And there''s a proportional drop. The bigger R1, the bigger is the
  proportion of the voltage that falls across R1. So it''s a simple way of thinking
  about how voltage drops across two resistors. There''s a completely analogous way
  of thinking about how current splits between two resistors.</p><p>Here the result
  looks virtually the same, except it has kind of the unintuitive property that most
  of the current goes through the resistor that is the smallest. So you get a bigger
  current in i1 in proportion to the R2. So it works very much like the voltage case,
  except that it has this inversion in it, that the current likes to go through the
  smaller resistor.</p><p>OK, so last problem. Using those kinds of ideas, think about
  how you could compute the voltage v0 and determine what''s the answer.</p><p>So
  what''s the easy way to think about this answer? What do I do first?</p><p>AUDIENCE:
  Superposition.</p><p>PROFESSOR: So superposition? That''s one thing.</p><p>AUDIENCE:
  Simplify [UNINTELLIGIBLE].</p><p>PROFESSOR: Simplify. So what''s a good simplification?
  Collapse?</p><p>AUDIENCE: You can put the two [UNINTELLIGIBLE] in series and treat
  them as one.</p><p>PROFESSOR: So you can treat this as a series combination, and
  you can replace the series of 1 and 3 with a?</p><p>AUDIENCE: [UNINTELLIGIBLE PHRASE].</p><p>AUDIENCE:
  4..</p><p>PROFESSOR: 4. So this can be replaced by four [UNINTELLIGIBLE] resistor.
  Now what?</p><p>AUDIENCE: You can do the same on the parallel one.</p><p>PROFESSOR:
  So you can replace the parallel of the 6 and a 12 with a?</p><p>AUDIENCE: 4.</p><p>PROFESSOR:
  Amazing -- with a 4. So there''s a 4 there and there''s a 4 there. And the answer
  is?</p><p>AUDIENCE: It''s half.</p><p>PROFESSOR: Half of whatever it was by voltage
  [UNINTELLIGIBLE] relationship. So you think about this becoming that. You think
  about the parallel becoming that. You get a simple divide by 2 voltage divider.
  So the answer is 7 and 1/2, which was the middle answer. And so what we did today
  was basically a whirlwind tour of the theory of circuits. And the goal for the rest
  of the week is to go to the lab and do the same sort of thing with practical where
  you build a circuit, and try to use some of these ideas to understand what it does.
  &nbsp;</p>'
type: course
uid: 9fe057844e7944c539f15aa427f7e263

---
None