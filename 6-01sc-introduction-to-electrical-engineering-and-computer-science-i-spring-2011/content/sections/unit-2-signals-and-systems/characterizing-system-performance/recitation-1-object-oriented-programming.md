---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: lF-7mmPHhG0
  parent_uid: 3f561ae9f1070b802b60db574a3b4632
  title: Video-YouTube-Stream
  type: Video
  uid: b9593201c69f007e71c435f06bdb1282
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/recitation-7-poles-part-i/id490181666?i=108667928
  parent_uid: 3f561ae9f1070b802b60db574a3b4632
  title: Video-iTunes U-MP4
  type: Video
  uid: d68910cc208497fa81f59b084bf3ec9f
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_rec7_300k.mp4
  parent_uid: 3f561ae9f1070b802b60db574a3b4632
  title: Video-Internet Archive-MP4
  type: Video
  uid: ea317f6f88205591d93d76b006b50c99
- id: Thumbnail-YouTube-JPG_1
  media_location: https://img.youtube.com/vi/lF-7mmPHhG0/default.jpg
  parent_uid: 3f561ae9f1070b802b60db574a3b4632
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: ce55b9b6f1314a539295722381fec44c
- id: MIT6_01SC_rec7_300k.srt
  parent_uid: 3f561ae9f1070b802b60db574a3b4632
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/characterizing-system-performance/recitation-1-object-oriented-programming/MIT6_01SC_rec7_300k.srt
  title: MIT6_01SC_rec7_300k.srt
  type: null
  uid: 9f2a5bae7e4d7c1f5ab3b15fd529d5ae
- id: Caption-OCW-SRT
  parent_uid: 3f561ae9f1070b802b60db574a3b4632
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: 11ca8761a2b9b4e780b9034eda124f16
- id: MIT6_01SC_rec7_300k.pdf
  parent_uid: 3f561ae9f1070b802b60db574a3b4632
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/characterizing-system-performance/recitation-1-object-oriented-programming/MIT6_01SC_rec7_300k.pdf
  title: 'MIT 6.01SC S11 Recitation 7: Poles, Part I Transcript'
  type: null
  uid: eaa90db4d386e267c5a332d64fc021fe
- id: Transcript-OCW-PDF
  parent_uid: 3f561ae9f1070b802b60db574a3b4632
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: 7bde543d5ed45603a850cffec946ca46
inline_embed_id: 37783122recitation7:poles,parti59449515
layout: video
order_index: null
parent_uid: 1900980a94dfdd0b4f70fee6ba697a76
related_resources_text: ''
short_url: recitation-1-object-oriented-programming
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/characterizing-system-performance/recitation-1-object-oriented-programming
template_type: popup
title: 'Recitation 7: Poles, Part I'
transcript: '<p>KENDRA PUGH: Today I''d like to talk to about poles. Last time I ended
  up talking to you about LTI representations and manipulations. And, in particular,
  I want to emphasize the relationship between feedforward and feedback systems, in
  order to segway us into the poles..</p><p>Using what we know about that relationship,
  we can find the base of a geometric sequence. And that geometric sequence actually
  represents the long-term response of our system to a unit sample response or a delta.
  That value is also what we refer to the poles.</p><p>At this point, I''ll go over
  how to solve for them and very basic properties of them. So that we can use the
  information that we have about the poles to try to actually predict the future or
  look at the long-term behavior of our system.</p><p>First a quick review. Last time
  we talked about feedforward systems. And, in particular, I want to emphasize the
  fact that if you have a transient input to your feedforward system, you''re going
  to end up with a transient response. There''s no method by which a feedforward system
  can retain information over more than the amount of time steps that you feed information
  into it.</p><p>Feedback systems, on the other hand, represent a persistent response
  to a transient input. Because you''re working with a feedback system information
  that you put in can be reflected in more than one time step and possibly multiple
  time steps, depending upon how many delays you have working in your feedback system.</p><p>Last
  time I also drew out the relationship between feedforward and feedback systems.
  You can actually turn a feedback system or talk about a feedback system in terms
  of a feedforward system that takes infinite samples of the input and feeds them
  through a summation that takes infinite delays through your system.</p><p>You can
  represent that translation using a geometric sequence. The basis of that geometric
  sequence is the object that we''re going to use in order to predict the future.
  And that''s what we''re talking about when we talk about poles.</p><p>You can have
  multiple geometric sequences involved in actually determining the long-term behaviors
  of your system. If you only have one, then things are pretty simple. You find your
  system function. You find the value associated with p0 in this expression.</p><p>It''s
  OK if there''s some sort of scalar on the outside of this expression. We''re working
  with linear time and variance systems, so that scalar is going to affect the initial
  response to your system. But in terms of a long term behavior, it doesn''t matter
  as much. So don''t worry about it right now.</p><p>Relatedly, if you''re solving
  for these expressions in second or higher order systems, you''re going to end up
  having to solve partial fractions. You can do this. And in part, one of the reasons
  that you would want to do this is so that you can get out those scalars, if you''re
  going to be talking about the very short-term response to something, like a transient
  input.</p><p>We''re not going to be too interested in those in this course. We''re
  mostly going to be talking about long-term response. So we can get around the fact
  the we''re dealing with a higher order of systems and not solving partial fractions
  by substituting in for an expression called z, which actually represents the inverse
  power of R and then solving for the roots of that equation.</p><p>If you substitute
  z in for 1 over R in this denominator and then solve for the root associated with
  that expression, you''ll get the same result. You''ll actually end up out with p0.</p><p>All
  right. So now we know how to find the pole or multiple poles, if we''re interested
  in multiple poles. What do we do now? I still haven''t gone over how to figure out
  the long-term behavior of your system.</p><p>The first thing you do is look at the
  magnitude of all the poles that you''ve solved for and select the poles with the
  largest magnitude. If there are multiple poles with the same magnitude, then you''ll
  end up looking at all of them. If you have different properties than the ones here,
  you can end up with some, you know, complex behavior. I would not worry about that
  too much. Or I would ask a professor or TA when that happens.</p><p>But in the general
  sense, if your dominant pole has a magnitude greater than 1, then you''re going
  to see long-term divergence in your system. This make sense if you think about it.
  If at every time step your unit sample response is multiplied by a value that is
  greater than 1, then it''s going to increase. And, in fact, the extent to which
  the magnitude of your dominant pole is greater than 1 is going to determine your
  rate of increase and also determine how fast your envelope explodes.</p><p>Similarly,
  if the magnitude of your dominant pole is less than 1, then in response to a unit
  sample input or a delta, your system''s going to converge. This also makes sense
  intuitively. If you are progressively multiplying the values in your system by a
  scalar that is less than 1, then eventually you''re going to end up converging to
  0.</p><p>To cover the only category we haven''t talked about, if your dominant pole
  is actually equal in magnitude to 1, then you''re not going to see convergence or
  divergence. And this is one of the places in which the magnitude of the scalar that
  you end up multiplying your system by can become relevant. We''re not going to focus
  on this situation too much. But it''s good to know what actually happens when the
  magnitude of your dominant pole is equal to 1.</p><p>The other feature that we''re
  interested in when we''re looking at the dominant pole of a system is if we were
  to represent the dominant pole in this form, what the angle associated with that
  pole is, if you were to graph that pole on the complex plane using polar coordinates.
  If your pole stays on the real axis, or if your pole does not have a complex component,
  then you''ll see one of two things.</p><p>The first thing that it''s possible for
  you to see is that you''ll get absolutely non-alternating behavior. Your system
  response stays on one side of the x-axis and either converges, diverges, or remains
  constant as a consequence of input of the unit sample. And you won''t see any sort
  of alternating or oscillating behavior. This only happens when your dominant pole
  is real and positive.</p><p>If you''re dominant pole is real and negative, this
  also means that it''s still on the real axis, but its value is negative. So if you''re
  looking at polar coordinates, it''s going to have an angle pi associated with it.
  This means you get alternating behavior. And what I mean when I say alternating
  behavior is that your unit sample response is going to jump across the x-axis at
  every time step. This is also equivalent to having a period of 2.</p><p>The other
  situation you can run into is that this angle is neither 0 nor pi. And at that point
  you''re going to be talking about oscillatory behavior or a sinusoidal response
  that retains its edges at the envelope of your function. In order to find the period,
  or in order to find the amount of time it takes for your unit sample response to
  complete one period, you''re going to take the angle associated with your dominant
  pole and divide 2pi by it. This is the general equation for a period.</p><p>This
  covers the basics of what you want to do once you already have your poles. Next
  time I''m actually going to solve a pole problem and show you what the long-term
  response looks like and also talk about some things about poles that I''ve pretty
  much skimmed over. And at that point you should be able to solve and look at poles
  for yourself. &nbsp;</p>'
type: course
uid: 3f561ae9f1070b802b60db574a3b4632

---
None