---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: e7Ptvu5Vu8k
  parent_uid: 91d15eafb8d5ed156d1a759c77d54fa9
  title: Video-YouTube-Stream
  type: Video
  uid: 7b54aa9be59adda7093ec3b7fd065a65
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/lecture-8-op-amps/id490181666?i=109416110
  parent_uid: 91d15eafb8d5ed156d1a759c77d54fa9
  title: Video-iTunes U-MP4
  type: Video
  uid: 6a4fa7a9cd1a45ff1b0e0234688fbd73
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_S11_lec08_300k.mp4
  parent_uid: 91d15eafb8d5ed156d1a759c77d54fa9
  title: Video-Internet Archive-MP4
  type: Video
  uid: 735df7ecd0cd4ac31e890fc76fbbb35b
- id: Thumbnail-YouTube-JPG_1
  media_location: https://img.youtube.com/vi/e7Ptvu5Vu8k/default.jpg
  parent_uid: 91d15eafb8d5ed156d1a759c77d54fa9
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 5f113635c18b4602cef69849f7296a8f
- id: MIT6_01SC_S11_lec08_300k.srt
  parent_uid: 91d15eafb8d5ed156d1a759c77d54fa9
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/op-amps/lecture-1-object-oriented-programming/MIT6_01SC_S11_lec08_300k.srt
  title: MIT6_01SC_S11_lec08_300k.srt
  type: null
  uid: b1d25473b4b1617cb55cf4db0439ace5
- id: Caption-OCW-SRT
  parent_uid: 91d15eafb8d5ed156d1a759c77d54fa9
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: 57939453bedfb065185a17cdde3a7503
- id: MIT6_01SC_S11_lec08_300k.pdf
  parent_uid: 91d15eafb8d5ed156d1a759c77d54fa9
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/op-amps/lecture-1-object-oriented-programming/MIT6_01SC_S11_lec08_300k.pdf
  title: 'MIT 6.01SC S11 Lecture 8: Op-Amps Transcript'
  type: null
  uid: df3199b89b9cad03924ce0067d2d3c09
- id: Transcript-OCW-PDF
  parent_uid: 91d15eafb8d5ed156d1a759c77d54fa9
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: 51a51ae8a1b5921192d83df4e9882e25
inline_embed_id: 24439581lecture8:op-amps47957890
layout: video
order_index: null
parent_uid: 6912b6f0dfbf7463fa378df8bde18e96
related_resources_text: ''
short_url: lecture-1-object-oriented-programming
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/op-amps/lecture-1-object-oriented-programming
template_type: popup
title: 'Lecture 8: Op-Amps'
transcript: '<p>The following content is provided under a Creative Commons license.
  Your support will help MIT OpenCourseWare continue to offer high-quality educational
  resources for free. To make a donation or view additional materials from hundreds
  of MIT courses, visit MIT OpenCourseWare at ocw.mit.edu.</p><p>PROFESSOR: Hello.
  Welcome. Welcome back from spring break. Today what I want to do is talk about op-amps.
  And in particular what I want to do is talk about modularity in circuit design.
  How do you make circuits that are modular? We''ll see that there''s special problems
  when you think about modularity applied to circuits. And op-amps are one solution
  for helping us think about those problems.</p><p>Before launching straight into
  something new though, I''d like to recap where we are under the assumption that
  you may not have been thinking about this exactly currently. So last time we took
  our first look at circuits. Circuits are very different from the kinds of things
  we''ve thought about before.</p><p>Before, in programming, in linear systems theory,
  we thought about blocks that had well-defined inputs and well-defined outputs. Circuits
  are different. Circuits are all connected together. And circuit theory is thinking
  about how do you organize your thoughts about complicated interactions among things.</p><p>The
  parts interact because they touch each other and they share voltages. Because they
  touch each other, they share currents. And you have to somehow think about that
  whole complicated system. We figured out that the way you think about that, you
  can think about it as three separate enterprises. How do you think about voltages.
  How do you think about currents. And how do you think about the elements.</p><p>How
  do you think about voltages? Well, the sum of the voltages around any closed loop
  is zero. Done. KVL -- Kirchoff''s Voltage Law. How do you think about currents?
  Draw any surface. The net current that leaves the surface is zero. KCL -- Kirchoff''s
  Current Law.</p><p>How do you think about the elements? Well it depends on the element.
  If you''re thinking about a linear resistor, it''s Ohm''s Law, V equals IR. If you''re
  thinking about a source, it could be a voltage source, then V equals v0, some fixed
  number. If you''re thinking about a current source, then current is fixed at some
  fixed number. So it depends. When you''re thinking about the element laws, it depends
  on what element you are thinking about.</p><p>And then you just combine all of those,
  and you can solve the circuit. The only problem that arises is that those equations
  are highly redundant. There''s a lot more KVL equations than you need. There''s
  a lot more KCL equations than you need. And so in fact, the trick in analyzing a
  circuit is to figure out the smallest number of equations that are adequate, the
  number of equations that are necessary and sufficient to find a solution.</p><p>Last
  time we went through three different ways to do that. We thought about what I will
  think of as primitive or element voltages and currents. The idea in that technique
  is you think about every element and assign to that element its voltage and its
  corresponding current. Then that gives you, as in this example if you''ve got six
  elements, that gives you six unknowns, one voltage across every element, one current
  through every element. So then you''ve got to dig up six other relationships. Sorry,
  start again. Six elements, six voltages, six currents, 12 unknowns, you need to
  come up with 12 equations. Six of them are element equations.</p><p>So six are easy.
  Then you have to come up with six more. And for this particular circuit, it turns
  out that there is three independent Kirchoff''s Voltage Law equations. And there
  are three independent KCL, Kirchoff''s Current Law equations. 12 equations, 12 unknowns
  to solve, done.</p><p>That''s actually more work than you need to do. So we looked
  at two other techniques for solving the same kind of circuits. One''s called node
  voltages and another is called loop currents. They are duals of each other. In the
  node voltage method you figure out exactly the minimum number of voltages that I
  would have to tell you in order to specify all of the element voltages.</p><p>So
  for example, if I told you this voltage here, and that voltage there, and this voltage
  there, and that voltage there, four of them, that would let you calculate all of
  the element voltages. But now I only have four instead of six. Four nodes instead
  of six element voltages. So it''s smaller. And we talked about last time how you
  could find the correct equations that go with those node voltages.</p><p>In the
  loop current method, you specify the minimum number of currents that would be sufficient
  to account for all of the element currents. And here in this circuit it required
  three. Three is smaller than six. There were six element currents. So again we''ve
  got a reduction in the number of unknowns -- 12 4, 3. So that''s kind of the idea.</p><p>And
  just to make sure that you''re all with it, think about this problem. How many of
  the following expressions are correct? Feel free to talk to your neighbor. At the
  end of about 45 seconds, I''ll ask you to raise your hand with a number of fingers,
  (1) through (5) -- indicating which is the correct answer. Dead silence. You''re
  allowed to talk.</p><p>OK, so how many of the relations are true? Everybody raise
  your hand. Indicate a number fingers that tells me how many of the answers are correct.
  Come on. Blame it on your neighbor. You can say anything, right? It''s always your
  neighbor''s fault. That''s very good. It''s about 95% correct, almost all correct.</p><p>This
  first equation, what is this? Give that a name. KVL. Is it correct? Sure. You need
  to figure out which path it corresponds to. It goes through-- The only v''s are
  over here. So therefore it must be something that has to do with this circuit. So
  this says that there''s 1, 2, 6, and 5. That''s path 1, 2, 6, and 5. So all you
  really need to do is check the polarities.</p><p>So if we took all of the variables
  to the same side, then we''d have minus v1 plus v2 plus v6 plus v5. If we think
  about going a loop that goes through the minus v1, that would be this way. Plus
  v2 plus v6 plus v5. So that''s right. Easy.</p><p>What''s the point of this equation?
  v6 equals e1 minus e2, what''s that say? Why''d I ask that? Yeah.</p><p>AUDIENCE:
  It''s saying that  the--</p><p>PROFESSOR: Exactly, it''s intended to make you think
  through the relationship between the primitive variables, the element voltages,
  and the node voltages. If I told you the node voltages e1 and e2, you could trivially
  compute v6. You could also compute any of the other v''s.</p><p>If I told you to
  find v-- what is that? My eyes are not very good. v4, if I told you to find v4,
  that would be e1 minus ground. We assign the number 0 to ground, so that would be
  e1. So the idea, the reason I ask number (2), is to make you think about how you
  relate the node voltages to the element voltages.</p><p>How about number (3), what''s
  that? Well it''s highly related to number (2). But it''s different from number (2),
  because?</p><p>AUDIENCE: Ohm''s Law?</p><p>PROFESSOR: Ohm''s Law. So equation (3)
  is the way Ohm''s Law looks when you use node equations. Ohm''s Law is a little
  bit uglier when you use node equations than when you use primitive variables. When
  you use primitive variables, the same relationship would''ve simply said that v6
  is R6 times i6. Because I''m using node voltages instead, the voltage across resistor
  six shows up as a difference.</p><p>How about this one? What''s that? True or false,
  this is KCL?</p><p>AUDIENCE: False.</p><p>AUDIENCE: False.</p><p>AUDIENCE: --KCL.</p><p>PROFESSOR:
  True. This is KCL, true. OK. This is KCL, false. Well, obviously we''re numerous.
  And it''s not, sort of, 100% participation, but-- This is not KCL. What is that?
  KCL says that the sum of current out of some closed path. This is mixed thing. i6
  is one of these things. And IB and IC is one of these things. So what is the equation
  for?</p><p>AUDIENCE: Incorrect.</p><p>PROFESSOR: Incorrect, yes. What would be the
  correct way of saying equation (4)?</p><p>AUDIENCE: i6 equals-- i6 is--</p><p>PROFESSOR:
  The answer to set questions according to the theory of lectures is go to the next
  slide. Here''s the correct expression. Why is this correct, and why is that not
  correct? Equation (4) is intended to be how do you relate the loop current to the
  element currents?</p><p>So i6 is an element current. It''s the current that goes
  through R6. When we do loop currents, we have two currents going through R6. So
  in the loop current view, the total current that goes through R6 is a sum or difference
  of the two loop currents that go through R6. So the element current through R6,
  which is i6, is a sum or difference of loop currents.</p><p>There are two loop currents
  we have to worry about. Which one goes through in the correct direction? i6 goes
  from left to right. So when we do the loop currents, we need to take positive as
  the direction from left to right. Well that''s the direction of IC and is the opposite
  direction of IB. So if I want to use loop currents to specify i6, it would be IC
  minus IB. Everybody clear on that? So equation (4) is the relation between element
  currents and loop currents.</p><p>So what''s equation (5)? Equation (5) is Ohm''s
  Law for loop currents. Again, if I were thinking about Ohm''s Law for R6, I would
  have v6 equals i6 R6. That''s the way you say it in element voltages and currents.</p><p>Over
  here, the current through R6 is IC minus IB. So Ohm''s Law looks a little bit more
  complicated. So the point is these three methods represent ways of figuring out
  a linearly independent set of unknowns and equations. They differ.</p><p>The left
  hand one is probably the easiest to think about, especially when you''re thinking
  about things like Ohm''s Law. It''s the natural way to specify the element relationships.
  It''s the relation between the voltage and current through that part. That generally
  gives me a large number of equations and unknowns.</p><p>You can reduce the number
  of unknowns by using something like node voltages or loop currents. And that gives
  you fewer equations to solve. They are completely equivalent. They look a little
  different. And the reason for talking about them is that when we think about writing
  a program to solve circuits automatically, which by the way will be the exercise
  in software lab this week. When we think about writing a program, writing a program
  is yet a different kind of challenge.</p><p>What''s the easiest system to automate?
  So the system that is easiest for you may or may not be the easiest system to automate.
  So that''s the point of this week''s software lab. We''ll do a method that''s closely
  related to the node voltage method. It''s not quite node voltages. It''s a little
  simpler than node voltages for a computer. It''s a little simpler to automate. So
  we use a method that''s called node voltages with component currents.</p><p>OK,
  now I''m going to start new stuff. That was review. What I want to think about today
  is what is it about circuit design that makes it hard. What are the issues that
  make it difficult to be modular when we''re thinking about the analysis and design
  of circuits.</p><p>And one of the hardest things to deal with is the idea that in
  a circuit, unlike in a linear time invariant system of the type we talked about
  in the previous module, in a circuit the presence of every element affects the currents
  and voltages through, in principle, every other element. So if you change one thing,
  you change everything.</p><p>So first off, I want to just give an example of that.
  Think about what would happen if I were trying to make a circuit to control the
  brightness of a light bulb. So I imagine that I''ve got this circuit and I close
  the switch. Closing the switch is equivalent to adding a component. So before I
  close the switch, when the switch was open, I have three elements, a voltage source
  and two resistors. After I close the switch, I have four elements, the original
  three plus the bulb. So the question is how would closing the switch affect V0 and
  I0.</p><p>Take a minute. Talk to your neighbor. Figure out how V0 and I0 change.</p><p>So
  what''s the answer? Everybody raise your hand, show a number of fingers equal to
  the answer. That''s very good. It''s 95% correct at least, maybe 100. OK, so the
  answer is (2). Why is the answer (2)? How do I figure that out?</p><p>AUDIENCE:
  So the total resistance of the circuit is going to decrease because you''re adding
  it in parallel. And then V0 is going to decrease because it''s going to have a lower
  equivalent resistance. And because that decreases, you have I0 to--</p><p>PROFESSOR:
  Yes, I think that''s exactly correct. So the idea was that when you add a component--
  Let''s think about the light bulb being a resistor. That''s kind of pulled out of
  thin air, but I sort of suggested that you might do that here. Think about representing
  the light bulb as a resistor. Then when you close the switch, these two resistors
  go in parallel. When you combine two things in parallel, the result is the same
  as a resistance that has a smaller value. And then think about how that smaller
  value would interact with this resistor and that source. And you can sort of figure
  out that the presence of this bulb would reduce this voltage and increase that current.</p><p>That''s
  kind of a high level of reasoning given where we are. If you wanted to think through
  this a little more step by step, it''s easy. You could think about figuring out
  what are the voltages and currents before and after you close the switch.</p><p>Before
  you close the switch, you can just ignore this, and you can calculate V0 just from
  a voltage divider relationship. Right, that''s clear? So you can see that when the
  switch is open, the voltage, V0, is going to be 8 Volts. And when the switch is
  open, you can figure out I0 by lumping these two resistors together to make a 3
  Ohm resistor. And you see that I0 is 4 Amps. Then to figure out what happens when
  you close the switch, just repeat. And the algebra is a little more tedious. I won''t
  try to go through it.</p><p>By the way, the answers, the slides that I show in lecture
  are always posted on the web. So these slides that have the answers, they are there.
  On the web there are two handouts per lecture. There''s an electronic version of
  the thing that we handed out. There''s also an electronic version of my slides.
  So everything that I showed is there.</p><p>I''m not going to go through the tedious
  algebra. It''s just tedious algebra. But if you go through the tedious algebra,
  you find that if you represent this bulb by resistor R, V0 becomes an expression
  that looks like this.</p><p>If you think about resistors, physical resistors, if
  you think about light bulbs being represented by a physical resistor, then the physical
  resistor has to have a resistance between 0 and infinity. And if you think about
  that expression, what could the value be if R varied between 0 and infinity? That
  expression is always less than or equal to 8 Volts, showing that V0 went down when
  you closed the switch.</p><p>Similar tedious algebra leads to an expression like
  this in R. And if you think about how this would change as R goes from 0 to infinity,
  you see that that''s always bigger than 4 Amps. So that means I0 goes up.</p><p>So
  the point is you can think through this in a more sophisticated way. And we hope
  by the end of the course you''ll all be able to do that. Or you can think through
  it in terms of just solving the circuit. Solve it in two cases when the bulb is
  there and when the bulb is not. Either way, the answer is (2). The V0 went down,
  and I0 went up.</p><p>The point is that when I added the element, currents that
  were far away from the element still changed. And that''s a general way circuits
  interact. They''re all connected. So the idea, the point of doing this is that the
  addition of a new element changed the voltages and currents through the other element.</p><p>That''s
  a drag if what I was trying to do, for example, was design a brightness controller
  for the flashlight bulb. Imagine that what I really wanted to do was use a voltage
  divider to make 8 Volts. And what was in my head was I''d like that 8 Volts to be
  across the light bulb. That''s a good idea. It just won''t work. At least It won''t
  work the way this circuit worked.</p><p>If I just build it like so, there''s an
  interaction between the bulb and the voltage divider circuits, so the voltage divider
  circuit is no longer a voltage divider. After, in this circuit, when I close the
  switch, current flows in this wire. The rule in a voltage divider is the same current
  has to flow through both resistors. If the same current flows through two resistors,
  then you can use the voltage divider relationship to see how voltage partitions
  between the two resistors.</p><p>If current gets siphoned off the node between the
  two resistors, you can''t use the voltage divider relation anymore. That violates
  the premise of the voltage divider relation. So when I close the switch, this is
  no longer a voltage divider, and it no longer works like a voltage divider. Is that
  clear?</p><p>So what I''d really like is some magic circuit that I can put here
  that isolates the effect of the bulb on the effect of the rest of the circuit. And
  that''s exactly what an op-amp does. That''s what we''re going to talk about next.</p><p>So
  this magic circuit is something that we''ll call a buffer. A buffer is a thing that
  isolates the left from the right. So the buffer is going to be something that measures
  the voltage on this side and magically generates that voltage over here without
  changing this side.</p><p>So what we want to do now is develop some thought tools
  for how you think about op-amps. Op-amps are different. And if you just look at
  the picture, op-amp has to be different because there''s too many terminals.</p><p>It''s
  not like a resistor that has two legs. It''s not like a V source which has two legs.
  It''s not like an I source which has two legs. It has three legs. In fact, I haven''t
  drawn all the legs. There''s more than three. There''s at least five.</p><p>So they''re
  different. And the way we think about them are different. The key to thinking about
  the way an op-amp works is to think about a new class of elements called controlled
  elements. So a controlled element is an element whose voltage current relationship
  depends somehow on a voltage and current measured someplace else in the circuit.</p><p>As
  an example, think about a current controlled current source. That''s depicted here.
  I would normally write a current source that was a circle. That means it''s an independent
  current source. That means that the current is fixed. The little diamond thing is
  my way of representing the idea that the amount of current that comes out of this
  current source depends on something else. In this case it depends on IB. And IB
  happens to be a current that flows in that circuit.</p><p>So the idea is that the
  current in the current source depends on some other current. It''s a current controlled
  current source. It''s a current source whose current is controlled by another current.
  Got it? So we''ll see. Figure out, for this current controlled current source circuit,
  what''s the ratio of Vout over Vin?</p><p>So what''s the answer? What''s the ratio
  of Vout over Vin? 100%, wonderful. The answer is (4). Easy to get. It''s easy to
  get because I rigged this question to be easy. I rigged it to be easy because you
  can sort of figure out everything that''s going on on the left. And then you can
  figure out everything that''s going on on the right. And so there''s no sort of
  complicated coupling between the two.</p><p>So what''s going on on the left, well,
  you can solve for IB. IB is just Vi over 1,000 Ohms. Then you can take that value
  of IB and use that to solve for what''s going on over here. Over here the out is
  this current, 100 IB times this resistance, 5 Ohms. But we just found out that IB
  is VI over 1,000 Ohms. Substitute it in, you get half Vi. So the answer is number
  (4). The ratio of Vout to Vin is a half.</p><p>So the point is these are a different
  kind of element, controlled sources, dependent sources. But they''re not too hard
  to work with. They sort of look different structurally.</p><p>So think about what''s
  going on here. The controlled current source, the current controlled current source,
  I have to think of that as a box, because the current source has to know the value
  of IB. So somehow this box, this thing that''s doing this current controlled current
  source, it knows about IB, and it knows about the current source. So they''re somehow
  linked. So that''s why I put a box around it. And then think about the equations
  that characterize that component.</p><p>So now we''ve got a component that''s got
  four wires coming out of it. The components we had before had two wires coming out
  of them, resistors, current sources, voltage sources. This kind of a component has
  four wires coming out of them. We call this kind of a component a two-port because
  we think of the left port and the right port. That''s compared to resistor, which
  we would call a one-port. We think about this being a two-port. And there''s now
  two equations.</p><p>Now I''ve got, for that two-port, I''ve got two voltages and
  two currents. There''s the voltage across the left part. And there''s the voltage
  across the right part. And there''s current through the left part. And there''s
  the current through the right part. So with the elements we''ve thought about before,
  I had one voltage across it and one current through it. Now I''ve got two voltages
  across it and two currents. It''s kind of twice as big. Not surprisingly, it takes
  twice as many equations.</p><p>Ohm''s Law was a single equation for one resistor,
  a one-port. V equals V0 was one equation for one component, a voltage source. Here,
  I''ve got one component that has four wires, four unknowns. And I get two equations.
  So for this particular dependent source, I know that the voltage across this pair
  of terminals is 0, because it''s essentially a short circuit between the two. Short
  circuit just means connected with a wire. And I know that the current I2 is related
  to the current over there this way.</p><p>The idea then is that this current controlled
  current source can be represented by a two-port, two voltages, two currents related
  by two equations. It''s kind of structurally twice as difficult to think about as
  a one-port. Functionally, it''s different from having two one-ports, because the
  two one-ports are coupled. And that''s the important part is the coupling between
  the two that you can''t model with a simple resistor and a simple constant source.</p><p>So
  when we think about an op-amp, a good first model for an op-amp is to think about
  it as a voltage controlled voltage source. And so that''s depicted here. I want
  to think about the op-amp, which I''ll symbolically write this way. This means something
  that has two inputs, a plus input and then a minus input, and a single output, Vout.</p><p>I
  can think about it as a voltage controlled voltage source. This I mean to be the
  element representation. This is how I''ll draw it when I make a schematic diagram
  of a circuit. This is the functional form. This is the way I''ll think about it
  when I''m analyzing it. I''ll think about the op-amp as being a voltage controlled
  voltage source.</p><p>This voltage source adopts a voltage that is some number K
  times the difference voltage Vplus minus Vminus. And the trick in op-amps is that
  K is typically a very big number, typically bigger than 10 to the 5th. We''ll see
  in a minute why that''s a frightfully useful component.</p><p>Let''s just walk through
  an example to see how you would solve a circuit that has this kind of a voltage
  controlled voltage source in it. So think about this circuit where I''m applying
  a voltage to the plus lead of an op-amp, and I''m wrapping the output back through
  the minus lead, through two resistors. And what I want to do is analyze that circuit
  by thinking about the op-amp as a voltage controlled voltage source.</p><p>So I
  can see just by the way it''s wired up that the voltage at the plus lead-- So I''m
  going to be thinking node voltages. Node voltages tend to be easy. I''m thinking
  node voltages. So I''m going to define all my voltages referenced to a ground. So
  I''ll call this node ground. That''s what the funny symbol means. Then this node
  voltage, the voltage at the plus terminal, is just the same as the input voltage.
  This voltage at the minus terminal looks like a voltage divider relationship.</p><p>If
  you look at my model, it''s very clear that I1 is 0, because there''s no connection
  here between the Vplus and the Vminus. So I1 is 0. That means the total current
  that flows into the plus lead of the op-amp is 0. The total current that flows into
  the minus lead of the op-amp is 0. So because there''s no current flowing in the
  plus and minus leads, I can calculate the voltage at this minus terminal as a voltage
  divider. And it''s just R1 over the sum of R1 and R2 times V0.</p><p>Then according
  to the voltage control voltage source model, Vout should be K times the difference
  between Vplus and Vminus. So I just substitute in for Vplus -- this guy, Vi, and
  for Vminus -- this guy. Do some algebra. I get this expression after some algebra.</p><p>And
  then I say, yeah but I know that K''s really big. So if K''s really big, KR1 is
  big compared to R1. So I can ignore that. In fact, K is so big that for any reasonable
  choice of R1 and R2, KR1 is even bigger than R2. So that means this reduces to this
  kind of a fraction.</p><p>So the response of this circuit, this op-amp circuit--
  So what did I do? I just took the op-amp circuit, and I modelled it as a voltage
  controlled voltage source, plugged through the equations, and found out that the
  ratio of the output voltage to the input voltage is R1 over R1 plus R2 divided by
  R1.</p><p>So the idea then is that this simple circuit works like an amplifier.
  It''s an amplifier in the sense that I can make the output voltage bigger than the
  input voltage. That''s a very useful thing. In fact you''ll find useful ways to
  use that when you do the design lab this week. So this as an amplifier.</p><p>So
  here''s a question. Make sure you follow what I just did. How could I choose the
  components R1 and R2 so that I make Vout equal to Vi?</p><p>AUDIENCE: Why is this
  0?</p><p>PROFESSOR: There''s no wire connecting.</p><p>AUDIENCE: Oh.</p><p>PROFESSOR:
  So there''s nowhere for current to go.</p><p>OK so how would I choose the components
  R1 and R2 in order to make the output voltage equal to the input voltage?</p><p>Wonderful.
  So the idea is that all of these manipulations have the same effect. All you need
  to do is look at the expression that we developed. The expression was R1 plus R2
  over R1. If you substitute, R1 goes to infinity, R2 equals 0, or the two at the
  same time, you get one in all of those cases. So that''s a way that you can turn
  this amplifier circuit, that in general would make the output bigger than the input,
  into something that makes the output equal to the input.</p><p>Now I want to turn
  to a simplification. I just dragged you through the math. Thinking about the op-amp
  as a voltage controlled voltage source, there''s actually a shortcut. The shortcut
  is something we call the ideal op-amp. So what I want to do in this slide is drag
  you through the math one more time, but then we''re done.</p><p>The idea is that
  if you have an op-amp, a voltage controlled voltage source, if you represent an
  op-amp as a voltage controlled voltage source, and if K is very big, the effect
  will be to make the difference between the positive and negative terminals of the
  op-amp quite small. You can see that here by way of a simple example.</p><p>So let
  me think about this case with, again, the voltage controlled voltage source model.
  So here I''ve got Vout. According to the voltage controlled voltage source model,
  Vout should be K times the difference between the two inputs. The positive input
  is clearly Vi. The negative input is Vo. One equation, two unknowns, solve for the
  ratio.</p><p>The ratio of Vout to Vi is K over (1 plus K). That''s the answer. Take
  that answer and back substitute to figure out how big was the difference between
  Vplus and Vminus. That''s just algebra. And what you see is that if this is the
  answer, then Vplus minus Vminus can be written as a fraction of Vi or a similar
  fraction of Vo.</p><p>K is big. K is essentially the same as K plus 1. K is in the
  denominator of both. What that says is the difference between the plus and the minus
  leads, the voltage between the plus and the minus leads, is very small if K is very
  large. OK? So we call that the ideal op-amp relationship.</p><p>The utility of that
  is that it makes solving the op-amp circuits much, much easier than what we''ve
  just been doing. I''ve been solving the circuits by thinking about the op-amp as
  a voltage controlled voltage source. That''s fine. But if I additionally know that
  K is very big, I can shortcut it. I can say, look, the effect of the op-amp is going
  to be to make the positive and negative inputs the same. If it didn''t do that,
  think of what it would mean.</p><p>If K is a big number, and if the output voltage
  is K times the difference, if the difference is anything other than epsilon, Vout
  has to be infinity. I mean if K is very big, right? If K is very big, the only way
  the output could be some reasonable number like a Volt would be if the difference
  between Vplus and Vminus is very small.</p><p>OK, well let''s work backwards. Let''s
  start with the assumption that Vplus minus Vminus is very small. And that lets us
  solve the circuits very quickly. So for example, the same circuit that took, previously,
  a few lines to get the answer to, if I just take as a rule that Vplus has to be
  Vminus, it''s a one step. Vplus equals Vminus, OK, Vi equals Vo, period, done. It''s
  a very simple way to think about the answer to an op-amp circuit.</p><p>So if the
  op-amp can be represented by a voltage controlled voltage source and if K is very
  large, then Vplus is roughly Vminus. Shortcut, ideal op-amp assumption. So, use
  that or ignore it depending on what your mood is. And figure out the voltage relationship
  for this slightly more complicated circuit.</p><p>So what''s the answer? Yes? No.
  How many are done? How many are not done? OK, take a minute. This is supposed to
  be easy. Think ideal op-amp.</p><p>OK, what''s the output? Everybody raise your
  hand, what''s the output? More hands, more hands, more hands. OK, tiny number of
  hands, but those who showed hands are about 100% correct. I don''t know how to grade
  that. Small participation, 100% among those who did participate. So how do I think
  about this? What''s step (1)?</p><p>All right, according to the theory of lectures,
  what is step (1)?</p><p>AUDIENCE: Look at the previous slide.</p><p>PROFESSOR: Look
  at the previous slide, yes. What was the previous slide? OK The previous slide had
  to do with?</p><p>AUDIENCE: The ideal op-amps.</p><p>PROFESSOR: Ideal op-amps. What''s
  ideal op-amps say? Vplus equals Vminus. What happens here if Vplus is equal to Vminus?
  Well what''s Vplus?</p><p>AUDIENCE: 0.</p><p>PROFESSOR: So what''s Vminus?</p><p>AUDIENCE:
  0.</p><p>PROFESSOR: 0. So if Vminus is 0, what do I do now? That bad, that hard
  huh? Well, I got a [UNINTELLIGIBLE] here in which three different currents can flow.
  How big is the current that can come into this node? What''s the sum of all the
  currents that can come into that node?</p><p>Well one could come in this way. One
  could come in that way. One could come in that way. How much current flows in the
  minus lead of the op-amp?</p><p>AUDIENCE: 0.</p><p>AUDIENCE: 0.</p><p>PROFESSOR:
  None. No current goes into the minus. No current enters the op-amp through the minus
  lead. So it''s the sum of three currents. How big is this current? How big is the
  current that flows in that lead? V1 -- V1 over 1, right? Ohm''s Law. So this node
  is 0. That node is V1. The voltage across this resistor is V1 minus 0. The voltage
  across is V1. The current is V1 over R. R is 1.</p><p>So the current that flows
  in this leg is V1. How much current flows in this leg? How much current flows in
  this leg?</p><p>AUDIENCE: V0.</p><p>PROFESSOR: V0. The idea is that the total current
  that flows into this node is V1 plus V2 plus V0. Solve for V0. V0 is minus V1 minus
  V2. Right? Got it?</p><p>The idea was that this is really easy to solve if you use
  the ideal op-amp approximation. You can see that this is 0. Therefore, this is 0.
  So you have a single KCL equation. And the result is that this circuit looks like
  an inverting summer. It computes the sum of V1 and V2 and then takes the negative
  of that and presents that at the output.</p><p>What I''m trying to motivate is that
  there''s a whole different level of reasoning that you can do when you have this
  element, which is an op-amp. Here what we''ve done is we''ve made something that
  performs a numerical operation. It presents, at the output, the negative sum of
  the two inputs.</p><p>OK another problem. Determine R so that V0 is twice V1 minus
  V2.</p><p>So how should I choose R? Not very many hands. This is the perfect nano
  quiz practice, right? This looks like a perfect nano quiz question, right? Smile.
  So what''s the answer? OK we''re down to about half correct. This is harder.</p><p>Basically
  you do exactly the same thing, it''s just that it''s a little algebraically messier.
  So not surprisingly, the first idea is to think about the ideal op-amp. We''ll think
  about what was the voltage here, what was the voltage there, and then we''ll equate
  them.</p><p>What''s the voltage at the plus lead? Well that''s easy. That''s just
  a voltage divider here. Since no current flows in here, I can compute the voltage
  relative to this ground as R over (1 plus R). That''s showed here. Times V1.</p><p>This
  one''s a little bit trickier because I''ve got two sources, V2 and V0, each pumping
  current into this place. The way I thought about it was start with V2 and then add
  to it this component, which can be thought of as a voltage divider here. So how
  big is the voltage at Vminus? Well it''s V2 plus a voltage divider here, which is
  given by this. That''s a little tricky.</p><p>If you''re not comfortable with that
  step, you could also solve for that voltage using the node method. The node method
  will give you the same answer. The answer is that the voltage at the Vminus port
  is two thirds of V2 and one third of V0. That sort of looks right because the resistors
  are in a ratio of 2:1.</p><p>And then using the ideal op-amp assumption, we equate
  the two, do some more algebra, and we get some relationship and figure out that
  R is 2.</p><p>The point is that this is a relatively complicated circuit. You could
  have done it if I had asked you to do it with the voltage controlled voltage source
  model. But the algebra is already hard here with the ideal op-amp assumption, and
  with the voltage controlled voltage source it''s even harder. So the idea is that
  the ideal op-amp assumption, the idea that Vplus is equal to Vminus, makes the work
  of calculating these responses significantly easier. Everybody''s with the bottom
  line?</p><p>We started with the idea that when you add an element to a circuit,
  in general, adding an element changes voltages and currents throughout the circuit.
  We wanted a way to make the design more modular, a way of adding a component without
  changing everything else. We thought about this op-amp thing. The model for the
  op-amp was voltage controlled voltage source. We inferred this ideal op-amp model.</p><p>The
  ideal op-amp model was great for calculating the response. It has this one problem.
  It seems to say these circuits are identical. If I literally believe the ideal op-amp
  assumption that all the op-amp does is magically make the plus and minus terminals
  the same, I would conclude that this circuit where the input comes in the plus and
  the output wraps around to the minus generates precisely the same input-output relationship
  as this one, where the input comes in the minus and the output wraps around the
  plus.</p><p>The ideal op-amp assumption simply says for both of those, Vi equals
  Vo. So I would assume from the ideal op-amp model I get the result that these two
  circuits work exactly the same way. Somehow that sounds wrong. I''ve got this part,
  and I can wire it up the right way and it works. Or I can flip the two wires, and
  it still works. Conservation of badness doesn''t let that happen, right? If you
  do something bad, it should break.</p><p>The ideal op-amp assumption seems to lead
  to a bogus result. It seems to say these two are the same. So what I''d like to
  do is think about that for a moment. We want to be comfortable with the assumption
  that we make. The ideal op-amp assumption makes analysis really easy, but we''d
  like to understand exactly what we''re assuming.</p><p>This just doesn''t sound
  right. OK, so let''s back up. Let''s not do the ideal op-amp assumption. Let''s
  Instead say that we use the voltage controlled voltage source model. So what I''ve
  done here is substitute into the left circuit. So this circuit is shown here and
  the other over here. All I''ve done is connected the input either to the plus or
  to the minus port and wrapped the other one around.</p><p>But now I''m analyzing
  it using the voltage controlled voltage source model. And I''ve done the tedious
  algebra. And I don''t think there''s any mistakes in the tedious algebra. In one
  case I get K over (1 plus K), which for large K is about 1. In the other case I
  get minus K over (1 minus K), which for K large is about 1.</p><p>The ideal op-amp
  assumption says that it doesn''t matter. The voltage controlled voltage source model
  says it doesn''t matter. And Freeman thinks this doesn''t make any sense. So what''s
  going on here? What''s going on is that we''ve actually made an enormous leap in
  thinking about the op-amp even as a voltage controlled voltage source. The two models
  that we talked about, the voltage controlled voltage source and the ideal op-amp
  model, are great for calculating answers. They are not so good at providing a mechanism
  for how the op-amp is actually working.</p><p>Think about just the ideal op-amp
  assumption. It''s great to think, OK, the op-amp is going to do whatever magic is
  necessary to make these two leads the same. Well how does it do that? The thing
  about the ideal op-amp assumption is that it doesn''t tell you the mechanism by
  which that happens. What does the op-amp actually do in order to get Vplus equal
  to Vminus? What''s actually going on inside the op-amp?</p><p>The ideal op-amp assumption
  is very good for analysis and not very good with mechanism. What''s the mechanism?
  What''s the op-amp actually doing? What it''s really doing is moving charge around.
  8.02 -- charge. So if you''re going to have a change in voltage, there has to be
  motion of charge. And that''s what''s missing from the voltage controlled voltage
  model and from the ideal op-amp model.</p><p>How do you think about moving charge
  around? Well it''s the same as moving water around. Somehow, I think it''s all those
  years of playing with water when I was a little kid, I find my intuition about water
  is better than my intuition about charge. So let me start by thinking about the
  intuition for water.</p><p>The way a water tank works is if the flow in is different
  from the flow out, the height changes. That''s continuity. So if the water is conserved,
  if there''s not significant evaporation over the duration of this experiment, or
  if molecules of water do not spontaneously disappear or appear, under either of
  those two assumptions, then the change in the height is proportional to the difference
  between the rate at which it''s coming in and the rate at which it''s coming out.
  If the rate at which it''s going out is equal to the rate at which it''s going in,
  there''s no change in height. If it''s coming in faster, it''s going up. If it''s
  coming in slower, it''s going down. All easy, right?</p><p>Charge works the same
  way. The thing that accumulates charge in an electronic circuit is a capacitor.
  And there''s a direct analogy between thinking about the way the flux of water generates
  height and the way flux of charge generates volts. So we can think about the flux
  of charge, that''s current. If there''s a net flux, if there''s a bigger current
  into a capacitor then there is out, the voltage on that capacitor goes up. If there''s
  a smaller current in than goes out, the voltage on the capacitor goes down just
  like the height in a tank of water.</p><p>We can make a much more realistic model
  for the way an op-amp works by explicitly making a representation for how the charge
  flows. And that''s shown here. I''m going to take the voltage controlled voltage
  source model but explicitly make a representation for the output charging up. What''s
  the op-amp do? The op-amp senses the voltage at the input and the output and does
  something to change the voltage at the output.</p><p>The thing it does is if the
  positive voltage is greater than the negative voltage, it pumps charge into the
  output node. If the opposite occurs, it sucks charge out. Now it''s important, this
  is not an accurate depiction of what''s inside an op-amp. This is the model for
  an op-amp. I don''t want to lead any of you to think that this is literally what''s
  in an op-amp. This is not literally what''s in an op-amp.</p><p>Here is much more
  literally what''s in an op-amp. This is the schematic diagram of a 709 which is
  a Widlar circuit. It''s a complicated transistor circuit. It''s ingenious. This
  is how you build a circuit that has the remarkable property of the ideal op-amp
  circuit. It''s not perfectly obvious from here.</p><p>And even here this doesn''t
  give Widlar enough credit. Here''s what he really did. He designed masks to shield
  semiconductor materials so that you could turn them into transistors so that it
  would turn into an op-amp. We''re not going to worry about this. This is two levels
  of abstraction more complex than we''re going to worry about. We''re just going
  to say, I don''t know what''s in there, but this is the way it behaves. This is
  intended to be a behavioral model for how an op-amp works.</p><p>And in fact, that''s
  an important idea that we use circuits-- I use circuits on a daily basis not because
  I design semiconductor devices but because I work on biological issues. I actually
  study hearing. And we make circuit models for the way biological parts work. And
  that helps us to understand the way the biological part works.</p><p>For example,
  here is a model taken from 6.021, where we try to understand how a nerve propagates
  an action potential by making a circuit model. That''s the same thing we''re doing
  here. We''re making a circuit model for how the op-amp works. it''s not intended
  to be literally what''s inside the op-amp. It''s intended to be a model that let''s
  us think about the behavior of the op-amp. This lets us understand now why it''s
  different when you flip the wires.</p><p>Let''s start with the original configuration
  where I put the voltage in the plus lead, and I wrap the output back around to the
  minus lead. What''s going to happen? What''s the op-amp actually do? Imagine that
  things had been stable. This was 0. The output was 0. Everybody was happy.</p><p>And
  now all of a sudden the input voltages steps up. What happens? The input voltage
  steps up. The voltage source suddenly generates a huge positive voltage. And that
  starts to put current into the capacitor that represents the voltage at the output
  of the op-amp. So as a result of this voltage being higher than where it was, current
  is being dumped by the op-amp into this capacitor, and the output voltage starts
  to increase. That''s shown it red.</p><p>As the capacitor voltage gets bigger, as
  the output voltage increases, the difference between Vplus and Vminus gets smaller,
  and the rate at which charge is flowing into the capacitor slows. And in fact, as
  the voltage at the output gets very close to the voltage at the input, the rate
  of current into the capacitor goes to 0. And the output voltage stabilizes at the
  input voltage.</p><p>The same thing happens in reverse if I were to change input
  voltage and make it go negative. If the input voltage went negative, then K times
  Vplus minus Vminus would be a big negative number and it would suck current out.
  The voltage controlled voltage source would suck current out of the capacitor and
  make the voltage fall. The voltage would fall. The absolute difference between the
  plus and minus port would get smaller. The current flowing would become less. And
  it would again stabilize when the output is equal to the input.</p><p>Contrast that
  to what would happen if I put the input into the minus port. If I put the input
  into the minus port, and the input goes through a step, then the input going positive
  makes the voltage controlled voltage source generate a big negative voltage. It
  sucks current out. So the input went positive. And the output goes negative. It
  goes the wrong way. That''s bad.</p><p>So here, if I put the input into the minus
  lead, a positive transition of the input leads to the output going the wrong way.
  And as it goes the wrong way, the drive to make it go the wrong way gets bigger.
  It''s a runaway system. It''s positive feedback.</p><p>So the idea is that by supporting
  the input into the negative lead instead of into the positive lead, leads to a positive
  feedback situation in which a small change at the input makes the output go the
  wrong way, convinces the op-amp that things are getting worse, so it makes even
  more current, which makes it go even more the wrong way. And the same thing happens
  with the flip situation.</p><p>The idea then is that by thinking about the flow
  of current-- What''s the op-amp actually doing? The op-amp is actually sensing the
  difference between the voltage at the positive port and the minus port, and it''s
  sourcing current that changes the output voltage to go up or down. You need to wire
  the op-amp so that ultimately the output equals the input. Otherwise the ideal op-amp
  condition that Vplus equals Vminus will ever be attained. So the left one is what
  we would refer to as a stable feedback situation.</p><p>You can think about that
  as analogous to thinking about a ball in a valley. So we have a valley, and we have
  a ball. The ball''s going to roll down here eventually. It''s stable. Bop it a little
  bit to the right, it''ll roll back into the valley. Bop it a little to the left,
  it''ll roll back into the valley. That''s as opposed to, when we''ve wired up the
  wrong way, it''s like we have an unstable equilibrium. It''s as though we''re trying
  to put the ball there. Bop it a little to right, it runs away to the right. Bop
  it a little to the left, it runs away to the left. That''s unstable.</p><p>There
  is a metastability plane. If you actually balanced it exactly, exactly, exactly
  at the right place, it would stay there. That''s what the solution is telling you.
  That was the minus K over (1 minus K). The fact that the equations had a solution
  is correct, it''s just an unstable solution. The tiniest little disturbance will
  make it go awry.</p><p>The idea then is that the ideal op-amp assumption is fine.
  It''s a good thing to use. It doesn''t tell you about the mechanism. If you think
  a little bit more about the way the physics works, you have to wire the circuit
  up so that it has negative feedback in order to get a stable equilibrium. So if
  you understand that, and you just make sure that you''ve hooked it up so that it
  has negative feedback, then you can use the ideal op-amp assumption. Everything''s
  just fine.</p><p>And in the interest of time, I''m going to just skip over this
  because we''ve already talked about all of this. It''s just another example.</p><p>The
  last thing I want to mention is just that in order to work this magic, the op-amp
  has to get power from somewhere. And so that means that it''s not a three-terminal
  device. It''s not the kind of device I''ve been drawing so far that has got power
  pins too. The way the op-amp works is it takes power from those power pins to be
  able to force the output to a voltage that''ll make the input the Vplus equal to
  Vminus. That''s the mechanism by which it works.</p><p>And that''ll have important
  consequences when we build the robot head, because what it means is that we''re
  not going to be able to generate arbitrary voltages at the output of an op-amp.
  We''re going to be limited to generating voltages that are between the power rails.
  So if we were to supply plus and minus 10 Volts to the power pins, we would not
  be expecting to be able to generate 20 Volts at the output. So that''s an important
  implication when we do the design lab.</p><p>In summary, what we''ve done is we''ve
  showed how circuits can be a pain to make modular, because in principle, adding
  one component changes voltages and currents everywhere. But there''s a way using
  op-amps to have this buffering idea that lets us logically separate parts of circuits
  so the one can control the other. Have a good day. &nbsp;</p>'
type: course
uid: 91d15eafb8d5ed156d1a759c77d54fa9

---
None