---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: oTNwGuI7Wic
  parent_uid: ec1daae8fe0f5dad365fb58e2a0f3def
  title: Video-YouTube-Stream
  type: Video
  uid: 4e5499fc60935bf1b66260686fc45c94
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/lecture-6-designing-control/id490181666?i=109416111
  parent_uid: ec1daae8fe0f5dad365fb58e2a0f3def
  title: Video-iTunes U-MP4
  type: Video
  uid: 052e1e9a399da97573e04b78bb1d582a
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_S11_lec06_300k.mp4
  parent_uid: ec1daae8fe0f5dad365fb58e2a0f3def
  title: Video-Internet Archive-MP4
  type: Video
  uid: 86d17759ab28961647aab60b260ade84
- id: Thumbnail-YouTube-JPG_1
  media_location: https://img.youtube.com/vi/oTNwGuI7Wic/default.jpg
  parent_uid: ec1daae8fe0f5dad365fb58e2a0f3def
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 83aa470e22a512bfd2172437cc0c2a0f
- id: MIT6_01SC_S11_lec06_300k.srt
  parent_uid: ec1daae8fe0f5dad365fb58e2a0f3def
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/designing-control-systems/lecture-1-object-oriented-programming/MIT6_01SC_S11_lec06_300k.srt
  title: MIT6_01SC_S11_lec06_300k.srt
  type: null
  uid: f5872d3c7ad271f58012c13b3cdc1d32
- id: Caption-OCW-SRT
  parent_uid: ec1daae8fe0f5dad365fb58e2a0f3def
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: 9f41ec24736bde522730d8c844cd992b
- id: MIT6_01SC_S11_lec06_300k.pdf
  parent_uid: ec1daae8fe0f5dad365fb58e2a0f3def
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/designing-control-systems/lecture-1-object-oriented-programming/MIT6_01SC_S11_lec06_300k.pdf
  title: 'MIT 6.01SC S11 Lecture 6: Designing Control Systems Transcript'
  type: null
  uid: b2937c9a50a95d980a646530a424ca7c
- id: Transcript-OCW-PDF
  parent_uid: ec1daae8fe0f5dad365fb58e2a0f3def
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: b0d48982b901a6023dc6f03a660da012
inline_embed_id: 61630553lecture6:designingcontrolsystems25106576
layout: video
order_index: null
parent_uid: 65b2b6f46f8dd1495f79bc7dbf57364e
related_resources_text: ''
short_url: lecture-1-object-oriented-programming
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-2-signals-and-systems/designing-control-systems/lecture-1-object-oriented-programming
template_type: popup
title: 'Lecture 6: Designing Control Systems'
transcript: '<p>The following content is provided under a Creative Commons license.
  Your support will help MIT OpenCourseWare continue to offer high quality educational
  resources for free. To make a donation or view additional materials from hundreds
  of MIT courses, visit MIT OpenCourseWare at ocw.mit.edu.</p><p>PROFESSOR: Today
  I want to talk a little bit about designing control systems. This will finish up
  our discussions on signals and systems. Let me then just briefly review where we
  are. Hopefully this might help you also for perspective with regard to thinking
  about the exam tonight.</p><p>We''ve looked at a bunch of different kinds of representations
  for discrete time systems. The easiest, most concise method we looked at was the
  representation using a difference equation. That''s mathematically as concise as
  you can get. But it doesn''t tell you important things like who''s the input and
  who''s the output and what are all the different ways that you can get through the
  system from input to output?</p><p>So for that question block diagrams are nice.
  Block diagrams are graphical. It makes it very easy to see when there is, for example,
  a cyclic path through the network.</p><p>But they''re graphic. They''re not nearly
  so concise as difference equations. So then we went on to operators. Operators are
  just as concise as difference equations but they contain additional information
  because the operators have an implicit argument. So there''s an input, which is
  the argument to the operator, and there''s an output, which is the output of the
  operator. So you can tell who is the input and who is the output.</p><p>So that''s
  good. That sort of combines the strengths of difference equations and block diagrams.
  You end up with a concise representation that has complete information about the
  signal flow paths.</p><p>Furthermore, you can analyze the operators by using polynomial
  mathematics and that gives rise to the notion of a system functional. And that''s
  a very nice closure because that represents an abstraction that lets us think about
  a whole system as though it were just one part, one thing, one operator.</p><p>So
  we use that structure then, all of those representations, to try to learn about
  feedback. And first off, in the block diagram it''s very easy to see that any time
  you have feedback -- feedback so enormously powerful that we want to use it in design
  -- but you can see immediately from the structure of the block diagram that if you
  have feedback then you have cycles.</p><p>Why is that interesting? Well, that''s
  interesting because if you have cycles then even transient inputs can generate persistent
  outputs. So that''s a kind of behavior that we would like to understand.</p><p>From
  the nature of feedback it generates cycles. From the nature of cycles it generates
  persistent responses even if there''s no input. And we saw that we could characterize
  those by thinking about those responses for one part at a time. And those parts
  we thought of as poles and the responses to a single pole we called modes. So we
  thought through a way of decomposing the response of a complicated system in terms
  of a number of additive components that are based on poles. Poles are just the base
  of a geometric sequence.</p><p>So today then what I want to do is use that framework
  to think about design. How would you optimize the design of a controller?</p><p>Looking
  back to where we''ve been, way back in Lab 4, ancient history, we looked at how
  you could program the robot to approach a wall. And we saw that depending on how
  you set up that system you could get very different performances. And what we''d
  like to do is have a way that we can design for performance without actually building
  it. The kind of thing that we built in the lab, Lab 4, was so easy that building
  it to determine its behaviors was not a bad problem.</p><p>But In general if you
  were building a 777, there''s more than one pole. And you wouldn''t necessarily
  want to test drive all of the bad configurations. So we''d like to be able to understand
  that kind of a problem analytically. We''d like to be able to analyze it.</p><p>So
  using the different representations you can generate a very concise representation
  just thinking in terms of difference equations. You all did this in Lab 4. And you
  get a single difference equation that tells you in principle everything there is
  that you could know, but not in a form that''s very easy to analyze.</p><p>It''s
  a bit better if you translate the difference equation into a block diagram because
  now you can see that this system of equations has in fact two feedback loops in
  it. Two cycles. Two things that might potentially generate persistent responses
  to transient signals, which could then degrade performance. If the transient signal
  lasts ten years it might be a bad controller. If the 777 hits turbulence and never
  stabilizes that would be bad. If small disturbances got bigger with time that might
  be bad, right?</p><p>So we can see that this simple controller described by these
  difference equations has the potential to do that sort of stuff. And we''d like
  to understand, when does it?</p><p>The easiest way to think about analyzing this
  is to focus first on the inner loop and ask the question, what''s the functional
  representation for that box which we would call an accumulator? This box, this thing,
  accumulates at its output, the sum of all the things that ever came in so we call
  it an accumulator. So what''s the functional representation of an accumulator? Well,
  we just do polynomial math. Easy so we can recognize from the block diagram that
  the signal Y could be constructed by applying R to W.</p><p>But we can also see
  in the block diagram that W is the sum of X and Y. And then if we take the left
  hand side and the right hand side of this double equation we get something that
  involves just X and Y, which we can solve for the ratio Y over X. Which then says
  that the ratio is R over (1 minus R). That''s a functional representation for the
  effect of the accumulation.</p><p>That''s also something that comes up so frequently
  in the design of control systems that we give it a name. We call this Black''s Equation.
  And it''s especially useful to avoid these little trivial steps in algebra, to just
  jump to the answer.</p><p>So let''s see that everybody''s following me. The equation
  for this box is the thing that we will call Black''s Equation. It''s not mysterious.
  It''s something that you could derive, so derive it. Figure out the functional form
  for the system that goes from X to Y and figure out which of these forms is correct.
  (1) through (4), or (5) if none of the above applies. So take 30 seconds, figure
  out the answer. I''m going to ask you to raise your hand. You''re free to talk to
  your neighbors.</p><p>OK. So everybody who raised your hands tell me what the right
  answer is. OK, wonderful. It''s about 95%. No. It''s about 100% correct out of about
  95% participation. So the answer you can form just like we did before, no particular
  tricks, using simple algebra. Simple algebra you get F over (1 minus FG). The thing
  I want you to recognize is kind of a graphical way of thinking about that. And you
  can just memorize F over (1 minus FG) and that''s fine.</p><p>But there''s some
  interesting things that the designer thinks about. This functional form is F, that''s
  the forward gain. That''s the gain through the system starting at the input and
  going directly to the output. So this form says that the closed loop gain, the system
  function that results when the loop is closed, is just the forward gain, F, divided
  by (1 minus the loop gain). The loop gain is the product around the loop once. So
  that''s just a convenient way of thinking about it. Any time you have a feedback
  system of this type you can think about the closed loop response as being the forward
  path F divided by (1 minus loop gain FG).</p><p>So the answer was 1. And generally
  we''ll see two different ways of representing the system. Sometimes we''ll represent
  it with a plus as we did with the accumulator. Many times we''ll represent it with
  a minus. That''s the way we think about control problems. We put in the minus because
  we''d like to think about the controller as trying to make something go to 0. So
  when you take the difference, that gives us an error signal. And then we can think
  about the controller being the thing that drives that error to 0.</p><p>But however
  you think about it, there''s two forms that are very closely related. They really
  differ by just a minus sign which you could think of as just multiplying G. So it''s
  sort of like the right hand side is just a minus G plugged into the left hand side.</p><p>So
  then the way you use this idea, you think about the block diagram and you say, OK
  I can replace this thing with an equivalent system which is R over (1 minus R) and
  then repeat. So the R over (1 minus R) means that, if you think about Black''s Equation
  now for this loop, you should think about the forward gain, K minus T, R over (1
  minus R), that''s this. Divided by (1 plus the loop gain). So 1 plus, and the loop
  gain, well, the wire down here just has a gain of 1. So the loop gain  and the forward
  gain are the same thing. So you get this kind of expression which simplifies to
  this.</p><p>There''s two things I want you to see about this. First off, I want
  you to see that even though the simple-minded way of plugging in said that we should
  have got a quotient of quotients N over D over N over D, it''s simplified to a single
  ratio. If you design a system out of just adders, gains and delays, that will always
  be true. There''s a closure. It will always be the case that the functional that
  represents a system of that form will always have the property that it''s a polynomial
  in R divided by another polynomial in R, that''s just the way polynomials work.</p><p>The
  other thing is that you can now start to interpret what the behavior of this could
  represent in a simpler form than thinking about this. So this kind of a representation
  that leads to intuition about what the behavior should be is very helpful when you''re
  thinking about design. And in particular this particular thing says that if we think
  about a simpler system that could generate that same response we can generate some
  intuition for how we would like to set the parameter k. So in particular this system
  functional which we generated for this system could equally apply to that system.
  Is that clear?</p><p>So there''s a numerator, which I''ve represented here. There''s
  a numerator, which has an R in it and has a minus kT in it. I''m going to, for reasons
  that you''ll see in a minute, I''m going to call something P0 because it''s the
  pole. So the numerator I''ve represented here and this denominator has this form.
  And I wrote it that way because this is the canonical form for the way of thinking
  about a pole.</p><p>So what I showed is that even though this was a more complicated
  system you can think about it as the cascade of a delay, a gain, and a pole. The
  pole can be calculated from the gain, the pole is the multiplier for R, so the pole
  is (1 plus kT). So if I were to choose kT to be minus 0.2 then the pole would be
  at 0.8. If the pole is at 0.8 then the mode, the natural response to the pole, would
  have the form P to the n. They always have the form geometric P to the n, so it
  would look like 0.8 to the n. Because of the pre-multiplier of 1 minus P0 the whole
  thing gets multiplied by 0.2 and because of the delay the whole thing gets shifted
  to the right.</p><p>The important thing is that by thinking about manipulating this
  as an operator we can recognize and simplify the form of the behavior. That gives
  us an intuitive grasp over how to best choose kT. It''s all clear?</p><p>Now, the
  behaviors that we''re interested in are not always unit-sample responses. We do
  unit-sample responses because they''re the easiest possible thing we could think
  of, right? A unit-sample is the simplest non-zero signal. A unit-sample is the signal
  that is different from 0 in exactly one place -- the easiest possible place, 0.
  And it has its easy-as-possible non-zero value -- 1. So we focus on the unit-sample
  signal because it''s the easiest possible signal we could think about.</p><p>But
  when we''re thinking about behaviors we''re often thinking about other things. Often
  we''ll think about the step response. Here I have illustrated the way you would
  measure a step response. A step response is what would happen if the output were
  initially 0, if we were at rest, and suddenly we turned on a signal that was constant
  at 1.</p><p>That would happen in the robot case if we started the robot close to
  the wall, at rest, near 0 -- so that the output signal is close to 0, but the desired
  input was a meter behind. Then that would be an input signal that started at time
  equals 0 equal to 1 and persisted forever at 1. And the result then would be what
  we call the step response.</p><p>The step response is typically easier to measure
  in the lab than is the unit-sample response. So we use the unit-sample response
  when we''re thinking analytically, when we''re doing calculations, and we use the
  step response when we''re in the lab trying to measure something.</p><p>And the
  whole theory wouldn''t be very useful if there weren''t a close relationship between
  those two things. This diagram illustrates the relationship. If we think about a
  system H for which we would like to find the step response, the step response to
  that system is what would the system do if you put the unit-step into the system.
  I''ve represented the unit-step here as u[n]. u[n], the signal that is 0 for n less
  than 0, and 1 for n bigger than or equal to 0 -- is just the accumulation of the
  delta function, the unit-sample.</p><p>So this system, the cascade of an accumulator
  with H, would measure the step response of H if it were driven with the sample signal.
  Because of the properties of polynomials and because block diagrams follow the rules
  for polynomials, we can flip these whenever the systems both start at rest, and
  if we flip those we get a different interpretation.</p><p>What this says is that
  if you were to take H and stimulate it with the unit-sample you would get h, little
  h, which we would call the unit-sample response because it''s the response to the
  system when the input is the unit-sample. So if you measured h with the unit-sample
  rather then with the unit-step you would get the unit-sample response from which
  you could generate the step response by running it through an accumulator.</p><p>So
  what that says is there''s a close association, there''s a close relationship, between
  the unit-sample response and the unit-step response. One is the accumulation of
  the other. The unit-step response is the accumulated response to the unit-sample
  response. So that means that in that previous example where we saw that setting
  kT equal to minus 0.2 resulted in this unit-sample response, that would correspond
  to this unit-step response. All you do is for every sample you calculate, for this
  response you calculate the sum of say, n equals 0, you would take the sum of all
  of the previous answers in H[n]. It''s the accumulation.</p><p>So it starts at 0
  since the sum of all those numbers is 0. Then at time 1 it becomes the sum from
  here back so it becomes 0.2. Then here it''s the sum from here back. And if you
  add these all up it becomes a number that approaches 1. Not surprisingly, right?
  If you''ve got a feedback system and if you started the robot up against the wall
  and the desired position was one meter behind you would monotonically approach 1,
  OK?</p><p>And what you can see is that if you change the value of the pole, here
  I''ve changed the kT from minus 0.2 which is what the previous answer was, to minus
  0.8, I''ve changed the value of the pole, the unit-sample response got faster. And
  the unit-step response also got faster.</p><p>The point is there are different kinds
  of performance metrics that we might want to use, unit-sample response, unit-step
  response, but the responses of all of them, you can tell something about the response
  to all of them from the response of the unit-sample signal. That''s why we focus
  so much on the unit-sample signal. It''s not because it''s the most popular thing
  to use in the lab. It''s because it''s the easiest thing to calculate with and it
  gives us insight into things that we would like to measure in the lab.</p><p>So
  for this very simple system what you can show is that there''s only a few possible
  behaviors, a few categories of behaviors. If you were to choose kT to be between
  0 and 1, then the pole, which is (1 plus kT) would also be between 0 and 1. Since
  the system has a single pole you can say a lot about the response from the numerical
  value of the pole.</p><p>If the pole is between 0 and 1 then the response is going
  to be monotonic and converging. That results because the unit-sample response was
  positive only and decayed towards 0. Because it''s positive only it means monotonic
  -- goes to 0 and makes it converge.</p><p>So you can infer properties about the
  unit-step''s response from properties of the pole just like we could infer properties
  of the unit-sample response. If you changed kT to be between minus 2 and 1 you get
  a P0 that''s between minus 1 and 0. Again that''s just that equation. That says
  that the response will be alternating.</p><p>So the sign of the unit-sample response
  goes positive then negative. It still converges in the sense that the unit sample
  response approaches 0. And what that means for the unit step-response is that the
  unit-step response will converge toward 1. The sign doesn''t alternate around 0,
  the sign alternates around 1. So again, you can infer the properties of the unit-step
  response from the properties of the unit-sample response.</p><p>And if you have
  kT that is less than minus 2 then you get a P0 that''s less than minus 1 and that''s
  a divergent response.</p><p>So the point is you can infer properties about the control
  system by thinking about the poles of the system where here I''ve illustrated it
  for a simple system that only has one pole.</p><p>OK. I told you a bunch of facts.
  Now you figure out something. How would I choose k for this system to get the quote,
  &quot;best performance?&quot;</p><p>So which value of kT would give the fastest
  convergence for the unit-sample signal? OK, participation is down but the hit rate
  is still good. Virtually everybody who volunteered to answer got the right answer.</p><p>The
  most popular answer was (2). Why is the answer (2)? What''s the range of possibilities
  that we could get? If we choose k, or kT, we could choose kT to be-- what''s the
  range of kT that we could use? Minus 2 to 0? [INAUDIBLE] we could use kT, any real
  number, right? We couldn''t use imaginary numbers because that doesn''t sort of
  make sense for a real system.</p><p>But we could choose any real number. The real
  numbers map, according to this chart, the real numbers map to a different real number.
  If you choose kT you can figure out where is the pole by that mapping.</p><p>Where
  would you put the pole to get the fastest response? If you have your choice of putting
  the pole anywhere on this red line, that red line or that red line, where would
  you put it and why?</p><p>AUDIENCE:  Just inside the [INAUDIBLE]</p><p>PROFESSOR:  Putting
  it inside the unit circle would probably be a good idea because?</p><p>AUDIENCE:
  [UNINTELLIGIBLE]</p><p>PROFESSOR: Yeah. If you didn''t put it inside the unit circle
  it wouldn''t converge. That''s right.</p><p>So you like [UNINTELLIGIBLE] the inside.
  Given  the choice of anywhere here and anywhere here which would you choose? How
  would you choose it? Yeah.</p><p>AUDIENCE:  Derive.</p><p>PROFESSOR:  Derive. And
  how do you get that?</p><p>AUDIENCE: [UNINTELLIGIBLE]</p><p>PROFESSOR:  What would
  happen if it was close to [UNINTELLIGIBLE]? It converges quite quickly, right? Poles
  always converge geometrically. The base of the geometric is the pole value. So you''d
  like the pole to be as small as possible to get the convergence as fast as possible.
  That make sense to everybody?</p><p>So in particular for this example if you chose
  kT to be minus 1 in that limit then this entire factor goes away. So the entire
  response degenerates to R and R is not instantaneous but it''s pretty fast. What
  that says is that you get to the final value in one step.</p><p>So if the input
  consisted of a unit sample, which has non-zero value only at 0, the output would
  have non-zero value only at 1, right?</p><p>Thinking about the way that works in
  practice, think about the robot and think about we''re trying to drive toward the
  wall. If we made kT be minus one, and just for the sake of being concrete let me
  say that T is about 1/10. That''s what the sampling period is for the robots we
  use in the lab. If T were 1/10 then the best k would be minus 10. And what that
  says is that if we were 1 meter away from where we want to be we would set the velocity
  to 10 meters per second. What that says is that if we started 1 meter away from
  where we want to be, so this is intended to represent position on the same axis
  that this has showed, so if we started here and we wanted to be here, time is plotted
  down.</p><p>If we use the rule that we just specified then we would set the velocity
  given this condition which is 1 meter away from where we want to be. We would set
  the velocity to be 10. If we set the velocity to be 10 then after 1 unit of time,
  after 1/10 of a second, we are 1 meter to the right, which just happens to be exactly
  where we want to be. Had we chosen k to be bigger we would have overshot. Had we
  chosen k to be smaller we would have undershot. k equals 10 gave us precisely the
  right answer so that we get there in one fell swoop.</p><p>Then on the very next
  step we would compute a velocity of 0 because we are at where we want to be so we
  would stay there. And that condition would persist forever.</p><p>The idea would
  be this simple system provides a way that we could set the gain so we could get
  to where we want to be in one step. It''s hard to beat that.</p><p>The problem that
  results and the reason you didn''t see that good behavior in the lab was that the
  sensors in the robot don''t work instantaneously. They introduce delay. And as an
  idealization of that delay I want to think through the same problem. But now let''s
  say that the sensor delays the input to the sensor which is the output of the system.
  Let''s say that the sensor introduces a delay of 1, so now instead of reporting
  d sensed, which was d0[n], it reports d0[n minus 1].</p><p>So now what would happen?
  Now with the delay, if I started here and if by some mysterious process I was here
  at time n equals 1, then I would calculate my new velocity. What would be my new
  velocity here? I''m right where I want to be. What would be my new velocity if I
  assume that the sensor has a delay of [UNINTELLIGIBLE]?</p><p>AUDIENCE:  10.</p><p>PROFESSOR:  10.
  Because of the delay the sensor is reporting that I''m a meter away from where I
  want to be. So the controller calculates, oh, I need to go forward a meter. I''ll
  set the velocity to 10. So having set the velocity to 10 and then one step goes
  by, now we''re completely on the wrong side. That''s what happens when you put delay
  into the system. So because we''re basing this decision on where we were last time
  we go to the wrong place.</p><p>So now we''re here. What will the controller say
  next?</p><p>AUDIENCE: [UNINTELLIGIBLE]</p><p>PROFESSOR: Stay here. You''re in a
  great place. I''m really 1 meter too close. In fact I banged into the wall. But
  the sensor is telling me I''m exactly where I want to be so stay here. Say I didn''t
  kill myself, what will the velocity next be? Minus 10. So now I tell myself to go
  back. That''s probably a good move. But now I still think I''m too close to the
  wall so I tell myself to continue to back up.</p><p>The idea is that I get poor
  performance. The delay had a devastating effect on the way that the controller worked.
  Even though it''s a tiny change to the way the system works it has a devastating
  effect on behavior.</p><p>We''d like to be able to predict that without having to
  measure it. Here''s the same equations except that I put a delay in the sensor.
  Here is the same block diagram but I''ve represented a delay in the sensor path.
  So now the question is, what''s the new functional representation for that control
  system?</p><p>&nbsp;</p><p>So what''s the answer? Can you rate the functional form
  for this system as one of (1), (2), (3), or (4), or is it none of the above? About
  1/3 participation and about 100% correct. The answer''s four. You get to use Black''s
  Equation or however you''d like to think about that. You can think about reducing
  the inner loop the same as we did before and then think about this as forward over
  (1 plus loop gain) but now the loop gain has R squared in it instead of R. We get
  this form.</p><p>How does this form differ from when the R wasn''t here? What''s
  the difference between R not there and R is there? What''s the answer? Anyone?</p><p>AUDIENCE:
  [UNINTELLIGIBLE]</p><p>PROFESSOR: The squared term. So this term in the previous
  form was just an R and in this form is a square and so what''s that do? What''s
  the importance of the fact that there''s a square there? Two poles, right? We now
  have a polynomial in the denominator that is quadratic in R.</p><p>And what that''s
  going to do is it''s going to give us two poles instead of one. The importance of
  that is that now we''re going to have to think through-- we previously categorized
  what were all the behaviors you could get from one pole. The behaviors you can get
  from one pole were monotonic divergence, non-monotonic alternating divergence, monotonic
  convergence, alternating convergence. So there were four behaviors that were possible
  with one pole.</p><p>Now we have to think through what are all the possible behaviors
  that we could get with two poles. Different problem. Hopefully they''re related.</p><p>So
  here, the way we would find out what the poles are is take this expression, substitute
  for every R, 1 over z, turn the ratio of polynomials in R into a ratio of polynomials
  in z. To do that in this case I had to multiply numerator and denominator by z squared.
  Having done that I get a second order polynomial in z in the bottom so there''s
  two poles which are the roots of that polynomial. And that''s just a quadratic equation.</p><p>The
  interesting thing now is to map out what are all the possible behaviors that that
  system can give us. It''s important to realize that''s a simple generalization of
  what we saw before. It will be the case that any system that we construct out of
  adders, gains and delays will have the property that we can write the system functional
  as a ratio of polynomials in R. By the factor theorem we will always be able to
  factor the denominator. And by the notion of partial fractions we''ll always be
  able to write some complicated expression like that in terms of a sum of parts.
  Each part being first order.</p><p>The intuition we get from this is that what we
  ought to do is factor the denominator, find the poles, and associate a behavior
  with each of those poles.</p><p>Here''s what the problem looks like for the two
  pole problem. If we have the general form given here and if we start by thinking
  about kT having a small magnitude, if kT has a small magnitude then we have 1/2
  plus or minus the square root of 1/2 squared. So that''s 1/2 plus or minus 1/2.
  That''s 0 or 1. So the poles for this system, if you make k be very small, the poles
  are at 0, near 0 and near 1. Is that a good system response or a bad system response?</p><p>Bad.
  Why? Well, we''re trying to think through the behavior of the  second order system
  by thinking about the separate behaviors of each of the poles.</p><p>Is this a good
  pole or a bad pole? Why? The response is always pole [UNINTELLIGIBLE]. The mode
  associated with the response at a pole near one is something near one to the end.
  That never converges. If you start with some error the error persists forever. Well,
  that''s not good. If wind turbulence knocks you into a decline in your airplane
  and it persists forever, that''s not good. You would like those things to damp out.</p><p>So
  this pole is bad. How about that pole? That one has a response that decays quickly.
  But the problem is that when you add the two pieces together, that was the reason
  I showed you this decomposition, you can think about the polynomial being factored
  and being broken into a number of parts. The part that''s associated with the pole
  near one has a response that goes for a long time. So that will asymptotically dominate
  your response. So we refer to this as a dominant pole. This pole dominates the response.
  That''s a way of inferring the behavior of two poles from the sum of single poles.
  In this particular case there''s one pole that matters more than the other one.
  So we call that pole the dominant pole.</p><p>If you were to make kT more negative,
  So here''s the general form. If you make kT negative, you can make the thing under
  the radical sign go towards 0. If you made the thing under the radical sign go to
  0 then you would get two poles at 1/2. So here we would see that if kT were minus
  1/4, if kT were minus 1/4 we would have 1/2 squared, which is plus 1/4. Minus 1/4
  would give us 0 under the radical.</p><p>So we would get two poles at 1/2. Is that
  good or bad? Well, it''s better than the previous example, right? Because each of
  those poles is associated with the response where the error gets half what it used
  to be on every step. So it converges.</p><p>If going from 0 to minus 1/4 is good,
  then going to minus 1/2 might be better, right? If you continue that trend, say
  you make kT be minus 1, if kT is minus 1 then you get 1/2 squared minus one. So
  1/2 squared is 1/4, minus 1 would be minus 3/4. That gives us a complex pole here.
  So we get two poles that are right on the unit circle.</p><p>What''s that mean?
  That means oscillations. Oscillations is something you can''t get with one pole
  with a real system. Oscillations result from a poll that has an imaginary component.
  If the system is real you could only get such poles in pairs. So it''s this pair
  that makes sense for a real valued system. And that gives rise to oscillations and
  that''s exactly what we saw here. So we can associate the oscillations that we saw
  in the simulated lab experiment with poles that have imaginary components.</p><p>So
  what would be the period of the oscillation in the system given by 1/2 plus j root
  3 over 2?</p><p>AUDIENCE: [INAUDIBLE]</p><p>PROFESSOR:  Excuse me? Excuse me?</p><p>AUDIENCE:  Where
  did the root three come from?</p><p>PROFESSOR: The previous page. If you substitute
  minus 1.</p><p>So what''s the period of the oscillation? So the period''s represented
  by 5 converged into 6.</p><p>So how do you get 6? The easiest way to think about
  that is to think about the poles being expressed in polar notation. The poles we
  previously said were 1/2 plus or minus j root 3 over 2. That''s the same as e plus
  or minus j pi over 3. It''s easier to use that form because if you take that form,
  so if you think about e to the j, what was it, 2 pi over 3? Pi over 3.</p><p>So
  if you think about that form, that''s the pole, we can write that that way. Then
  the inside has a magnitude of 1. So we can think about that just being a magnitude
  of 1 and an angle of pi over 3. So when you raise that to the n, the magnitude to
  the n, one to the n is always 1, and the angle raised to the n, it just increases
  linearly with n. So the angle goes from pi over 3 to 2pi over 3 to pi to 4pi over
  3, et cetera.</p><p>So you can think about this going from pi over 3, 2pi over 3,
  pi, 4, 5, 6. It takes n equals 6 to get around to where it started so the period
  is 6.</p><p>If you were to further change the game, if you were to make it even
  more negative, the poles would go outside the unit circle. And then what would happen?</p><p>AUDIENCE:
  [UNINTELLIGIBLE]</p><p>PROFESSOR:  Right. So that''s completely unacceptable. The
  point is that by changing the gain you can get any behavior on this figure which
  is called the root locus. So root meaning the root of a polynomial. Locus meaning
  the acceptable values of points. So the root locus shows you all the possible behaviors
  they could result from this system.</p><p>So given that root locus, how would you
  choose k to make your system response as fast as you could? So what value of kT
  would you want? Everyone raise your hands. That''s very good. So the most popular
  answer is number (2). So why would the answer be number (2)? What do you look at?
  Yeah?</p><p>AUDIENCE: [INAUDIBLE]</p><p>PROFESSOR: Remember what we''re trying to
  do. We''re trying to infer properties of the behavior of this second order system
  from the pole locations. We know that there''s an expansion that lets us expand
  the system in terms of the sum of two first order responses. The slowest of the
  first order responses will dominate eventually. So what we need to look at is the
  slowest of the two responses.</p><p>We would like to know of the two poles which
  one is the slowest? The slowest is the one that''s closest to the unit circle. So
  we would get the fastest response when the slowest one is as fast as possible. As
  the poles initially go toward each other from 0 to 1 this one is getting faster,
  this one is getting slower. So the slowest one is this one. So the slowest one is
  fastest when they meet.</p><p>And then when they diverge does the slowest one get
  faster or slower? It''s already slower because it gets closer to the unit circle.
  So you get the fastest response whenever you get the two poles both colliding at
  1/2 and that was the case that happened when kT was minus 1/4 from two or three
  slides ago.</p><p>So the idea then is to try to infer what would be the behavior
  of this higher order system by thinking about the behaviors of the individual components,
  here the poles. And what we saw was something that''s in fact a very important general
  trend. What we saw was that we first analyzed the wall finder system assuming there
  was no delay in the sensor. And we found that that system was characterized by a
  single pole and we had the design freedom of putting that pole anywhere we wanted
  to on the real axis. And that allowed us to choose the pole to be at 0 which gave
  terrific performance.</p><p>The interesting thing that happened when you add just
  one more pole by putting a delay in the sensor, you make the system more complicated
  and now you can''t possibly get nearly so good behavior. The behavior is a lot worse
  than it was before. And in fact, if you were to do the same kind of analysis by
  putting yet another delay in the sensor you would find even worse behavior.</p><p>The
  idea then, the generalization of the way the behaviors is working, generally speaking
  adding delays inside a feedback loop is a destabilizing thing. Generally as the
  number of delays increases you end up having to back off on the maximum gain that
  you can use because the system becomes less stable.</p><p>So the overall moral is
  that delays are bad generally. I mean, you could concoct some kind of a weird scheme
  where that wouldn''t be true. But it''s actually hard to concoct such a weird scheme.
  In general, and in virtually every physical system that you''ll run into, adding
  delays makes the system harder to stabilize. And that''s the big message.</p><p>And
  the system that we looked at in the lab, the wall finder was actually quite hard
  because the number of delays was large. If you try to track where delays can enter
  the robot system they get in at very many different places. In the physical sensor,
  in the microprocessor, in the conversion from analog to digital, there''s a number
  of delays in that system. And that''s why it becomes hard to stabilize.</p><p>OK.
  So that''s the main content for today. What I want to do is give you one more practice
  question. The big problem that I want you to think about from today is how do you
  characterize performance? When we had a single pole performance was easy to talk
  about because performance was diverging monotonically, diverging alternating, converging
  monotonically, converging alternating. There were four kinds of behaviors.</p><p>When
  we went to second order we saw some new behaviors. It could become oscillatory.
  What I''d like you to do now is think not just about those properties but many other
  properties.</p><p>So here''s some questions. Think about the system on the top and
  I''d like you to infer properties about that system. In particular, does this system
  have three poles? Is the unit sample response, is there a way to write that as the
  sum of three geometric sequences? What''s the unit sample response? And is one of
  the poles that z equals 1? So think about the system, think about five ways of characterizing
  it and tell me how many of those five characterizations is correct.</p><p>So how
  many of the properties are true?</p><p>AUDIENCE: [UNINTELLIGIBLE] Probably 2/3 correct?</p><p>PROFESSOR:
  How many poles? How do you get three? Where are the poles?</p><p>AUDIENCE: [UNINTELLIGIBLE]</p><p>PROFESSOR:
  How do I find poles? What do I do? Yes?</p><p>AUDIENCE:  You use Black''s Equation
  [UNINTELLIGIBLE] the top you can express [UNINTELLIGIBLE] so use Black''s Equation
  to express the system function as R cubed over (1 minus R-cubed) then--</p><p>PROFESSOR:
  That''s right.</p><p>AUDIENCE:  --the denominator as an order of 3 and you combine
  the 3s.</p><p>PROFESSOR:  So a little more formally, we would take this thing and
  we would rewrite that with R goes to 1 over z. So we get 1 over z cubed, 1 minus
  (1 over z cubed), which is then, clearing the z cubes we would get 1 over (z cubed
  minus 1).</p><p>How many poles? Three. What are the poles of z cubed minus 1? Three
  poles in what?</p><p>AUDIENCE: 0 [UNINTELLIGIBLE]</p><p>PROFESSOR:  And so let''s
  vote. Let''s take a vote. There''s two poles at z equals 1. Yes? No?</p><p>AUDIENCE:
  [UNINTELLIGIBLE]</p><p>PROFESSOR:  Why not?</p><p>AUDIENCE: [UNINTELLIGIBLE]</p><p>PROFESSOR:
  So there''s two poles. I made a [UNINTELLIGIBLE] plane. Where''s the poles? Well,
  you could factor it, right? If you factored it you''d find that there is a pole
  at 1, right? But then there''s two more poles like that. So the poles are the three
  roots of 1, which can be written like 1 e to the j, 2pi over 3, and e to the j minus
  2pi over 3.</p><p>Which pole was the dominant pole?</p><p>AUDIENCE: [UNINTELLIGIBLE]</p><p>PROFESSOR:
  OK, bad question. What''s a better question?</p><p>AUDIENCE:  How many dominant
  poles are there?</p><p>PROFESSOR: How many dominant poles are there? That''s a much
  better question, yes. There''s sort of three poles that are equally dominant, right?
  They all have the same magnitude.</p><p>Why do we talk about dominant poles? What
  are dominant poles good for? If I told you that I had a pole at 3 and a pole at
  minus 1, which one''s the dominant pole?</p><p>AUDIENCE:  3.</p><p>PROFESSOR:  Why?</p><p>AUDIENCE:  Greater
  magnitude.</p><p>PROFESSOR: Greater magnitude. Why do we care? We don''t care, right?
  What''s good about the dominant pole? Well, we can write this response as something
  that looks like three to the n plus minus 1 to the n. If you let n get big enough
  the only one that matters is 3 to the n.</p><p>So if all you care about is exactly
  how the plane was flying the instant before it hit the ground then you would only
  need to worry about long time. And if you only worry about long time you only need
  to worry about the pole that''s worst behaved. That''s where the concept comes from.
  So none of these poles are particularly worse behaved than the others.</p><p>What''s
  the unit-sample response associated with that pole? We have a name for that [INAUDIBLE]
  right?</p><p>AUDIENCE: It''s huge.</p><p>PROFESSOR:  It''s [UNINTELLIGIBLE]. What''s
  the unit-sample response associated with this pole? Well, it''s got a complex value
  right? So the unit-sample response associated with that pole is e to the j 2 pi
  over 3 n. That''s a complex number. That''s 1 at time 0 and e to the j 2 pi over
  3n at time 1 and e to the j 4 pi over 3 at time two. So it goes from here at 0 to
  here at 1 to here at 2,3, 4, 5, 6, 7, 8.</p><p>What''s the period of this pole?
  What''s the period of the unit-sample responses associated with that pole? 3. Because
  it takes 3 to get around to where you started again.</p><p>What''s the period of
  this pole? 3. You just spin around backward.</p><p>What''s the period of the response
  associated with that pole? Bad question. All right, what''s a better question? Is
  there a period associated with it? You could say that period 1 [UNINTELLIGIBLE]
  definition of period.</p><p>What''s the period of this pole? Dumb question, right?
  Period implies repeat. If the response repeats itself after some time then we would
  say the response is periodic. Neither of those poles, well, the minus 1 is. Is the
  minus 1 pole periodic? Yes.</p><p>What''s the difference  between periodic and alternation?
  Does a [UNINTELLIGIBLE] alternate?</p><p>AUDIENCE:  Yes.</p><p>PROFESSOR: Does it
  oscillate?</p><p>AUDIENCE:  No.</p><p>PROFESSOR:  Bad question. Alternate is a word
  that we invented for one pole. Because the response alternated in sine. The unit-sample
  response in one pole, where the pole is a negative number, alternated in sine. So
  we gave that a name.</p><p>Alternation is not necessarily something that we would
  like to associate with a higher order system.</p><p>Periodic is perfectly reasonable
  to talk about for a higher order system. Periodic merely means that if y of n were
  a periodic signal that I could express y of n plus n as y of n. That would be periodic.
  If the thing repeats itself we would say it''s periodic.</p><p>So the point of going
  over this stuff is just to give you some exercise in thinking about how to think
  about properties of systems. We develop properties initially thinking about one
  pole. Those properties were easy. Converging, diverging, monotonic, alternating.</p><p>When
  we try to think about corresponding properties of higher order systems we can''t
  simply map the simple properties of first order systems into the other. We have
  to think about more complicated things. Then we think about things like dominant.
  If one of the poles has a bigger magnitude than the other then for large times we
  can ignore the smaller one.</p><p>What happens for short time? Does this response
  monotonically increase with time for all time? No. Since the response associated
  with minus 1 alternates in sine, for short times, for times with n close to 0, that
  can be just as important as this one. So the dominant pole idea tells you how things
  work when you have large times. It doesn''t necessarily tell you how things work
  when you have small times.</p><p>How about, the unit sample response is the sum
  of three geometrics. Yes or no? What are the three geometrics? And the answer to
  that''s yes. That''s very important. The three geometrics over here are this pole
  to the n plus this pole to the n plus something that goes with this other pole to
  the n. Now it''s a weighted sum but the weights are not necessarily 0.</p><p>The
  slide that I showed you for the partial fraction decomposition, you can always write
  a higher order system as a sum of first order factors. That''s the partial fraction
  expansion. That doesn''t mean the weights are all unity.</p><p>Number (2), can you
  write the unit-sample response as the sum of three geometric signals? Yes. There
  it is. And if you''re really good at complex math you could find out a, b and c.
  And that would tell you the unit-sample response and that would tell you the answer
  to (3) and (4).</p><p>Is the unit-sample response 0, 0, 0, 1, 0, 0, 0, 1, 0, 0,
  0, 1, 0, 0, 0, 1? Or 1, 0, 0, 0, 1, 1 -- whatever. Is it one of those two or something
  different? And how do you figure it out? How do you figure out the unit? Is the
  unit-sample response-- Is number (2) correct? Is the unit-sample response 0, 0,
  0, 1, 0, 0, 0, 1, 0, 0, 0, 1-- Yes? How do you know that? You could solve that equation.
  Is there an easier way? Yeah?</p><p>AUDIENCE:  I wrote it as a difference equation.</p><p>PROFESSOR:  Just
  write the difference equation. Exactly. So even though I bad-mouth difference equations
  a lot, here it''s easy. In fact, you can see it in the network. Thinking about the
  difference equation would be easy. Thinking about the network would be easy.</p><p>If
  we think about the unit-sample response of this thing started at rest, rest means
  this is 0, this is 0, and this is 0 initially. Unit-sample response means this becomes
  1 at time 0. At time 0 this is 1, this is 0, this is 0, this is 0. So if I think
  about what''s the time response look like and I did plus, this is 0, 1, 0, 0, 0.
  The first answer is 0.</p><p>Clock ticks. What happens? This is 1. This becomes
  1. This doesn''t change. That doesn''t change. This goes to 0. 0 comes around here.
  That goes to 0. So that''s the answer at time 1.</p><p>What happens at time 2? Just
  keep working it. The clock ticks, this goes to 1, this goes to 0, these stay 0,
  this stays 0. That''s the answer at time equals 2.</p><p>Now the clock ticks. Now
  this comes over to here, that means it comes back here. This is still 0. That comes
  to 1. That''s the answer for time 3. Now the clock ticks. And you can see the whole
  thing would just repeat itself now.</p><p>Is the response periodic? Yes. The response
  is periodic. What''s the period? 3. And I can see [INAUDIBLE] if the [INAUDIBLE]
  there it''s going to have be related to the period over here. These periods are
  not same. This period is 3, this period is 3, this period is 1, if you want to call
  that a period. But they are related.</p><p>OK. The point of this exercise is to
  illustrate two things. We inferred properties of first order systems by looking
  at a single pole which for a real system could only behave in one of four different
  ways.</p><p>Second order system introduced new behaviors. Now we can oscillate,
  which we couldn''t do before. Having got to oscillation, oscillation came about
  because of complex numbers. If you go to higher order systems nothing new happens
  in algebra. There''s no such thing as meta-complex numbers, right? Complex is as
  bad as it gets.</p><p>So you can have complex numbers. The higher order behaviors
  can still have complex numbers but you have to think when we ask you, what''s the
  property of a higher order system. You can think about it in terms of the individual
  parts but it requires some thinking.</p><p>OK. Good luck tonight. See you then.&nbsp;</p>'
type: course
uid: ec1daae8fe0f5dad365fb58e2a0f3def

---
None