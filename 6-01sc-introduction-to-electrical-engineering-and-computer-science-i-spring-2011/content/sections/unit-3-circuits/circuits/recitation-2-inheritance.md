---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: dAZ-i9MsbRM
  parent_uid: 45306826826d0ac5b06dbe85b0b4d85f
  title: Video-YouTube-Stream
  type: Video
  uid: 55a9201f66be3f6cb5b8b32a2f082f48
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/recitation-10-circuits-nvcc/id490181666?i=108667951
  parent_uid: 45306826826d0ac5b06dbe85b0b4d85f
  title: Video-iTunes U-MP4
  type: Video
  uid: 26155ff6f919db6567bcc5355157b2cd
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_rec10_300k.mp4
  parent_uid: 45306826826d0ac5b06dbe85b0b4d85f
  title: Video-Internet Archive-MP4
  type: Video
  uid: 98ac3077520c693c5afff89877fd0cad
- id: Thumbnail-YouTube-JPG_1
  media_location: https://img.youtube.com/vi/dAZ-i9MsbRM/default.jpg
  parent_uid: 45306826826d0ac5b06dbe85b0b4d85f
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 0cf86efd25217d020b7f2167d600212c
- id: MIT6_01SC_rec10_300k.srt
  parent_uid: 45306826826d0ac5b06dbe85b0b4d85f
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuits/recitation-2-inheritance/MIT6_01SC_rec10_300k.srt
  title: MIT6_01SC_rec10_300k.srt
  type: null
  uid: da828303e5cbed0dd429d6f8f9a3dafb
- id: Caption-OCW-SRT
  parent_uid: 45306826826d0ac5b06dbe85b0b4d85f
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: 84c7764e6a9c4fa70472e81729d931a6
- id: MIT6_01SC_rec10_300k.pdf
  parent_uid: 45306826826d0ac5b06dbe85b0b4d85f
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuits/recitation-2-inheritance/MIT6_01SC_rec10_300k.pdf
  title: 'MIT 6.01SC S11 Recitation 10: Circuits: NVCC, Sample Problem Transcript'
  type: null
  uid: ce95472564b89bf2de77b68b244c412e
- id: Transcript-OCW-PDF
  parent_uid: 45306826826d0ac5b06dbe85b0b4d85f
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: 554b5427315b8fc47c0ce0002d929c4d
inline_embed_id: 86902023recitation10:circuits:nvcc,sampleproblem33882366
layout: video
order_index: null
parent_uid: c1a11356f20d61ecdbf385a0ade29169
related_resources_text: ''
short_url: recitation-2-inheritance
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/circuits/recitation-2-inheritance
template_type: popup
title: 'Recitation 10: Circuits: NVCC, Sample Problem'
transcript: '<p>PROFESSOR: Today I''d like to talk to you about a new method for solving
  circuits. Last time, we reviewed using KVL, KCL, and Ohm''s Law in order to solve
  circuits in a general sense. This produced a lot of equations, in particular, a
  lot of redundant equations or a lot of dependent equations, that we don''t necessarily
  need for solving our circuit.</p><p>Today I''m going to review the Node Voltage
  Component Current method, which is very similar to node analysis. So if you hear
  one versus the other, know that you''re talking about approximately the same thing.
  And I''ll review the difference in a second.</p><p>Once we know how to use the NVCC
  method for solving circuits, we can express the relationships between components
  in our circuit more concisely and more effectively, and possibly solve our equations
  faster, which is relevant when we''re working on a mid-term or in the general sense,
  just trying to save time. Let''s take a look at NVCC.</p><p>As I said before NVCC,
  stands for Node Voltage Component Current. And what that means is if you have a
  very simple circuit-- let''s say just a voltage source and a couple of resistors.
  Previously, with KVL, we were interested in the voltage drop around the loop being
  equivalent to 0. In this case, we''re actually going to look at the voltages associated
  with particular nodes.</p><p>To do that we''re going to label our nodes, which are
  anywhere our components connect. We''re also going to go after the component current.
  When we''re doing KCL, we typically look at the flow in and out of a particular
  node. At this point, we''re going to look at the flow through a given component.
  So we''re also going to label all of the currents associated with our circuit.</p><p>But
  when we approach NVCC method, we''re going to think about the currents flowing through
  a particular component as opposed to and out of a particular node. NVCC is sort
  of the opposite of KVL and KCL in that sense, even though you''re still going to
  end up using the same relationships. So at this point, I''ve labeled the currents
  going through-- I labeled one individual current for every component in my circuit.</p><p>The
  next step would be to identify what I''m going to call ground, or in particular,
  one of my nodes -- I''m going to assign to ground or relative voltage 0. At that
  point, I''m going to write out the relationships between the voltage drop across
  particular components, the current flowing through that particular component, and
  whatever relationship the component requires the voltage and the current to have
  to one another.</p><p>That''s a whirlwind review of NVCC method. Node analysis is
  very similar. The main difference between node analysis and NVCC method is when
  your component is a voltage source. And there are multiple currents flowing into
  that voltage source.</p><p>You can treat this as a single voltage. You can treat
  this as a single voltage node, where this voltage it has value 0. And actually write
  your KCL equations as though this point were collapsed. So current flowing in and
  current flowing out, or vice versa, have to sum to 0. That''s the major difference.</p><p>Let''s
  look at an example. You can find this example repeated in 6.4.3 of the reading.
  And I''m going to walk through these directions.</p><p>So the first thing I''m going
  to do is label my nodes and my currents. People interchangeably use e or n. It doesn''t
  really matter. I guess n in particular could refer to the node, while e in particular
  could refer to the voltage associated with that node.</p><p>Now I''m going to specify
  the voltage drop across a particular component in terms of the node voltages. I''m
  also going to assign n0 to 0 as my ground. As a consequence, I know that n1 is going
  to be 15 Volts.</p><p>My voltage drop is typically specified in the same direction
  as the current - that I''ve also decided. So this convention is arbitrary. But if
  you want to be consistent in your work, and make it easier to get partial credit
  or get help in office hours, et cetera, then assume that the voltage drop occurs
  in the same direction as the current.</p><p>That''s it for our relationship associated
  with voltage drop. Now I''m going to go over KCL for the relevant nodes. And in
  the last step I''m going to combine the two into the equation that you''re certainly
  allowed to use to express your work on midterms. Or if you can skip to the third
  step immediately, then that''s OK. Just check your signs.</p><p>Here''s the second
  step. Flowing into n1 is i0 and flowing out is i1. So i0 is going to be equal to
  i1. Flowing into n2 is i1 and i3. And flowing out of n2 is i2. Flowing into n0 is
  i2, and flowing out of n0 is i0 and i3. we''re almost certainly not going to end
  up using that equation. Because it''s the last of our KCL equations and is dependent
  upon the other equations that we''ve already written out for KCL.</p><p>I3 is equal
  to 10 Amperes. So we can go ahead and make that substitution. I still have to work
  with i1 and i2 though. And I can go after expressions for them in terms of my node
  voltages and components by using the equations for voltage drop I made earlier.</p><p>This
  is the equation that you can jump straight to, if you understand where this expression
  comes from, as a consequence, of our KCL and also our component voltages. I''m going
  to substitute in 15 Volts for n1 here. And now I have an expression that only contains
  n2 and known values. So I can solve for n2. and I''ll do that real quickly right
  now.</p><p>So first I''m just going to copy this over. I''m going to multiply through
  by 6 Ohms. And I solved for the voltage associated with n2.</p><p>At this point,
  I can solve for i2 and i1. Sorry about that. What do I have left? i3 I know is 10
  Amperes. i0 is equal to i1, which is negative 1 Amperes.</p><p>There''s a voltage
  drop associated with the 3 Ohm resistor, which is 15 minus 18, negative 3 Volts.
  And the voltage drop associated with the 2 Ohm resistor is 18 Volts, since n0 is
  ground. This concludes my introduction to node voltage component current method
  or node analysis without the ability to collapse voltage sources for KCL. &nbsp;</p>'
type: course
uid: 45306826826d0ac5b06dbe85b0b4d85f

---
None