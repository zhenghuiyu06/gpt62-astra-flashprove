# VO LOCKED — GPT-6.2 Astra / OpenAI & Anthropic
# Amy 2026-11-05 verbatim. Do not rewrite.

## S01
There's a lot of noise around GPT-6.2 Astra right now. An OpenAI benchmark, a model ID spotted in Codex, and some wild-looking SVG demos are all getting mixed together. But they aren't the same kind of evidence. So what can we actually verify? Let's separate the official updates from the rumors—and figure out what any of this means for the work you do.

## S02
Start with something OpenAI actually published. On BenchCAD 2.0, a newer internal model scored 0.875, compared with 0.594 for GPT-6 Astra at its highest reasoning setting. That's a big gap on this particular test.

## S03
And this isn't just an abstract math quiz. BenchCAD asks models to reconstruct 3D parts and assemblies and identify connections on circuit boards. If you work with CAD or hardware, you can see why that would matter.

## S04
But here's the catch: OpenAI hasn't named that internal model in the article. The score doesn't prove it's GPT-6.2 Astra, and a result on BenchCAD doesn't tell us how it performs across every engineering task. It's a strong signal from OpenAI's own test—not a hands-on review of a new public model.

## S05
So the benchmark is real, but the model behind it is still unnamed. What about the GPT-6.2 Astra name people keep seeing?

## S06
Some Codex users have shared screenshots showing a `gpt-6.2-astra` model ID in their usage breakdowns. That's interesting. But the model picker in those reports still said GPT-6 Astra.

## S07
Maybe OpenAI was testing a new model or routing some requests differently. We don't know. An ID in a usage page isn't an official release announcement, and it doesn't tell you which model produced any particular output. So for now, treat GPT-6.2 Astra as a reported sighting, not a model you can confidently select and test.

## S08
Of course, a model name only gets people so far. The visuals are what really made this rumor travel.

## S09
Clips circulating online show SVG recreations of familiar game scenes: Dust2, Nuketown, Rust, and Minecraft. And yes, the detail is fun to look at—especially if the file really uses vector paths rather than a screenshot embedded inside an SVG wrapper.

## S10
But here's the important part: a good-looking SVG doesn't tell us which model made it. The Dropday page for the Minecraft example currently credits GPT-6 Astra, and the site warns that its model credits may be inferred. We also don't have a controlled record of the prompt, retries, and source file for every example. So these are interesting visual-coding demos. They aren't proof that GPT-6.2 Astra generated them—or that it would do the same thing on your project.

## S11
And game scenes aren't the only kind of SVG being shared. One example tries something with a very different job.

## S12
A social post attributes a labeled animal-cell SVG to GPT-6.2 Astra after a short prompt. The result is eye-catching, but this is where looking impressive and being useful can part ways. Are the labels biologically correct? Can you edit the file? And can we verify which model actually produced it?

Until those questions are answered, it's a promising-looking example—not a reliable model comparison or a finished classroom diagram.

## S13
So let's leave the unverified model attribution there. OpenAI has also documented a hardware project we can examine more directly.

## S14
OpenAI says two team members worked with GPT-6 Astra on a device that lets people talk to Codex. GPT-6 helped define the functional requirements; Astra worked on the look, the enclosure, the circuit board, the interface, and the software integrations. The two-person team designed the test device in under a week as a side project. A manufacturer then built a small batch of prototypes in under a month.

## S15
That's a much more concrete story than an anonymous SVG. But the part I wouldn't skip is what happened after the design: getting it ready to manufacture still took several rounds of human review and iteration. OpenAI says Astra missed some production limits and assembly details. So yes, AI helped move a physical idea forward. No, it didn't remove the engineers from the process.

## S16
OpenAI is also testing related workflows with Chip Ganassi Racing, turning 3D scans into editable CAD models and manufacturing drawings. And it has a research collaboration with Mazda to explore vehicle designs through simulation. Those are early, reviewed projects—not proof that every engineer can hand an AI a sketch and get a production-ready product back.

## S17
From hardware prototypes to something closer to your everyday workflow: OpenAI also updated ChatGPT Images.

## S18
OpenAI just introduced ChatGPT Images 2.6. The obvious new trick is looping GIFs: describe what should move, or upload a still image and ask ChatGPT to animate it. You can adjust the playback speed and share the result. That could be useful for a quick social graphic—but GIF creation is still rolling out, so it may not be on your account yet.

## S19
The quieter feature might save more time: saved reference photos. Name a photo once, then call it back in a later chat with an @ mention. If you keep making images of the same character or product, that's one less thing to re-upload.

## S20
OpenAI says Images 2.6 also generates faster and keeps details more consistent across edits. Change the background, and the character's outfit should stay put. Sounds useful. But we'd still need to see how it holds up across a real project, not just a single demo.

## S21
That's an official product update. But here's a different trust problem: if a third-party provider says it's running a premium model, how would you know? Anthropic has been working on a way to check.

## S22
Anthropic has released FlashProve, an open-source research prototype built around a surprisingly simple question: did this answer actually come from the model you paid for?

## S23
Imagine a third-party service tells you it's using a premium model, but quietly routes your request to something cheaper. You can't tell just by reading a good answer. FlashProve aims to give the provider a way to attach a cryptographic proof that the response came from a committed set of model weights, without revealing those weights.

## S24
The numbers are striking. In Anthropic's test on Llama 4 Maverick, a 400-billion-parameter mixture-of-experts model, one H100 GPU generated proofs at about 110 tokens per second. Each proof was roughly 19 megabytes for a 1,024-token request. An earlier system, VerInf, reported a 93.6-gigabyte proof for the same model and took almost a day to verify it.

## S25
Claude helped improve the proof system, and Anthropic published code and Lean proofs for its top-level security claims. That's real research you can inspect. But FlashProve is still a prototype. Producing the proofs takes much more compute than ordinary inference, and the current setup has limits on model type, decoding, and context length. It also proves which committed computation produced the tokens—not whether the answer is correct.

## S26
So this won't suddenly put a “verified model” badge on every AI response. But it is a serious step toward checking a claim that today we're mostly asked to take on trust.

## S27
So here's the thread running through all of this. OpenAI's internal engineering score is documented, but the model isn't named. The GPT-6.2 Astra sightings and SVGs are interesting, but their attribution still needs proof. The hardware work shows useful progress with engineers in the loop. Images 2.6 gives creators new tools to try. And FlashProve asks whether we can verify the model behind an answer at all.

The next big AI story won't be decided by the wildest demo. It'll be decided by what we can check—and by what actually helps you finish the work.
