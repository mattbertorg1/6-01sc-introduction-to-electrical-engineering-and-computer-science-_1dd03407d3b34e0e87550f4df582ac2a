---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: qGZy1CRoZdE
  parent_uid: 29d84b1f967478526263a18038d0daf8
  title: Video-YouTube-Stream
  type: Video
  uid: bb23805447bd6de91e4abe939f2cf270
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/recitation-9-circuits-representation/id490181666?i=108667952
  parent_uid: 29d84b1f967478526263a18038d0daf8
  title: Video-iTunes U-MP4
  type: Video
  uid: e911b5301d26fb5a38220b226883083f
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_rec9_300k.mp4
  parent_uid: 29d84b1f967478526263a18038d0daf8
  title: Video-Internet Archive-MP4
  type: Video
  uid: 92b63a124aa2559143043e86563cb394
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/qGZy1CRoZdE/default.jpg
  parent_uid: 29d84b1f967478526263a18038d0daf8
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 29814318358adc7e570fe9f88f510f6f
- id: MIT6_01SC_rec9_300k.srt
  parent_uid: 29d84b1f967478526263a18038d0daf8
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuits/recitation-1-object-oriented-programming/MIT6_01SC_rec9_300k.srt
  title: MIT6_01SC_rec9_300k.srt
  type: null
  uid: e93e9cbb016ae2902f2ba684734544ff
- id: Caption-OCW-SRT
  parent_uid: 29d84b1f967478526263a18038d0daf8
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: 0bc067c663a6a4ba59db58f0d20986d1
- id: MIT6_01SC_rec9_300k.pdf
  parent_uid: 29d84b1f967478526263a18038d0daf8
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuits/recitation-1-object-oriented-programming/MIT6_01SC_rec9_300k.pdf
  title: 'MIT 6.01SC S11 Recitation 9: Circuits: Representation, KVL, KCL Transcript'
  type: null
  uid: 168db08b11a5b1190091362ffd9e78d2
- id: Transcript-OCW-PDF
  parent_uid: 29d84b1f967478526263a18038d0daf8
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: 073de3b87033926f7d43be1a3d15bcfa
inline_embed_id: 7386792recitation9:circuits:representation,kvl,kcl36923802
layout: video
order_index: null
parent_uid: c1a11356f20d61ecdbf385a0ade29169
related_resources_text: ''
short_url: recitation-1-object-oriented-programming
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuits/recitation-1-object-oriented-programming
template_type: popup
title: 'Recitation 9: Circuits: Representation, KVL, KCL'
transcript: '<p>KENDRA PUGH: Hi. Today, I''d like to talk to you about circuits. Last
  time, we finished up the LTIs, and signals, and systems, where we learned how to
  both model existing systems and predict their long-term behavior. But we haven''t
  forayed into how to actually create systems in the physical world. We''ve created
  some amount of systems in software and made some brains for our robots. But if we
  want to make something in the physical world, then we probably have to come up with
  ways to model physical systems or use physical components. That starts our new model
  on circuits. Circuits are going to be our first foray into designing systems in
  the physical world, also designing systems using physical components.</p><p>It''s
  worth mentioning now that the information that you learn about circuits is good
  for more things than even circuits. You can use basic circuit diagrams and properties
  of circuits to model all sorts of kinds of systems, especially ones in the human
  body-- circulatory system, neurological system, different kinds of fluid flow, that
  kind of thing. In the next few videos, we''ll go over how to represent circuits,
  and also cover some of the basic methods by which people solve circuits. We''ll
  also introduce an element called an op-amp, and use that element in order to enable
  us to do things like modularity and abstraction from our circuits.</p><p>First,
  let''s talk about representation. In the general sense, when you come across a circuit
  diagram, you''re going to see-- at the very broad level-- a bunch of elements and
  a bunch of connections between the elements. Those things will form loops and nodes.</p><p>If
  you don''t actually specify the elements, then your circuit diagram actually looks
  a whole lot like a block diagram. And in fact, block diagrams and circuit diagrams
  are very closely related in part because block diagrams are used to model feedback
  systems, which frequently are implemented using circuits. In this course, we''re
  going to be focusing on independent sources and resistors as the two major kinds
  of elements that we''ll use in our circuits.</p><p>We''ll also use things like potentiometers,
  which are resistors that you can adjust, and op-amps. And we''ll look at op-amps
  specifically in a later video. But I have one drawn up here just so you recognize
  it when you see it written. Note that it looks a whole lot like the block diagram
  symbol for a gain. And that''s intentional, and we''ll cover that later.</p><p>But
  in the meantime, the other sources that we''re going to be using are independent
  current, and voltage sources. We''re going to use resistors to adjust the amount
  of voltage and current that we''re actually dealing with and then sample either
  the current or the voltage at a particular point in our circuit to get the desired
  values that we''re after. On a circuit diagram, when you''re interested in the voltage
  drop across a particular element, you''ll indicate it by putting a plus and minus
  sign. This also indicates the directionality of the voltage drop.</p><p>Likewise,
  when you''re interested in the current flowing through a particular element, you''ll
  usually see an indication of it by labeling the current i, and then maybe i with
  some sort of subscript, and an arrow indicating the direction of current flow through
  that element so that you avoid making sign errors with the person that might be
  reading or writing your diagram. A quick note here. This is the reason that electrical
  engineers use j to symbolize values in the complex plane. It''s because i is used
  in particular for values of current.</p><p>Let''s review Kirchhoff''s voltage laws
  and Kirchhoff''s current laws. You''ve probably covered this in 8.02, electricity
  and magnetism, or possibly in an AP physics class. But we''re going to go over it
  really fast right now.</p><p>Kirchhoff''s voltage law is that the voltage drop around
  a loop is equal to 0. Or if you take the voltage drop across a particular loop in
  your circuit, the sum of those voltage drop is going to be 0. Let''s demonstrate
  on this diagram. Or, I''ll demonstrate on this diagram.</p><p>Say the voltage drop
  across this element is equal to V, right? Doesn''t matter what it is. We''re going
  to stick with that. The voltage drop across these elements, if I were to move around
  this loop, is going to sum to 0. Note that if I''m tracing out my voltage drop across
  this loop, I''m actually moving through this voltage source in the direction opposite
  of its indicated potential. So when I move through this voltage source, I''m going
  to account for its value as negative V. As I work my way around the rest of the
  circuit, the voltage drop across these elements is going to sum to V.</p><p>This
  is true for all loops in my circuit. So any loop that includes V, the elements I
  encounter as a consequence of moving around that loop are going to have voltage
  drop equal and opposite to the value I get by moving through V in this direction.
  This loop counts, too, but it doesn''t include V. All this loop tells me is that
  the voltage drop across this element is equivalent to the voltage drop across this
  element. Or, the voltage drop in this direction across that element is equal to
  the voltage drop in this direction across this element. That''s Kirchhoff''s voltage
  law.</p><p>Kirchhoff''s current law is that the current flow into a particular node
  is equal to 0. Or, if you take all of the current flows in and out of a particular
  node and sum them, they should sum to 0. I''ve actually got the same set up here.
  I''m not going to use a current divider.</p><p>I''m interested in the current flowing
  over this element. It''s actually the same as the current flowing over this element
  because resistance doesn''t change current, resistors flowing through a resistor
  should not change the current. So this is still the same i. Here''s my node. The
  current flowing in this direction and in this direction, if I took the linear combination
  of these two currents, they would be equal in value to the current flowing into
  this node.</p><p>When I''m looking at the current flowing through a particular node,
  I pick a direction. It''s usually arbitrary. I pick a direction. It''s arbitrary
  which direction I pick. Typically, you pick currents flowing into the node as being
  positive. I sum up all the currents, and I set that equal to 0. So in this case--.
  Or-- pretty simple.</p><p>Let''s practice on this particular circuit. One thing
  to note is that when you''re solving circuits in the general sense, both when you
  want TA help and when you''re solving for a mid-term and want partial credit, you
  want to label all of your nodes, all of your elements, and all of the currents that
  you''re interested in solving. See, I''ve got my voltage drop across this resistor,
  this resistor, and this resistor labeled, as well as these currents, which I''ll
  also be solving for.</p><p>The first thing that I would do when approaching this
  problem is attempt to reduce this circuit to something that is a little bit simpler.
  The first thing that I''m going to do is try to figure out how to change these two
  resistors in parallel into a single resistor and still have an equivalent circuit.
  That''ll allow me to solve for I1. There will be 0 nodes in my system. I''ll just
  have one single loop. And the current through the system will just be V/R.</p><p>So
  if I''m just looking at these two resistors, I have resistors in parallel. In the
  general sense, the way to solve for resistors in parallel is to take the inverse
  of the sum of their inverses. When you only have two resistors, you can typically
  cheat by saying that this is equal to their product over their sum.</p><p>I''m going
  to redraw my current understanding of the circuit. The other stuff that I''ve saved
  myself is that because these resistors are in parallel, they''re a current divider.
  They take the current in and divide it two ways determined by the ratio between
  these two values. The thing I''m actually interested in expressing is that V2 and
  V3 are the same value. When you have a current divider, the voltage drop across
  all elements in the current divider are the same. So the value of V here is going
  to be both V2 and V3. 2R plus 6/5 R. I''m going to go with 16/5 R for now. I''ve
  solved for I.</p><p>At this point, I have a voltage divider, which means that the
  current flowing through this part of the system is going to be the same. But the
  voltage drop across this element versus this element is going to be proportional
  to the ratio between these two values. V1 is going to be the amount of the total
  resistance in this simple circuit that this resistor contributes over the entire
  resistance in the system. Or, 10/5 R over 16/5 R, which is 10/16 R, or 5/8 R. Or,
  it''s going to be 5/8 V.</p><p>Same thing happens with V2. Note that these two values
  should sum to V in order to maintain Kirchoff''s voltage law. We''ve also found
  V3. So the two things that we have to find are I2 and I3.</p><p>Here, I''ve just
  done Kirchoff''s current law for this node. Because I''m working with a current
  divider, I can break up the total current flowing into that node into the number
  of parts equal to the sum of these values and then distribute them. And then, that''s
  [? inappropriate ?] given that less resistance means more current. What do I mean
  by that?</p><p>Well, I mean that here my current is equal to 5/16 V over R. I2 is
  going to be equal to this value over the sum of these two values times I1. Likewise--.
  And just to simplify--.</p><p>That concludes my tutorial on circuits. Next time,
  we''ll talk about other ways we can solve this circuit, and then we''ll end up talking
  about op-amps. &nbsp;</p>'
type: course
uid: 29d84b1f967478526263a18038d0daf8

---
None