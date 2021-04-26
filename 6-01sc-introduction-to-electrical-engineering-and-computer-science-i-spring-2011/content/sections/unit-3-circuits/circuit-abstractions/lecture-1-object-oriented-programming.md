---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: FANl3evX0FQ
  parent_uid: 67eaeb1f5ad5390317013ce003fe7c4b
  title: Video-YouTube-Stream
  type: Video
  uid: e19f44e8b1560e1e29f3aafd14747102
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/lecture-9-circuit-abstractions/id490181666?i=109416116
  parent_uid: 67eaeb1f5ad5390317013ce003fe7c4b
  title: Video-iTunes U-MP4
  type: Video
  uid: 0a9bf724952dd8286329e7efde135417
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_S11_lec09_300k.mp4
  parent_uid: 67eaeb1f5ad5390317013ce003fe7c4b
  title: Video-Internet Archive-MP4
  type: Video
  uid: 88b2bacc6106caf765b3590e83124255
- id: Thumbnail-YouTube-JPG_1
  media_location: https://img.youtube.com/vi/FANl3evX0FQ/default.jpg
  parent_uid: 67eaeb1f5ad5390317013ce003fe7c4b
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: be9d1dae6dc606362a0819d111d6c13f
- id: 3Play-3PlayYouTubeid-SRT
  media_location: FANl3evX0FQ
  parent_uid: 67eaeb1f5ad5390317013ce003fe7c4b
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: 72b1f5557a78cd22fff0e6fd3da7366a
- id: FANl3evX0FQ.srt
  parent_uid: 67eaeb1f5ad5390317013ce003fe7c4b
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuit-abstractions/lecture-1-object-oriented-programming/FANl3evX0FQ.srt
  title: 3play caption file
  type: null
  uid: 8f335ecb40a7909b3982489ebc3402c5
- id: FANl3evX0FQ.pdf
  parent_uid: 67eaeb1f5ad5390317013ce003fe7c4b
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuit-abstractions/lecture-1-object-oriented-programming/FANl3evX0FQ.pdf
  title: 3play pdf file
  type: null
  uid: 93f3579d19470bfb8aa57f0c9cb4ae04
- id: Caption-3Play YouTube id-SRT
  parent_uid: 67eaeb1f5ad5390317013ce003fe7c4b
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: 5406e1f2c5347b4c0f5d798a96fc0189
- id: Transcript-3Play YouTube id-PDF
  parent_uid: 67eaeb1f5ad5390317013ce003fe7c4b
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: 0290ce8129869fb37e2456023733e6f5
inline_embed_id: 40301445lecture9:circuitabstractions30074907
layout: video
order_index: null
parent_uid: e019a65fac12802a35be220a70b2f839
related_resources_text: ''
short_url: lecture-1-object-oriented-programming
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuit-abstractions/lecture-1-object-oriented-programming
template_type: popup
title: 'Lecture 9: Circuit Abstractions'
transcript: '<p>MALE SPEAKER: The following content is provided under a Creative Commons
  License. Your support will help MIT OpenCourseWare continue to offer high quality
  educational resources for free. To make a donation or view additional materials
  from hundreds of MIT courses, visit MIT OpenCourseWare at ocw.mit.edu.</p><p>PROFESSOR:
  So today I want to finish up thinking about circuits. And the major topic for today
  is just one -- thinking about abstractions that we can use for thinking about circuits.
  The attractions are things that capitalize on linearity. And they include things
  like [UNINTELLIGIBLE] and superposition. OK so what I want to do is finish up thinking
  about circuits. And just to get you thinking about circuits, let''s think about
  where we are.</p><p>Last time we saw that one of the issues in thinking about circuit
  design, is the fact that every part, in principle, interacts with every other part.
  Which makes the design process harder than the design process was for things like
  linear systems, where we thought about boxes having inputs and outputs. In linear
  systems, when we thought about boxes having inputs and outputs, the output didn''t
  necessarily have any affect on the input, unless there was an explicit path feedback.</p><p>In
  circuits, there''s feedback always. There''s no way to avoid it. And in fact, that
  coupling can make thinking about the circuits very difficult. And we introduce that
  idea by just thinking about, even if you wanted to close a switch, you know a circuit,
  that''s logically the same as adding a new part. And when you do that, that''s going
  to change the currents and voltages everywhere. So that''s kind of a big thing--
  that''s kind of the thing that''s different about circuits from what we''ve been
  thinking about before.</p><p>Because that complicates design, we''d like some way
  of dealing with it. And the way we introduced, and the way that you used in the
  lab, so far, has been to use a buffer. We can use an op-amp to make a buffer. And
  a buffer has this nice isolation property. In this particular circuit, it has the
  property that it copies this voltage to the output, regardless of what''s at the
  output.</p><p>That means we could put a switch here, we could change the light bulb,
  we could do anything we wanted to, and we would still know, because of the properties
  of the op-amp, we would still know that this voltage is going to be 8 Volts, regardless
  of what we put there. So that''s very nice, that gives us a modularity, that gives
  us a way to design things. It let''s us design the left-- make a circuit that generates
  8 Volts without knowing precisely what''s going to be the ultimate circuit that
  that drives. So that''s nice, it allows us to do modularity.</p><p>And in many instances,
  that''s a very good solution. In fact in the solution-- in the problems that you
  are working on in lab, where you''re trying to drive a motor-- that''s an excellent
  solution. It''s not always an excellent solution. In some sense, it''s very expensive.
  An op-amp is a complicated part. If you were to look inside an op-amp, there''s
  some two dozen transistors in most op-amps. So it''s not an inexpensive part, especially
  when you think about this kind of a circuit that only has three parts to the left.</p><p>The
  op-amp is actually a more complex device than anything else up. So op-amps are wonderful,
  op-amps allow us to make buffers, buffers are wonderful, but they''re not always
  the best solution for thinking about modularity. And, in fact, there''s other ways.
  And so that''s what we want to think about today is -- other ways for achieving
  modularity in circuit design.</p><p>And the key to thinking about this, is to think
  about, well, what''s the worst thing that could happen? If I changed this part arbitrarily,
  just how bad can things get? So I''ll let you answer that. Think about that circuit,
  and assume that this is a 90 Volt power supply, 3 Ohm, 6 Ohm, but this can change--
  R0 can change. I''ve tabulated some values of R0 and putative, corresponding values
  for V0 and I0. Are my putative answers right?</p><p>So take a minute, talk to your
  neighbor, figure out how many of these-- let''s see-- ten blue numbers are right
  or wrong.</p><p>It''s very quiet, you are allowed to talk to people.</p><p>So how
  many of the numbers are wrong? So raise your hand, indicate by number fingers how
  many mistakes are in the table. More votes, more votes-- come on, come on. if you
  had talked more, you could blame it on your neighbor more easily, so talk quickly.</p><p>OK.
  So does everybody agree with their neighbor? OK, i don''t see a single right answer.
  So take 30 more seconds and think about it again. I don''t see any right answers.
  So assume your answer''s wrong.</p><p>[CHUCKLES]</p><p>Color blind-- OK, so how
  many of the voltages and currents are incorrect?</p><p>OK, how about a re-vote?
  So how many of the blue numbers-- the currents and voltages, how many of V0 and
  I0 -- how many of those are incorrect? OK, not very many votes-- I''d say about
  80% correct, now. That''s definitely an improvement. What would have to be true?
  If I wanted to prove that some of these numbers were wrong, what could I do? Give
  me a condition that would have to be true if the numbers were correct.</p><p>AUDIENCE:
  V0 has to equal I0?</p><p>PROFESSOR: V0 has to equal I0. We know that this resistor
  better be-- better obey Ohm''s Law. That''s what we mean by that symbol. So it had
  better be the case that V0 is I0R0. So you you''d want this number to be the product
  of that and that. So 0 is the product of 0 and 30, that looks good. 30 is 2 times
  15, 36 is 3 times 12, 48 is 6 times 8. 60 is-- well that''s a little marginal. how
  about if I rearrange it a little bit, and say what if R is V/I?</p><p>If I is 0,
  that would make the resistor infinity, so there''s a way of thinking about that
  last line as correct. That''s a little funny. Maybe the forward way of thinking
  about it is, well what if I made the resistor infinite? if I made the resistor infinite,
  what would be I? 0. And what would be V?</p><p>What would be the voltage difference
  if this were right, then? The voltage divider--</p><p>AUDIENCE: Oh, yeah.</p><p>PROFESSOR:
  So if there''s no current here, then you can use the voltage relationship-- the
  voltage-divider relationship here. 6 over (3 plus 6) times 90 -- which is 60. So
  if you use straightforward reasoning saying, what if the resistor was infinitely
  large? What would happen? Then you would conclude that the bottom line is OK. If
  you choose-- if you show that R equals V over I, are you done? What else has to
  be true in order for the numbers to be true? It''s not very hard.</p><p>AUDIENCE:
  The voltages drop out of the [UNINTELLIGIBLE]. The resistor has to be the same as
  the--</p><p>PROFESSOR: So the voltages-- that''s an instance-- what you just said--
  is an instance of KVL. Basically, the voltage around all of the loops better be
  0. The sum of the voltages around all of the loops better be 0, and the sum of the
  currents in all of those closed surfaces better be 0, right? KVL better be satisfied
  everywhere, and KCL better be satisfied everywhere.</p><p>So, in particular, we
  can ask about this node. We could say, do the currents flowing into that node sum
  to 0? So if you take a line here-- let''s take this line-- if V0 happened to be--
  V0 happens to be the voltage here, right? So if V0 were 36, then that puts some
  voltage on this leg. 36 would what, 54? So then you''d have to say-- you''d have
  to compute, then, the current through here and the current through there, and see
  if those currents sum to 0.</p><p>And, in fact, if you do those calculations, you
  if you can convince yourself of those are all true. So the answer was 0. All of
  those answers were true. The point of doing the exercise was to just remind you
  about how you solve circuits, but also to let us look at patterns. The interesting
  thing in this problem is the pattern the results between the V''s and the I''s.</p><p>So
  if I were to make a plot, in fact, those V''s and I''s all fall on a straight line.
  Well that''s pretty interesting. So if I plot just this V versus this I-- so V equals
  0, 30, 36, 0, 30, 36, 48, 60 -- and the corresponding I''s, 30,15,12,6,0 -- 30,15,12,6,0.
  Those points all fall on a straight line. That suggests that there''s some pattern
  here. And if there''s a pattern, then there might be a way to exploit it.</p><p>So
  that''s what I''m trying to develop-- is a way to exploit the pattern that results
  when parts of circuits interact. The interesting thing that we-- so not only is
  it true that there''s a simple pattern, but it turns out that the pattern is completely
  independent of the thing that I put on the right. The pattern is a property of the
  circuit to the left.</p><p>One way to convince yourself of that is to substitute--
  take that resistor out, and put in a voltage source, and redo the problem. This
  time, instead of assuming that there''s an Ohm''s Law-type resistor here, assume
  there''s a constant voltage, and that constant voltage is adjusted to 0,30,36,48,60.
  If you re-solve that problem, you get exactly these same currents. The answer continues
  to fall on exactly the same line.</p><p>So that''s a very interesting pattern. The
  idea is that when the circuit on the left interacts with the circuit on the right,
  regardless of what the circuit on the right is, you get a simple relationship between
  the voltage and current that comes out of the circuit on the left. So that motivates
  the idea that we can think about the left-hand circuit as some kind of a generic
  part. We call that generic part a one-port.</p><p>Think about this circuit on the
  left-- the thing that''s in the red box-- it''s got at its terminals-- the terminals
  are the things that poke through the red box. First off it has two terminals, two
  terminals is just like all of our other parts. And it''s like a resistor, it''s
  like a voltage source, it''s like a current source, it''s a two terminal device.
  And just like a voltage source or a resistor or a current source, there''s some
  voltage across those terminals, and there''s some current that flows in those terminals.</p><p>So
  there''s some current that goes in the plus. And that same current comes out the
  minus. That''ll be true for this circuit, just the same as it''s true for a resistor
  or voltage source or anything else, the only difference is, the thing that''s inside
  the box-- the thing that''s inside the one-port-- is more complicated than it was
  for a simple resistor or voltage source or current source. So what we can think
  about, is this whole red box just looks like a super part.</p><p>So the interesting
  thing that happens is, this red box behaves like a one-port, like a super part.
  And just like a resistor has a relationship between V and I, V equals IR, Or a voltage
  source has some kind of a constraint, V equals V0. Or a current source has some
  kind of a constraint, I equals I0. This funny part has a relationship between V
  and I that''s given by that curve.</p><p>In some sense, it''s not very different.
  So we think that-- so what we want to do now is figure out the rules that govern
  the currents and voltages that flow through one-ports. And in particular, how special
  was this straight line thing? I mean if they were always a straight line, that would
  be really easy, right? So the question-- so the next question I''d like to ask is,
  just how often are we expecting to see straight lines there?</p><p>I already said,
  the primitive elements that we think about-- Ohm''s Law, resistors, voltage sources,
  current sources-- they have straight line constraints between the voltages and currents
  that they can generate. So think about what I''m doing. I''m trying to think about
  a rule that''s going to let me describe the currents and voltages into that red
  box from the previous slide, much like I would describe the voltages and currents
  in an Ohm''s Law a resistor.</p><p>I can tell you the voltage-current relationship,
  V equals IR for an Ohm''s resistor, independent of what it''s connected to. That''s
  the reasoning that I''m using here. I''m going to try to figure out, independent
  of what it is connected to, what will be the voltage-current relationship for the
  red box? So the question is, when are we expecting straight lines, and when are
  we not expecting straight lines?</p><p>So here''s a simple circuit. Here''s a super
  part made out of one linear resistor, one Ohm''s Law resistor, and one voltage source.
  What''s the current-voltage relationship for that part? What if I put a red box
  around the whole thing, and asked you to draw the I-V curve, the current voltage
  curve? Which would it look like, A,B,C,D -- which should have been (1), (2), (3),
  (4) -- so you can raise fingers, or none of the above?</p><p>So take 30 seconds.
  Figure out what would be the I-V curve for this part.</p><p>So if you map A to D
  into (1) to (4) -- which of those plots describes the current-voltage relationship
  for that circuit? Map A to D to (1) to (4). OK, you''re quiet, and the success rate
  is smaller than usual, about 50% correct. Take 30 seconds, reconsider your answer,
  try to get this up to 85% or so.</p><p>[CHATTER]</p><p>So which is the best plot?
  Which plot best characterizes the circuit on the top? OK, that''s much better. That''s
  about 75%. Certainly not 100%, but better. OK so how do you think about this? One
  way to think about it is special cases. Can you think about any special cases that
  are particularly easy to check? 0 -- OK, what equals 0?</p><p>AUDIENCE: V or I --</p><p>PROFESSOR:
  V or I -- yes. So what if you were to make -- if you were to make I equal to 0?
  First off, if you made I equal to 0, what''s special in the plots? If I equals 0,
  then you round up x-axis. Sorry, if you make I 0, what will V be? If you made I
  be 0, how big will be V? 5 Volts, right? If you make I be 0, then there''s no voltage
  across the resistor. So the total voltage here will be the same as the voltage across
  the voltage source, V equals 5.</p><p>So the intersection on the x-axis should be
  at the point V equals 5. Makes sense? Now if you said V equals 0, how big would
  I be? If you set V equal to 0 -- how do you set V equal to 0?</p><p>AUDIENCE: Negative
  2.5.</p><p>PROFESSOR: Negative 2.5, so what is negative 2.5?</p><p>AUDIENCE: The
  value of I.</p><p>PROFESSOR: So do you need-- how do we set V equal to 0? What''s
  the circuit way of saying, set V equal to 0? You set V equals 0 in a circuit by--</p><p>AUDIENCE:
  Grounding.</p><p>PROFESSOR: --grounding, by setting it-- by putting in a wire. So
  you run a wire from here to here. Voltage across a wire is always 0, right? So you
  set something to 0 by putting a wire across it. We call that a short circuit. OK,
  there''s a short path for the voltage travel. So you put a short circuit here, and
  then I becomes V over R, and the only trick is that it''s up, right? Current likes
  to flow down the electrochemical gradient. So it likes to go down the electrical
  gradient. So the current is going to go up, but the reference direction for this
  I is down, so I is minus 2.5.</p><p>So the intersection on this axis is minus 2.5.
  So we know that it has to go through a negative on the bottom, and it has to go
  through a positive V on the x-axis, and the only curve that does that is (A). And
  if we wanted to be a little bit more fancy, we could figure out the general rule.
  We could just write an expression for Vr. Well by KVL, Vr is always the difference
  between V and 5 Volts.</p><p>And we could write an expression for the current through
  the resistor. That''s just V over R. Vr is V minus 5, R is 2. So I get some expression
  which is, lo and behold, linear in V. So just like that more complicated circuit
  that I''d looked at, I ended up with a straight line relationship in the current
  voltage-- the relationship between the current and voltage falls on a straight line.</p><p>So
  how special is that? Well it actually happens pretty robustly. Think about what
  would happen if I had two parts, the generically-- so I''m thinking about these
  being generic boxes, inside could be anything. There could be a current source,
  a voltage source, a linear resistor, or some other one-port. So if I had a generic
  box here, and a generic box here, and I connected them in parallel, under the condition
  that each of the generic boxes had a straight line current-voltage relationship,
  it''s easy to argue that the resulting relationship between current and voltage
  for the parallel combination is also a straight line.</p><p>All you need to do is
  realize that if you hook two things in parallel, the parallel voltage is the same
  as V1 and V2. So all the voltages are the same. And the currents add. So Ip, the
  current end of the parallel combination is the sum of the two I''s. So if you think
  about the relationship between V1 and I1, and the relationship between V2 and I2,
  you could derive the relationship between Ip and Vp by just adding.</p><p>V1 equals
  v2 equals Vp, that''s what we saw here. And the current at the bottom is the sum
  of the other two currents. So, in particular, if this was a straight line, and that
  was a straight line, the sum of two straight lines is a straight line, right? If
  you add two straight lines, you get a new straight line. So what this shows is that
  if you started with parts that were themselves straight lines, parallel combinations
  would generate a new part with another straight line.</p><p>Same sort of thing happens
  if the two parts we''re in series. In series we would have Iseries -- it''s the
  same as I1 equals I2-- so that''s the equivalent of the y-axes, where previously
  we had equivalents of the x-axes. And now if both of these boxes had linear I-V
  curves, I would now add horizontally rather than adding vertically. But I have the
  same result. If the two, individual one-ports had linear I-V curves, and if I add
  horizontally, I''ll get a new linear I-V curve.</p><p>And in fact, if you start--
  if you put any combination of parts that have linear I-V curves together to form
  a new circuit-- a new one-port, the I-V curve for that new one-port will be a linear
  function. And the way to see that, is to think about linear equations. Remember
  when we solve a circuit, we have to have one law for every element, Like Ohm''s
  Law-- it''s V equals IR, or voltage source is V equals V0 or something like that--
  we need one law for every element.</p><p>And then we have KVL and KCL. Well all
  of the-- if we start with the assumption that each component has a straight line
  relationship between voltage and current, which is true for linear resistors, voltage
  sources, and current sources. Those equations that describe those parts are what
  we call linear equations. Linear equation is an equation where the function of the
  unknowns is a quote -- linear function.</p><p>It has the form-- some constant times
  an unknown, plus some other constant times some other unknown, plus, in principle,
  any number of those. But it has to be a linear function, so you''re not allowed
  to have things like V-squared in there. But if you think about things like voltage
  sources and current sources and Ohm''s Law, they don''t have squares in there, they''re
  linear equations.</p><p>And the idea then, when we''re solving for the I-V relationship
  for this new one-port thing, all we''re doing is we''re solving a system of linear
  equation. Sort of in the abstract, the idea is that we write down all of the component
  equations inside the box, we write down all of the relevant KVL and KCL, and then
  we solve. So they''re all going to have-- each one of those equations is going to
  be linear, so it''s going to be something like, say, a0x0 if x is my unknown. ''x''
  could be a current or a voltage.</p><p>And then I might have sum of x1, then I might
  have sum of x2, and I might have a whole bunch of things, and they all add together
  to be some constant, like that. So that might represent part one-- that might represent
  one of the components in the box. Then I would have another component, which would
  be some other linear equation.</p><p>Then I''d have a KCL equation, well KCL is
  easy, because that only has currents in it, and the multipliers are all 1 or minus
  1. Right, so that''s clearly linear. And I have KVL equations. Those are linear.
  And the point is, that when you solve linear equations, you get a new linear equation.
  So think about solving this by the method of substitution. I could figure out what
  is x0 here.</p><p>If I use this equation to figure out x0. x0 would be a linear
  function of all the other x''s. So then if I plug that linear function into here,
  I replace this linear equation with a new linear equation with one fewer unknown.
  if I keep doing that, I just keep replacing linear equations with other linear equations.
  When I''m all done, I''m left with a new linear equation. That''s why, if you start
  with parts that linear I-V curves, you''ll end up with a straight line I-V curve.</p><p>So
  that idea that the I-V function is a straight line is quite robust. It will happen
  anytime you go to circuit out of ideal parts-- whereby ideal parts, I mean Ohm''s
  Law resistors, voltage sources, and current sources. So that has a very interesting
  circuit interpretation. If I know that an arbitrary circuit can be represented by
  a straight line-- if the I-V curve can be represented by a straight line-- well
  that generates an equivalent set.</p><p>There''s obviously more than one circuit
  that could generate the same straight line. Here''s a circuit that can generate
  that straight line. In fact, it will always be true that I can generate a circuit
  with one voltage source and one Ohm''s Law resistor that will mimic the behavior
  of any arbitrary combination of resistors, voltage sources, and current sources.
  All I need to do is think about, you take the complicated thing, figure out its
  straight line plot, now you read off some critical numbers from this plot.</p><p>You
  say, OK, well what if the current were 0? Well if the current were 0, I''d be on
  this axis. If the current were 0 in the circuit, V would be V0. So that means you
  look over here, you figure out the x-intercept, and the x-intercept is the value
  of the voltage source. Similarly, if you figure out the rate of growth of I -- so
  more generally, if you solve for I, I will be the difference between V and V0 divided
  by R, that''s just Ohm''s law for the resistor.</p><p>And that then lets you figure
  out the law for the slope. The slope over here is going to turn out to be one over
  this resistor-- I should have had-- this should be R0, these two should match. So
  the slope of this line is one over that resistor. So in general, regardless of how
  complicated the box is, figure out the straight line and I-V curves, read off the
  x-axis, read off the slope, and that lets you construct a simple circuit that has
  the same Vi curve. We call that circuit the Thevenin Equivalent.</p><p>What that
  means is, you can think about a complicated circuit, regardless of how many parts,
  by a circuit it just has two. That''s an abstraction that lets us think more simply
  about complicated circuits even if there''s no buffers. This is true always. OK,
  it''s not true-- it''s not it''s not the case that if I change the thing that I
  put here-- if I change the thing I put here, this relationship is still true. It''s
  the equivalent of Ohm''s Law for complicated circuits.</p><p>Ohm''s Law is what
  I get if what''s in the box is a single resistor. If what''s in the box is complicated,
  more generally this is what I get, the Thevenin Equivalent. Of course there''s lots
  of circuits that have this I-V curve. So a different one is a current source with
  a resistor. That''s called a Norton Equivalent. You do the same sort of thing. What
  would happen if here, if I set V to be 0? Well how do I make V be 0? I make V be
  0 -- Did I write that on the slide? no I didn''t write it on the slide. I make V
  be 0 by putting a short circuit here. I connect a wire.</p><p>If I put a wire here,
  then how big is the current I? Well if I put a wire here, it''s easier for this
  current to go through the wire than it is to go through that resistor. So all of
  this current goes through the wire. All of this current is I0. So if I put a short
  circuit across V -- if I make V be 0, how big is i? Minus I0 right? All the current
  I0 goes through, it just goes to backwards.</p><p>So that''s how I get this point.
  So if I wanted to replace some complicated circuit with a Norton Equivalent, I would
  take the complicated system, to figure out the I-V curve, read off the intercept
  on this axis, change the sign-- that''s the most confusing part, by the way. This
  is the error that you all make. There''s a minus sign in the current relationship.
  We like to draw-- it just makes us feel good to have the arrow go up.</p><p>And
  if you make the arrow go up, it''s in the wrong direction to I. So when we did the
  Thevenin equivalent, there was no sign from it, this was V0. So the voltage on the
  voltage source is equal to the x-intercept. But when we do the Norton, the current
  in the current source is minus the y-intercept. Same idea, though. OK? So the idea
  is that Thevenin and Norton equivalent circuits are equivalent, in the sense that
  they generate the same voltage. that the more complicated circuit did.</p><p>So
  that means for thinking about the circuit we can ignore the complicated stuff, and
  just know two numbers, V0 and R0, or I0 and R0. So one more step, what this all
  means is, that if you can represent the current voltage relationship for an arbitrary
  circuit in terms of a straight line, that means that when we''re trying to characterize
  an arbitrary circuit, it doesn''t matter how complicated it is. It could have 100
  parts in it.</p><p>Regardless of how complicated it is, I only need to measure two
  things in order to fully characterize it. If a circuit is made out of linear resistors,
  voltage sources, and current sources, three special linear parts-- if a circuit
  is composed entirely out of linear parts, doesn''t matter how many parts are in
  it, there could 100, there could be 1,000-- I only need to measure two things to
  get a complete description. And that''s because two points determine a straight
  line.</p><p>I know, by having proved it by using linear algebra, I know by using
  linear algebra that the solution is a straight line. I know from geometry that two
  points determine a straight line. I only need to find out two points. So by convention,
  the easiest two points is usually the simplest cases. Set the voltage to 0 and set
  the current to be 0. So that motivates the idea that if I have an arbitrary circuit,
  if I want to figure out this reduced complexity abstraction-- say I want to make
  a Thevenin Equivalent-- what I would do is first to ask the question, how big is
  the open circuit voltage?</p><p>Open circuit means there''s no connection between
  the terminals. That means the current is 0. If the current is 0, I''m on the x-axis.
  So over here I''m on the x-axis, so I''m thinking about the red point. Open circuit
  over here means there''s no connection here, which means the current is 0, and all
  I need to ask is-- regardless of how complicated it is the circuit-- how big is
  the voltage that I would measure here?</p><p>So in this circuit, if I have a-- yeah,
  I confused myself for a moment. if this current is 0, then this voltage drop is
  0. This voltage source prescribes the voltage between these nodes to be 1 Volt,
  so V0 is 1 Volt. So I just fell one point. I set I to be 0, I found the open circuit
  voltage. Then I need to find one other point, because I only  to find two. So I''ll
  find the short circuit current.</p><p>Imagine that I put a wire between the input
  and the output, and I''ll compute how much current that circuit generates in that
  wire. Again the only confusing part is that the reference directions are backwards
  to the way you might have expected them to be. If I put a short circuit here, then
  the voltage between these nodes is still 1 Volt. That''s what the voltage source
  always says.</p><p>So the current that flows through this wire, the short circuit
  current, is just this V over that R, except it''s in the negative direction. And
  the way you can think about that is that the slope of this curve has to be positive.
  I need-- because of the way Ohm''s Law works-- increasing the voltage better tends
  to increase the current, because that''s what Ohm''s Law resistors do. So I need
  to have this slope be positive if it''s going to be Ohm''s Law.</p><p>So I characterize
  just those two points, and then the resistance is simply the ratio of the two. So
  the resistance is related to the slope. It''s 1 over the slope, you don''t need
  to worry about that. The resistance is always V over I, so you just take the open
  circuit voltage and divide by the short circuit current, minus sign, and you get
  that the resistor must be 2 Ohms. Is that all clear?</p><p>The idea is that we''re
  trying to build an abstraction that lets us simplify the way we think about circuits,
  without introducing buffers. So that means then that these two circuits are equivalent
  to that circuit, in the sense that they all share the same I-V curve. If you substituted
  one server for the other, you couldn''t tell from outside the red box which was
  on the inside of the red box.</p><p>OK so I''ll do an example now. Think about,
  what if I want to find the equivalent-- the Thevenin equivalent for this circuit.
  I just do the things I just told you to do. First thing I think about is, what''s
  the open circuit voltage? So If I think about open circuit, there''s no connection
  here. That means this current is 0. That means that the voltage that develops is
  the voltage divider. So I get 7 and a 1/2 volts-- 3 over (1 plus 3) times 10, right.</p><p>So
  that gives me one point-- that tells me the voltage source for the Thevenin equivalent.
  Then for the second point, I want to think about the short circuit current. So I
  consider putting a wire here, and then I compute the amount of current that flows
  in that wire. And in this circuit, this wire shorts out that resistor, so all the
  current goes through this wire, and none of the current goes through that resistor.</p><p>So
  that means that the total current that flows is 10 Volts divided by 1 Ohm, which
  is 10 Amps. And then I know that the equivalent resistance is the ratio of the open
  circuit voltage to the short circuit current, except I have to worry about the minus
  sign. And so I end up with the equivalent resistance being the 7.5 Volts, which
  is the open circuit voltage, divided by 10 Amps, so I get 7.5 Ohms.</p><p>And so
  the answer then, is that here is the circuit I started with, here''s the Thevenin
  equivalent circuit, they''re identical in the sense that they have the same I-V
  curve. And you can just sort of see why that has to be true. If you think about,
  here''s the two circuits, and if you think about the simple cases, if you set I
  to be 0, the voltages better be the same. Well over here it''s 7.5 by the voltage
  divider, over here it''s 7.5 by the fact that there''s no current going through
  that resistor.</p><p>And the short circuit current better be the same. So over here,
  if you short this out, you''re going to get 10 Amps, over here if you short it out,
  you''re going to get 10 Amps. So you can always go back and forth. The point is,
  that you can substitute the simpler circuit for the more complex circuit, because
  they have the same I-V curve. OK, just to make sure that you''re following me, here''s
  a question that has to do with taking the same circuit, but considering the Thevenin
  equivalent-- Thevenin or Norton equivalent-- at three different ports.</p><p>Here
  I''m thinking about what would happen if I looked in terminal A, what if I looked
  in terminal B, or looked in terminal C? Figure out the Thevenin and Norton parameters,
  and see if there''s an error in the table.</p><p>So how many errors are in the table?
  About 50% correct again. So which entry don''t you like.</p><p>AUDIENCE: 2D?</p><p>PROFESSOR:
  That''s exactly right, so 2D is wrong. How do I figure out 1A? How do I figure out
  V0 for the a circuit? So the definition of V0 is the open circuit voltage. So I
  need to figure out, for the a circuit, how big would be the voltage across A if
  there was no current flowing in the leg of A. Everybody clear on that? So the thing
  that I would do is, I would think about, there''s no connection here. What''s the
  voltage here? So how would I calculate that? Yeah.</p><p>AUDIENCE: You would use
  the current-divider relationship to figure out that current flowing through that
  is going to be 4 Amps.</p><p>PROFESSOR: Precisely, so first I need to take-- here
  are the current sources, so I have two resistor lengths, so that''s a perfect set
  up for the current divider. So the amount of current that goes in this leg compared
  to that leg is the ratio of this resistance to the sum of resistances, right? And
  if you work that out, you''re going to get 4 Amps coming through here. So then after
  you know the current through this leg, it''s an easy matter to take the current
  and turn it into a voltage, so the voltage at the a port is 4 Amps times 5 Ohms
  is 20 Volts. Is that clear?</p><p>And similarly, but with a different answer, the
  voltage at the B terminal is the same 4 Amps, but now times 10 Ohms. So that''s
  how we got 40. And at C, it''s the same 4 Amps, but now it''s times the sum, 4 times
  15 is 60. Everybody''s happy about that? So the point is that when you generate
  an equivalent circuit, it depends upon which set of terminals you''re using. You
  can''t just take a circuit and say, give me the Thevenin Equivalent.</p><p>You have
  to say, give me the Thevenin equivalent looking somewhere. So I could look in the
  A port, the B port, or the C port, and I get different V0''s. How would I compute
  the I0? Short circuit current-- so what I would do is I would short this out. When
  I do that, all the current flows in this leg and one of the current flows that leg.
  So that means I have, equivalently, 10 Ohms in parallel with 10 Ohms. Then by the
  current divider, how much current goes down one leg?</p><p>Half of it. I get a different
  answer over here, because now I short out that node, which shorts out that resistor,
  so now I get a different ratio of resistors. It''s not the same as the first, so
  I know that this answer can''t be 5. And, in fact, if you work it out, the answer
  is 20 over 3. And finally, if you short here, then you know that that short circuit
  shorts out both this series combination and that one.</p><p>So all of the 10 Amps
  goes through that, so you get that 10 Amps. Then how do you get R0, which is the
  ratio of V0 over I0. So if you take V0 over I0, you get 4. Here if you do right
  answer, you get 6, and here if you do that you get 6. The point is, that the Thevenin
  equivalent you get is different. The Norton equivalent that you get is different,
  depending on which ports you''re looking at.</p><p>OK there''s two reasons for thinking
  about this. One-- so why am I thinking about all of these equivalent circuits? So
  I wanted to have an abstraction that was useful for thinking about how parts interact.
  I wanted a way of thinking about what would happen if I changed the load on the
  circuit without having to recalculate all the voltages and currents throughout the
  circuit. And so this Thevenin and Norton idea is a way of doing that.</p><p>That''s
  important from a practical sense, because when you buy a part-- when you buy an
  electronic part, they tell you how it works by telling you the Thevenin equivalent
  or the Norton equivalent, or whatever is the easy way to think about it. So there''s
  a practical reason-- when you buy an op-amp, they tell you how good the op-amp is
  by telling you how big is the equivalent resistance at the output.</p><p>So it has
  a practical value, because it lets you-- it''s the way you specify an electronic
  part. You can''t -- when the manufacturer makes a part, they can''t know what you''re
  going to do with it. So they tell you how it works by telling you something about
  the equivalent circuit. There''s also a different reason for thinking about this,
  and that is because it''s conceptually simplifying to think about Thevenin and Norton
  equivalents.</p><p>So here''s an example that''s very much like the first problem
  that I worked out. What would be the effect of closing this switch on the current
  I? We solved the problem very much like this last time, and one way you can solve
  it is you figure out I in two cases, when the switch is open and when the switch
  is closed. And you figure out whether went up or down, and you know the answer.</p><p>The
  point is, that if you think about this in terms of equivalent circuits, it''s completely
  trivial. If I think about what would happen-- I''m interested in what happens at
  I, what I do is split the circuit into two pieces, the stuff to the left of I, and
  the stuff to the right to of I. I make a Thevenin equivalent for both of them, and
  then I jam together the two Thevenin equivalents. What I get, in detail, is showed
  here.</p><p>So if I look left, I see a 20 Volt source with a 4, 4, and a 2. That
  has a Thevenin equivalent that is showed here, which is independent of the state
  of the switch. So the same Thevenin occurs on the two sides, switch open, or switch
  closed. If i make a Thevenin over here, there''s no sources. So it''s just going
  to be a resistance. So when the switch is open, I have to 2 Ohms, when the switch
  is closed, I have 1 Ohm.</p><p>I don''t even need to figure out what are these part
  values to see that, if I make this resistance smaller, which happens if I close
  the switch, the current goes up. I mean it''s true that I showed here that the Thevenin
  voltage is 10 and the Thevenin resistor is 4. I don''t even care. Regardless of
  what the Thevenin voltage was, regardless of what the Thevenin current is, it''s
  going to be the same when the switch is open and closed. And that''s a powerful
  statement.</p><p>I know it''s the same, so when I close this which, all I''ve really
  done is I''ve made that resistor smaller. The net series resistance is down, the
  current is up. So I have two reasons for thinking about Thevenin and Norton equivalence.
  One is practical value, the other is conceptual simplicity. It lets you simplify
  way you think about a circuit, and it''s a way of gaining intuition without ever
  even solving the equations.</p><p>Most circuit designers don''t solve certain equations.
  They know what it''s going to do just by looking at it, and this is the kind of
  reasoning that they use. OK, there''s one more topic-- the idea of Thevenins and
  Nortons really derived from linear algebra. The basic parts of most interest are
  linear. And when you put together a system out of linear parts, you get a linear
  system.</p><p>There''s one more consequence of linearity that is terribly useful,
  and that''s the idea of super position. If you have a system of equations that is
  linear, and if you have multiple sources, things are very simple. You can see that
  over here. If I had multiple sources, the system of equations that I get wouldn''t
  look quite like this. These terms, the constant terms, they''re the ones that come
  from the drives, the voltage sources, the current sources.</p><p>So if I had two
  drives, I would get something else here. I would get plus a at N+1 for example--
  source one, source two. And I would get source one, source two. So the idea is that,
  if I have a system that has multiple sources, I know from the structure of the linear
  equations, there is just more constant terms. OK, well what''s that mean? That means
  you can just use linear algebra to see that the answer to this problem is the sum
  of the answers to that problem plus the answers to that problem.</p><p>That''s just
  linear algebra. What that means in terms of circuits is, I can figure out the response
  to a circuit by turning on the sources one at a time. That''s called superposition.
  And generally speaking, it''s a lot easier than solving the circuit out the long
  way. So here I''ve got two sources So say I wanted to compute I, in response to
  V0 and I0.</p><p>What I would do, is I would turn off the I0 source, and calculate
  the voltage that results just from the voltage source. That''s the same as setting
  this to 0 and finding the response to this. So if I want to set I to 0, the way
  you set I to be 0 is open circuit. If you open circuit something, there''s no current
  going to flow through it. So I replace the current source with an open circuit,
  and compute the i that would be result when the current source isn''t there. OK,
  well that''s easy.</p><p>If their current source we''re not there, this would be
  open circuit. The current, i, would just be the total voltage going through R1 and
  R2. So the answer, I1, the first component of the current I, would be V0, the result
  of the voltage source divided by the sum of R1 and R2. Now that''s not the whole
  answer. That would be the whole answer if I0 weren''t there.</p><p>So now I have
  to worry about the other case. What if only I0 were there? Well now I have to set
  V to be 0. Well setting V to 0 is not open circuiting it. You can''t just reach
  in, grab the voltage source, and throw it away, because that''ll make the current
  0. If I want the voltage to be 0, I have to short circuit it. So what I do then,
  is I leave the current source alone, and I replace the voltage source with a short
  circuit, guaranteeing that V is 0. Then I ask, how big is I2, the component of I
  that results from the current source?</p><p>Well if I''ve short circuited this,
  then I just get a current divider. This current has to do with how readily the current
  divides between R1 and R2. The amount that goes through the R1 side is in proportion
  to R2 make R2 bigger, more of it goes through R1. Standard current divider, except
  for the slippery minus sign. So if I only had the current source, the current I2
  would have been current divider operating I0 with the slippery minus sign.</p><p>So
  that means, by superposition, that the result of having both sources on is just
  the sum of those answers. That''s a very big simplification. If you''ve got multiple
  sources in the circuit, you can think about them all at once. And if you really
  good at writing linear equations and solving them with pencils, you''ll get the
  right answer. But there''s an enormous simplification if you just turn off all but
  one, and do them one at a time.</p><p>So here''s a problem. Here''s a very simple
  circuit, compute V by using super position. V is the voltage across the resistor.
  How big would V be if you used the idea of super position?</p><p>So what''s the
  answer? 50% correct, roughly speaking. OK I want to use superposition. So how big
  would the voltage v be, if all I had was the voltage source? One. How big would
  the voltage be if i only had the current source? Ah, got half of you. That explains
  the 50% correct. How big would the voltage be, if I only had the current source?
  It''s tempting to say (1). I say tempting, because that''s the wrong answer.</p><p>[LAUGHTER]</p><p>What
  is wrong about the answer (1)? What does the voltage do to the current source? The
  voltage due to the current source is the voltage that the current source would have
  generated if the voltage source weren''t there. If the voltage source weren''t there,
  then-- half of you got it right, so half of you can shout the answer. So if the
  voltage source weren''t there, the voltage source would be 0.</p><p>If the voltage
  source were 0, then V would be 0. So if the voltage due to the voltage source is
  1, the voltage due to the current source is 0. The sum of the two is 1. The answer
  is 1. OK? Make sense? So, very closely related problem. What''s the current I? Solve
  that by superposition.</p><p>So how big is the current I according to superposition?
  Wonderful, so how big is the current i generated by the voltage source? 1. How big
  is the I generated by the current source? Negative 1, the sum is 0. All right, so
  those two problems were trivial by superposition. They''re not too hard by non-superposition.
  But the point is, that they''re trivial by super position.</p><p>So what we saw
  today-- the goal for today was to generate some abstractions that let you think
  about the way parts interact with each other, because that''s a central issue when
  you''re thinking about circuit design And we built the idea of Thevenins and Nortons
  and super positions. That was the basic idea. And the sub-theme-- or maybe I should
  say the major theme is really that.</p><p>It''s the importance of linear algebra.
  So the take home message is probably, take 18.06. So this was all about the application
  of 18.06 to the solving of circuits. See you later. &nbsp;</p>'
type: course
uid: 67eaeb1f5ad5390317013ce003fe7c4b

---
None