---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: rOA1VC5aQ7Q
  parent_uid: c0036fe0bb52d07c7c852a48884de6fc
  title: Video-YouTube-Stream
  type: Video
  uid: 36cb57f3facb9c2fbf45800171dbed29
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/recitation-12-thevenin-norton/id490181666?i=108667922
  parent_uid: c0036fe0bb52d07c7c852a48884de6fc
  title: Video-iTunes U-MP4
  type: Video
  uid: 96a5fba01e8d35fceb37522b8d0873cc
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_rec12_300k.mp4
  parent_uid: c0036fe0bb52d07c7c852a48884de6fc
  title: Video-Internet Archive-MP4
  type: Video
  uid: 6c063a4b73679cd7fba57c02127cb018
- id: Thumbnail-YouTube-JPG_1
  media_location: https://img.youtube.com/vi/rOA1VC5aQ7Q/default.jpg
  parent_uid: c0036fe0bb52d07c7c852a48884de6fc
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: c8654edfee9c5d1355922d18226d72f7
- id: MIT6_01SC_rec12_300k.srt
  parent_uid: c0036fe0bb52d07c7c852a48884de6fc
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuit-abstractions/recitation-1-object-oriented-programming/MIT6_01SC_rec12_300k.srt
  title: MIT6_01SC_rec12_300k.srt
  type: null
  uid: 60013079727e5e31cbee23ce0fb72315
- id: Caption-OCW-SRT
  parent_uid: c0036fe0bb52d07c7c852a48884de6fc
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: 0f341ffe284e71efc6aa98f7693148c7
- id: MIT6_01SC_rec12_300k.pdf
  parent_uid: c0036fe0bb52d07c7c852a48884de6fc
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuit-abstractions/recitation-1-object-oriented-programming/MIT6_01SC_rec12_300k.pdf
  title: 'MIT 6.01SC S11 Recitation 12: Thevenin/Norton Equivalence and Superposition
    Transcript'
  type: null
  uid: 191bc3ad538419e74f389a5c6ae0bc70
- id: Transcript-OCW-PDF
  parent_uid: c0036fe0bb52d07c7c852a48884de6fc
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: 6c0f5710c1da1fbdc994a13d9be0acf5
inline_embed_id: 52010640recitation12:thevenin/nortonequivalenceandsuperposition19494090
layout: video
order_index: null
parent_uid: e019a65fac12802a35be220a70b2f839
related_resources_text: ''
short_url: recitation-1-object-oriented-programming
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuit-abstractions/recitation-1-object-oriented-programming
template_type: popup
title: 'Recitation 12: Thevenin/Norton Equivalence and Superposition'
transcript: '<p>PROFESSOR: Last time we talked about op-amps and the fact that they
  allowed us to abstract away certain components of a circuit and sample particular
  voltages from a circuit and then modify those voltages as we would like in an LTI
  fashion. Today I''d like to talk to you about some other interesting things that
  fall out of the fact that we''re only dealing with LTI systems. In particular, Thevenin/Norton
  equivalence and superposition.</p><p>Thevenin/Norton equivalence is the idea that
  if you have a very complex circuit, but it''s still a LTI circuit, you can express
  it using a linear curve. And superposition is the idea that because you''re also
  dealing with LTI components, if you''re trying to solve a circuit, you can take
  the individual contributions of independent sources to that circuit and sum them
  in order to find out either the total current flowing through a particular component
  or the total voltage drop across a particular component. At this point, I''ll walk
  you through both.</p><p>Thevenin/Norton equivalence is an important concept in that
  you may have a very complicated circuit. And you don''t really want to talk about
  the entire complicated circuit. You just want to sample the voltage drop or current
  in a very particular location.</p><p>Because we''re dealing with LTI systems we
  can actually express that particular sample as its relationship between I and V
  and possibly whatever resistive component is associated with the voltage drop across
  that sample. We can solve for this curve by looking at the location that were sampling
  and finding the open circuit voltage associated with that position. Or if we were
  to leave the two terminals from where we are sampling open, what is the voltage
  drop across that section of our circuit?</p><p>That''s the point right here, where
  the current flowing through the system is 0. And there''s a given voltage associated
  with it. Likewise if we want to find the other intercept, we can close those two
  terminals by running a wire across them and then look at the current that flows
  across that wire. That''s the close circuit current.</p><p>The slope is going to
  tell us about our resistance, if any. If we''re only dealing with a voltage source
  or a current source, then we''re only going to be dealing with a straight line.</p><p>Once
  we''ve solved for these values, we tend to express them either as a Thevenin equivalent
  circuit or a Norton equivalent circuit. And you can convert between the two. Let''s
  walk through an example.</p><p>Here I''ve got a simple circuit. And I would like
  to find the Thevenin equivalent of that circuit, given that I''m sampling from above
  this resistor and below this resistor. The first thing that I''m going to do is
  find the open circuit voltage. Or if I were sampling from this point to this point,
  what is the voltage drop across this section of the circuit?</p><p>Well, I''ve got
  36 Volts. There''s 12 Ohms of resistance in the section that I''m sampling. And
  there''s 6 Ohms of resistance outside the section that I''m sampling. So 2/3 of
  my total voltage drop across this voltage divider is going to be accounted for inside
  my Thevenin equivalent circuit. So my Thevenin equivalent voltage is 24 Volts.</p><p>Now
  I want to go after the short circuit current. If I were to draw a wire from this
  terminal to this terminal, I''m curious what this value would be. As a consequence
  of connecting these two terminals, these resistors are going to be completely bypassed.
  We don''t actually have to drop any voltage or put any current through these resistors
  because there''s actually an infinitely easier way for the current to go.</p><p>In
  this case, we''re just going to follow Ohm''s law. 36 divided by 6 is 6 Amperes.
  But because of the directionality on this short circuit current, current in this
  system is going to flow in this direction. So are short circuit current is actually
  negative 6 Amperes.</p><p>That just leaves Rth. Once again we''re going to rely
  on Ohm''s law. If we divide our voltage by our current-- you can''t have a negative
  resistance. We''re actually going to divide by the negative of this. We''ll get
  out 4 Ohms.</p><p>Let''s do it again, this time with a slightly different sample
  point and find the Norton equivalent of our circuit. So if I''m only sampling across
  the 9 Ohm resistor-- I personally still solve for the Thevenin equivalent voltage
  first because I think it''s easiest. I''ll just make note of it over here.</p><p>The
  voltage drop across this resistor is determined by the fact that this is a simple
  voltage divider. The other resistors in this circuit-- 7, 2, 9 Ohms. So the voltage
  drop across this resistor is going to represent half of the total voltage in our
  circuit. That''s 18 Volts.</p><p>The short circuit current associated with connecting
  these two terminals is 36 Volts divided by the sum of these two resistors. Once
  again we''re going to end up bypassing this resistor entirely because, think about
  it this way, if there was a resistor across here with 0 resistance, all the current
  would sink through it, or it would represent the location for which infinite current
  would flow.</p><p>36 divided by 9 is 4. And because we''re following in the opposite
  direction we''re going to say this is negative 4 Amperes. In this orientation, the
  Norton equivalent amperage is actually the negative of this value. You sometimes
  see the arrow pointing downwards.</p><p>This preserves our property of short circuit
  current. If this was short circuited, Isc would still be negative 4 Amperes. And
  our Vth-- if our Vth was the voltage drop across these two points-- ha, I haven''t
  solved for Rth yet.</p><p>There are a few ways to do this. But I''m going to use
  Vth and In. 18 over 4, we can reduce it to 9 over 2. And if I were to solve back
  out for the voltage drop across this resistor just as a consequence of I Norton,
  I would get 18 Volts, which is also the Thevenin equivalent voltage for this circuit.</p><p>That
  covers Thevenin/Norton equivalence. And we''re going to talk about superposition
  really quickly.</p><p>Superposition is yet another circuit-solving strategy. It
  falls out as a consequence of only working with LTI components. And it means that
  in order to solve for a given component current or component voltage, you can actually
  find it by taking the linear combination of every contribution as a consequence
  of independent sources. What do I mean when I say that?</p><p>Well, if you have
  a circuit like this-- and you might recognize it from the NVCC lecture earlier--
  you can actually express it as a linear combination of just the voltage source and
  just the current source. Note what when I remove the current source, I end up with
  no connection because if you have 0 current flowing through a system, it''s the
  same as if the connection has been removed. Note that when I remove the voltage
  source, I no longer have a voltage drop across that connection, but I maintain the
  connection.</p><p>If in this example I was just looking for I1. I1 would be the
  linear combination of the contribution of I1 in this particular circuit plus I1
  in this particular circuit. So this is the expression that I''m looking for. In
  the first circuit, I''m just going to use V over IR -- or V equals IR -- and I''m
  going to have 3 Amperes in this direction.</p><p>In this circuit I''m actually going
  to have to use a current divider. Identify that I have five parts total to distribute
  among these two branches. Identify that this side is going to get the inverse of
  this side''s contribution to the total parts, or this side is going to get the proportion
  of parts equivalent to this side''s contribution. And vice versa.</p><p>That this
  side is the side that I''m interested in. And so 2/5 of the total current flowing
  through this current divider is going to end up in this branch. 2/5 of 10 is 4.
  It''s in the opposite direction of this current flow. So I''m actually going to
  contribute negative 4 Amperes from this subcircuit.</p><p>This should match the
  results from the NVCC lecture. That''s my super fast coverage of superposition and
  also Thevenin/Norton equivalence. Next time we''re going to start a whole new module.
  &nbsp;</p>'
type: course
uid: c0036fe0bb52d07c7c852a48884de6fc

---
None