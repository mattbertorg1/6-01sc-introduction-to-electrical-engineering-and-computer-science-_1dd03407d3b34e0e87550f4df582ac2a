---
about_this_resource_text: ''
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
embedded_media:
- id: Video-YouTube-Stream
  media_location: sNLB6_ZIfX0
  parent_uid: 318bfd15daa7da712fcadc365bcf72d1
  title: Video-YouTube-Stream
  type: Video
  uid: 29890ac4fed87c60789fba85feee1410
- id: Video-iTunesU-MP4
  media_location: http://itunes.apple.com/us/itunes-u/recitation-11-op-amps/id490181666?i=108667925
  parent_uid: 318bfd15daa7da712fcadc365bcf72d1
  title: Video-iTunes U-MP4
  type: Video
  uid: a2474974da39debac4c5250131d8fa22
- id: Video-InternetArchive-MP4
  media_location: http://www.archive.org/download/MIT6.01SCS11/MIT6_01SC_rec11_300k.mp4
  parent_uid: 318bfd15daa7da712fcadc365bcf72d1
  title: Video-Internet Archive-MP4
  type: Video
  uid: 7dd79061160ef875d12f5b0a93c20b00
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/sNLB6_ZIfX0/default.jpg
  parent_uid: 318bfd15daa7da712fcadc365bcf72d1
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: fc8a0fed20f30655ca22699daed87455
- id: MIT6_01SC_rec11_300k.srt
  parent_uid: 318bfd15daa7da712fcadc365bcf72d1
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/op-amps/recitation-1-object-oriented-programming/MIT6_01SC_rec11_300k.srt
  title: MIT6_01SC_rec11_300k.srt
  type: null
  uid: 268de70e643aac214e3e4348f4138883
- id: Caption-OCW-SRT
  parent_uid: 318bfd15daa7da712fcadc365bcf72d1
  title: Caption-OCW-SRT-English - US
  type: Caption
  uid: bad9b1abe347d1460eda33137c46b6c0
- id: MIT6_01SC_rec11_300k.pdf
  parent_uid: 318bfd15daa7da712fcadc365bcf72d1
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/op-amps/recitation-1-object-oriented-programming/MIT6_01SC_rec11_300k.pdf
  title: 'MIT 6.01SC S11 Recitation 11: Op-Amps Transcript'
  type: null
  uid: 253fc70fbdcf8bbc336c98315e27447f
- id: Transcript-OCW-PDF
  parent_uid: 318bfd15daa7da712fcadc365bcf72d1
  title: Transcript-OCW-PDF-English - US
  type: Transcript
  uid: b72f4bb698bb04db42608e9f429d8da1
inline_embed_id: 45982868recitation11:op-amps45578431
layout: video
order_index: null
parent_uid: 6912b6f0dfbf7463fa378df8bde18e96
related_resources_text: ''
short_url: recitation-1-object-oriented-programming
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/unit-3-circuits/op-amps/recitation-1-object-oriented-programming
template_type: popup
title: 'Recitation 11: Op-Amps'
transcript: '<p>PROFESSOR: Hi. Last time we talked about NVCC method and how to reduce
  the number of equations we had to deal with to solve a particular circuit. At this
  point, we''re pretty well equipped to solve circuits in the general sense, but we
  really haven''t talked about how to use that information or possibly use circuits
  in a particular way.</p><p>Before we jump into both that and abstraction of circuits,
  we need to talk about op-amps. Op-amps is short for Operational Amplifier. And it''s
  a tool that we can use in order to sample particular voltages from a subsection
  of the circuit without affecting it.</p><p>Another thing we can use op-amps to do
  is modify our signal. Or if we''re going to sample a voltage from a particular subsection
  of the circuit, we can then do stuff to that voltage without affecting the circuit,
  all within the op-amp or within the op-amp''s special subset of circuitry.</p><p>So
  first of all what is an operational amplifier? Well, an operational amplifier is
  a giant web of transistors. But what an operational amplifier does is act as a voltage-dependent
  voltage source.</p><p>It can effectively sample voltages from an existing circuit
  and then use them to power some other object, for instance a light bulb. If you
  set up this kind of circuit, you will not actually be powering this light bulb with
  5 Volts, because the light bulb itself acts as a resistor. And so the voltage drop
  across this part of the circuit is going to be different from just 5 Volts.</p><p>If
  you want to enable a voltage drop of 5 Volts across this light bulb, then you have
  to stick up an op-amp. You have to use an op-amp to sample the voltage drop at this
  component and put it in between the light bulb and the rest of the circuit.</p><p>When
  you see an op-amp on a schematic diagram, it''ll frequently look like this. You''ll
  have a positive input voltage, a negative input voltage, power rails, which are
  actually the thing that determine the range of expressivity that the op-amp has,
  and an output voltage. In reality, the relationship between the output voltage and
  then input voltages is something like this, where K is a very large number.</p><p>The
  effect that this has is that Vout is going to be whatever Vout needs to be, such
  that Vplus is equal to Vminus. That''s the basic rule you want to use when you''re
  interacting with op-amps. So in this case, if we wanted to power this light bulb
  with 5 Volts, we would do something like this. Excuse the sloppiness of the second
  diagram.</p><p>We still have our 10 Volt voltage source. We still have our voltage
  divider. This point samples 5 Volts from this sub-circuit -- and isolates this part
  of the circuit from the light bulb.</p><p>Vout has to be whatever value is necessary
  such that this sample point and this sample point are equal. Since this value is
  5 Volts, this value will also be driven to 5 Volts by the op-amp, which means that
  this value is 5 Volts. And we''ve successfully managed to power a light bulb with
  5 Volts.</p><p>The other thing you might be asked to do is to take an existing schematic,
  an existing circuit diagram and figure out what the operational amplifier does to
  a given signal or possibly what Vout is or possibly what Vout is in terms of the
  input signal. So let''s practice using this diagram.</p><p>Here''s what we''re after.
  I''m going to figure out where Vplus is going to be. This is another voltage divider.</p><p>I''m
  now interested in Vminus, in terms of Vout, which is another voltage divider. I
  can set these two equations equal to one another and solve for Vout.</p><p>I found
  a new expression for Vout in the particular case where V is 10 Volts. If my input
  voltage were previously unspecified, or if this voltage source were not specified
  or just Vin, then I would be after this expression.</p><p>Some things I''d like
  to mention, while we''re talking about op-amps, all the operational amplifiers we''ve
  been working with so far deal with Vout in terms of Vin, where Vin is driven through
  the positive terminal, and the negative terminal is typically connected to ground.
  You can do the opposite and end up with some interesting effects. But it comes at
  a cost. It is entirely possible that you will end up driving your op-amp to an unstable
  equilibrium.</p><p>What you need to look at is this relationship. There may be a
  particular point, in which case your system is stable. But if you get any sort of
  minor perturbations, you''ll actually end up with divergence. If this is the case,
  then you''ll probably burn out your op-amp. You can do this by hooking it up in
  this way. This is expensive and could possibly burn you.</p><p>The other thing to
  note is that the power rails on your op-amp limit its range of expressivity. And
  I think I''ve said this before, but it''s worth mentioning again. If your op-amp
  is only powered by 10 Volts, it cannot amplify your input signal to a final value
  greater than 10 Volts. Likewise, if your input value is a negative voltage, and
  you''re working with a non-inverting amplifier, if your ground is truly ground or
  if your ground is higher relative than your input voltage, you cannot actually express
  a negative voltage.</p><p>The third thing I''d like to quickly mention is that there
  are some terms associated with op-amps that you might hear used by the staff or
  online, that sort of thing. A buffer and a voltage follower are the same thing.
  And that''s explicitly when you want to sample a signal or you want to sample a
  particular voltage, and you don''t want to multiply it or add it to something or
  do any kind of LTI operations that we might be able to do using op-amps in this
  course.</p><p>You can work with amplifiers. And the thing we worked with earlier
  was an amplifier for a value less than 1. You can also use op-amps to some signals.
  And if you look for a voltage summer amplifier on the internet, you should be able
  to find some information.</p><p>In any case, op-amps are really powerful. They allow
  us to both isolate a particular section of a circuit and sample a particular voltage
  value from that circuit without affecting that circuit, and also allow us to modify
  that particular voltage value before using it in another part of our overall circuit.
  Therefore, we''re enabled to design more complicated and powerful things.</p><p>Next
  time, I''ll talk about superposition and Thevenin Norton equivalence, which will
  further enable modularity and abstraction in our circuit design. &nbsp;</p>'
type: course
uid: 318bfd15daa7da712fcadc365bcf72d1

---
None