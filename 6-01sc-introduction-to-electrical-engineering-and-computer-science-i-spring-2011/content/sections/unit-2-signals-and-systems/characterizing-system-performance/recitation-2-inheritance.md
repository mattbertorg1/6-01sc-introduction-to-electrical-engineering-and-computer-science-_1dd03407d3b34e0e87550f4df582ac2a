---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: QleELaAfTd4
  parent_uid: 1a9f4493139190354c5302996c08dc6b
  title: Video-YouTube-Stream
  type: Video
  uid: 80643849b6ae1f6b6216ac34dd721412
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/recitation-8-poles-part-ii/id490181666?i=108667950
  parent_uid: 1a9f4493139190354c5302996c08dc6b
  title: Video-iTunes U-MP4
  type: Video
  uid: 2ac46fc9531e3658a6357001aab7ca0b
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_rec8_300k.mp4
  parent_uid: 1a9f4493139190354c5302996c08dc6b
  title: Video-Internet Archive-MP4
  type: Video
  uid: 298fc5b8ce0eee4bb4a678f7b4755ff1
- id: Thumbnail-YouTube-JPG_1
  media_location: https://img.youtube.com/vi/QleELaAfTd4/default.jpg
  parent_uid: 1a9f4493139190354c5302996c08dc6b
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: adbbcf11ab7df2030d142f60d620c01a
- id: MIT6_01SC_rec8_300k.srt
  parent_uid: 1a9f4493139190354c5302996c08dc6b
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/characterizing-system-performance/recitation-2-inheritance/MIT6_01SC_rec8_300k.srt
  title: MIT6_01SC_rec8_300k.srt
  type: null
  uid: ae94de7c573aa41a6ded44fb3f0ec8d9
- id: Caption-OCW-SRT
  parent_uid: 1a9f4493139190354c5302996c08dc6b
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: 5de9c9dec4a35e8565c94bf2fef87fa3
- id: MIT6_01SC_rec8_300k.pdf
  parent_uid: 1a9f4493139190354c5302996c08dc6b
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/characterizing-system-performance/recitation-2-inheritance/MIT6_01SC_rec8_300k.pdf
  title: 'MIT 6.01SC S11 Recitation 8: Poles, Part II Transcript'
  type: null
  uid: 98e935a56bf61d379205317d3ec1acb3
- id: Transcript-OCW-PDF
  parent_uid: 1a9f4493139190354c5302996c08dc6b
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: 28f9202d873b608b2df6c257b81fcbc8
inline_embed_id: 43470958recitation8:poles,partii39831209
layout: video
order_index: null
parent_uid: 1900980a94dfdd0b4f70fee6ba697a76
related_resources_text: ''
short_url: recitation-2-inheritance
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/characterizing-system-performance/recitation-2-inheritance
template_type: popup
title: 'Recitation 8: Poles, Part II'
transcript: '<p>PROFESSOR: Last time we introduced poles. And in particular, we introduced
  how to move from the manipulation of feed-forward and feedback systems and the geometric
  sequence that fell out into using the base of that geometric sequence to attempt
  to predict the long-term behavior of the system. When we''re solving for poles and
  we''re only interested in long term behavior, one of the easiest ways to do so to
  solve for the roots of z, where z is a substitution for 1 over R in the denominator
  of the system function.</p><p>Once we''ve done that, we have a list of poles. From
  that list of poles, we would like to select, the dominant pole, or the pole with
  the greatest magnitude, and then based on the magnitude and period of that pole
  we can determine what the long term behavior of our system looks like.</p><p>Today
  I''d like to mention to you some notable things about poles. If you are interested
  in this information or feedback and controls in the general sense, I highly recommend
  6.003. But here''s some information you should at least be aware of as a consequence
  of 6.01. The other thing I would like to do is just walk through a couple of pole
  problems to familiarize you, or get you more comfortable with the idea of solving
  for the poles of a system function, or looking at the unit sample response of a
  system function and then graphing the poles.</p><p>The first thing that I want to
  mention is pole-zero cancellation. And what do I mean when I say that? I mean that
  if both the numerator and the denominator have a degree of R in them, then you''re
  going to have both a zero and a pole.</p><p>If the zero and the pole have the same
  value associated with them, you may be tempted to cancel them out. Unless both the
  zero and the pole are equal to 0 -- don''t do it. The reason why is that when you
  get to a implementation of a real system, it is highly unlikely that both the zero
  and the pole will be implemented to a degree of accuracy that you will actually
  see those two things cancel out. The only exception to this is when both the pole
  and the zero are equal to 0, or in this case.</p><p>This you should feel free to
  convert to this. In almost any other situation, don''t factor.</p><p>The other thing
  I want to talk about is repeated roots. If you have a repeated root, you''ll have
  repeated poles. This does get tricky when you''re talking about how to add the unit
  response of those poles. But the long term behavior of your system is going to look
  the same. So if both of these poles are the dominant pole, then the characteristics
  of both, which are the same, are going to determine what your long term behavior
  looks like. If they''re not, then the dominant pole is going to determine what your
  long term behavior looks like.</p><p>The last thing I want to mention is superposition.
  So far we''ve only talked about the unit sample response of a system function and
  how we use poles to determine what the long term behavior of our system''s going
  to be. We can look at the response to more complicated inputs than the unit sample
  response, or the delta. In fact, one of the things we'' probably end up looking
  at some point is the step function.</p><p>The thing that you need to know to go
  from talking about unit sample response to any other sort of response, is that we''re
  still working with an LTI system. What that means is if you take the summation of
  your inputs, and apply the system function to that summation, it is the same as
  the output that would result from inputting all those values at once. The best way
  I would like to explain it is by referring again to if your function was a system
  function, the same property applies.</p><p>Now let''s walk through a pole problem.
  Here I have a second order system set up. We''ve got two degrees of R. I have feedback,
  and I can solve for an expression of y in terms of x. In fact, let''s do that right
  now. y is the result of the summation or a linear combination of x plus a delayed
  signal of y scaled by 1.6 in a linear combination with a delayed value of the delayed
  value of y scaled by negative 0.63.</p><p>There''s my first degree. For consistency''s
  sake, there''s my second degree. Let''s first solve for the system function. If
  you''re confused, I recommend doing the algebra from here to this expression. You
  should get this fraction out.</p><p>Our second step is to solve for the roots of
  z. Remember that z is equal to 1 over R in the denominator of the system function.
  In this case, we''ll be working with-- all I''ve done there is taken every degree
  of R, substitute it in for 1/z. and then multiply it out, so that I''m not working
  with z in the denominator anymore. I''m actually just working with everything in
  the numerator.</p><p>If I follow this back out, I get this expression. And my poles
  are going to be 0.7 and 0.9. All right, based on my poles, what are the properties
  of the unit sample response in the long term? First thing I''m going to do is look
  for the dominant pole among the poles that I found. In this case, I don''t even
  have to worry about finding the length of the distance from the origin for poles
  in the complex plane. All I have to worry about is the magnitude of poles on the
  real axis.</p><p>0.9 is my dominant pole, because it''s the largest pole. 0.9 is
  less than 1. So I''m going to end up with convergence. Eventually, my system is
  going to converge, or tend towards 0.</p><p>The other interesting property of my
  system is what is its period, how does that relate to what my function''s going
  to look like. In this case, we''re only working on the positive real axis, so the
  angle associated with graphing this pole on the complex plane is 0, so there is
  no period for our system. This means that our system is going to converge monotonically.</p><p>Now
  let''s walk through some unit sample responses and then graph the poles that generated
  those unit sample responses on the unit circle, where this is the complex plane.
  Let''s look at this graph first. The first thing that I notice about this graph
  is that, like in the previous example, we have monotonic convergence. We''re tending
  towards 0, and we''re not alternating or oscillating about the x-axis.</p><p>So
  I know I''m going to be working somewhere along this line before the edge of the
  unit circle. Because at the edge of the unit circle, the distance from the origin
  is equal to 1. If you made me guess, then I would look at the distance here and
  compare it to the distance at the next time step.</p><p>I realize this is a blackboard.
  It''s not entirely to scale. But for the purposes of this demonstration, I''d like
  to say that the signal at this time step is 0.5 the signal from the previous times.</p><p>Likewise
  at the next time step, I would like to say that this signal is 0.5 the signal from
  the previous time step, and so on and so forth. Therefore, I''m going to graph my
  pole right here.</p><p>Let''s take a look at this graph. I''ve drawn these squiggles
  to indicate that the unit sample response exceeds the bounds of the space that I
  gave for this graph. So just assume that these values are much larger than I''ve
  drawn them.</p><p>The first thing that I notice about this unit sample response
  graph is the fact that not only am I increasing in a way that does not seem to change
  in any way-- we''re going to end up diverging-- is that I''m actually alternating
  about the x-axis. And that particularly, that if I were to call this an oscillation,
  then I would say it''s an oscillation with period 2. This means that I''m working
  with a negative real pole. The fact that I''m diverging means I''m working with
  a negative real pole that has magnitude greater than 1.</p><p>If you had to make
  me guess, I would look at the distance associated with this time step, compare it
  to the distance associated with this time step. And if you had to ask me, I would
  say this is about 1.3 the value at the previous step. Likewise, if I were to look
  at the next time step, I would say that this increase is about 30% of the previous
  value.</p><p>I''m not even going to try that one. But what I''m trying to get at
  is that you can use comparisons of previous and future time steps in order to attempt
  to determine the magnitude of the pole if you''re working with the first order system.
  If you''re working with the second order system, then it''s possible that you''ll
  see some really interesting initialization effects. And you should probably ask
  one of us what''s up. But for this example, we''re going to put our pole over here.</p><p>Here''s
  the last graph I want to talk about. The first thing that I notice is that it doesn''t
  seem to be diverging, but it doesn''t really seem to be converging either. If this
  is the case, then I''m going to put it on the unit circle. The second thing that
  I notice is that it''s not monotonic and it''s not alternating. This is oscillating.
  So in order to determine what angle I''m going to sign to my unit simple response,
  I''m going to count out the time steps that it takes to cycle through an entire
  period and then from there figure out what the angle would have to be in order to
  determine a period of that length.</p><p>So I start here. I''m just going to count
  1, 2, 3, 4, 5, 6, 7, 8 -- to complete one full oscillation. This means that my period
  is 8. If I have to divide 2pi by a particular angle in order to get out 8, I want
  to divide by pi/4. So at this point, I''m working with a magnitude of about 1, and
  I want this angle to be about pi/4.</p><p>This concludes my tutorial on solving
  poles. Next time, we''ll end up talking about circuits. &nbsp;</p>'
type: course
uid: 1a9f4493139190354c5302996c08dc6b

---
None