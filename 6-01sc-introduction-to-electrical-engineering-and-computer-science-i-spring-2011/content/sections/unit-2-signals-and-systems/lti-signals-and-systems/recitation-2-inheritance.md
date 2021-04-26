---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: l0tUtVRhmDs
  parent_uid: a88c63cbdb35384bcb592b23018b9025
  title: Video-YouTube-Stream
  type: Video
  uid: 60e6cd53d270a115be36b1307a89d740
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/recitation-6-system-equivalences/id490181666?i=108667926
  parent_uid: a88c63cbdb35384bcb592b23018b9025
  title: Video-iTunes U-MP4
  type: Video
  uid: 8d95682882cc4c2c06020ace20a106ed
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_rec6_300k.mp4
  parent_uid: a88c63cbdb35384bcb592b23018b9025
  title: Video-Internet Archive-MP4
  type: Video
  uid: 86e9ea85a9a396d343652f495e323014
- id: Thumbnail-YouTube-JPG_1
  media_location: https://img.youtube.com/vi/l0tUtVRhmDs/default.jpg
  parent_uid: a88c63cbdb35384bcb592b23018b9025
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 10b4aaf2f6a219c57a4ebc3e320888c6
- id: MIT6_01SC_rec6_300k.srt
  parent_uid: a88c63cbdb35384bcb592b23018b9025
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/lti-signals-and-systems/recitation-2-inheritance/MIT6_01SC_rec6_300k.srt
  title: MIT6_01SC_rec6_300k.srt
  type: null
  uid: 60c9b2f0d0aca47350a071a40c95aff7
- id: Caption-OCW-SRT
  parent_uid: a88c63cbdb35384bcb592b23018b9025
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: 8874e28474b2355992478e5a6caa6ad3
- id: MIT6_01SC_rec6_300k.pdf
  parent_uid: a88c63cbdb35384bcb592b23018b9025
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/lti-signals-and-systems/recitation-2-inheritance/MIT6_01SC_rec6_300k.pdf
  title: 'MIT 6.01SC S11 Recitation 6: System Equivalences Transcript'
  type: null
  uid: 615a51289ed287050f55a95cb45103d1
- id: Transcript-OCW-PDF
  parent_uid: a88c63cbdb35384bcb592b23018b9025
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: 6ba0cfbd6879f22034419e670e1e1aa2
inline_embed_id: 21822172recitation6:systemequivalences21051528
layout: video
order_index: null
parent_uid: 09ae0a4b00ca37192b3ffe9f36ca05cd
related_resources_text: ''
short_url: recitation-2-inheritance
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/lti-signals-and-systems/recitation-2-inheritance
template_type: popup
title: 'Recitation 6: System Equivalences'
transcript: '<p>PROFESSOR: Hi. Today I''d like to talk about signals and systems again.
  At this point, you''re probably familiar with the motivation for why we''re talking
  about discrete linear time and variant systems, and also with a few of the representations
  that we''re going to end up using in this course. But you''re still not sure what
  it is that we''re trying to accomplish. Or where''s the part where we get to predict
  the future based on the fact that we are capable of manipulating these systems?</p><p>Well,
  we actually have to be capable of manipulating these systems. And at this point,
  we can describe this system as we see it, but we can''t also manipulate its representation
  in ways that make sense to us. So the thing that I''m going to do today is talk
  about different system equivalences and how to take a system and solve for an expression
  that represents a complex system and also how if you know that some things in your
  system are equivalent, how you can convert between them. At that point, we should
  be able to talk about poles, which is how we''re going to actually predict the future.</p><p>So
  different equivalences that I''d like to talk about. I''m first going to briefly
  review the facts that last time we discovered the notion of system function, right?
  We can take a representation of a system and abstract it away into some sort of
  function, where we take the input as it''s given to us and then multiply it by this
  function and then get the output that we''re interested in.</p><p>How do we deal
  with something more complex? I mean, y is all the way over here. And we''ve got
  multiple system functions. And I don''t even know what happens here, but it doesn''t
  have to be that scary. Let''s break it down.</p><p>One of the easiest ways to approach
  something like this is to identify each position where you have a new signal, or
  if you were to sample here, you would have a new signal, and label those values
  appropriately. You can then start with your final output and then back solve for
  the values that you''re interested in as a consequence of that final output.</p><p>In
  this particular example, y is going to be y2 plus y3. y2 is going to be y1 times
  H2, where H2 is some system function. And it probably is abstracting away some combination
  of gains, delays, and adders like this one here. y1 is going to be x times H1. And
  Y3 is going to be x times H3.</p><p>Now I''ve got all my expressions in terms of
  either y or something for which I have an equivalent expression for x. So I can
  do my substitutions, come up for an expression for y over x, in terms of H1, H2,
  and H3.</p><p>Here I''ve just made the substitutions of the equations above and
  factored out the x. If I wanted the system function, I would then just divide by
  x. And then I would have y over x is equal to this expression.</p><p>The thing I
  wanted to indicate is that if I wanted to abstract this away into its own box--
  maybe I wanted like a big H or an H0 or something like that-- and it represented
  what was happening in this top line, cascading two system functions is the functional
  equivalent of multiplying them together. So if I have an expression for H1 and I
  have an expression for H2, and I want the expression that is equal to cascading
  H1 and H2, I just multiply them together.</p><p>Likewise, if I want an expression
  for the linear combination of two system functions applied to an input individually,
  like the combination H1 and H2, and H3, it''s a summation of those two values which
  is expressed here. This is the same as the relationship that we reviewed in a very
  basic sense when we were originally doing the accumulator. The only thing I''m attempting
  to indicate is that, that relationship scales to an arbitrary level of complexity.
  So if you need to, you could shift around these values, if you can find some sort
  of equivalence.</p><p>Let''s see what happens when H2 is equal to H3. I''m going
  to take my operator equation. What this means is that if I wanted to rewrite this
  block diagram, I could do so by doing-- This is really similar to bubble pushing.
  If you''ve done 6.004 or 6.002 and have experience with logic gates, I just wanted
  to indicate that it''s also a thing that you can do for block diagrams and system
  functions.</p><p>There''s one more type of equivalence that I want to talk about.
  I call it feedback equivalence. Here''s our normal accumulator rate. If I wanted
  to represent this feedback system as a feed forward system, what would I have to
  do? Well, the first time that I sampled from x, it would just be y. So right now
  this diagram matches for the first time step.</p><p>On the second time step, if
  I had an input from x from the previous time step, I would also want to account
  for it by putting in a delay and then summing it with the current value of x in
  order to get y. At the second time step, I would want access to the starting value,
  the value from the previous time step, and the value from the current time step.</p><p>And
  one more time, to exhaust the example, at the third time step, my output would be
  a linear combination of the starting value, the value from the first time step,
  the value from the second time step, and the value from the current third time step.</p><p>We''d
  end up doing this ad nauseum to model our feedback system. So it''s difficult to
  do on paper, but it turns out there''s a great relationship between these two equivalences
  and things that we already know from-- I want to say high school calculus or possibly
  18.01, 18.02.</p><p>Geometric sequences. When we solved for the system function,
  we found an expression for our feedback system. If I wanted to find an equivalent
  expression using this feed forward system, I would look at this infinite summation
  of x terms. So if I wanted to know something about the long-term behavior of the
  system, in terms of this system function, I would solve for this expression and
  then using my knowledge of geometric sequences, in order to express the long-term
  behavior.</p><p>In the general sense, in this course, we''re going to be looking
  at the unit sample response of a system. What that means is, if the only thing I
  ever do for input is a single value of 1 at time 0, then what does my output look
  like? The reason we''re looking at the unit sample response is because it''s (a)
  the simplest way to look at the long-term behavior of a discrete linear time invariant
  system. But the other reason (b) is -- once we have this, we can also use it to
  do things like to make predictions about the long-term step response and other more
  complicated input signals.</p><p>In the case of the accumulator, if I input 1 at
  time 0, my output is going to be 1 forever more. That''s reflected in the coefficient
  of my geometric sequence. If I want to know what my long-term response is going
  to look like, I can look at the coefficient of R and make a decision about whether
  or not I''m going to diverge or converge or do neither.</p><p>So if I put a coefficient
  on R, whatever p0 converges to is what my system is going to converge to. So using
  my knowledge of p0, I can make long-term predictions about the behavior of the system.
  Next time I''m going to go over some general classifications of those behaviors
  for the system and how to more effectively use our knowledge of p0 and how to deal
  with things like second order systems. &nbsp;</p>'
type: course
uid: a88c63cbdb35384bcb592b23018b9025

---
None