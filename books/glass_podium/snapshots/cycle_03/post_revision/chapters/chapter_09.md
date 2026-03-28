# Chapter 9

Yusuf talked to himself when he worked. It wasn't the self-conscious muttering of someone performing eccentricity, just a steady half-voiced account of whatever his hands were doing, so constant it barely registered as speech anymore. It came in fragments of logic and technical shorthand, with the occasional "right" serving as both punctuation and encouragement. The calibration bay at two in the morning was the only place it didn't sound odd. Diagnostic terminals threw blue-white light across his face, the desk, and the paper cup he had filled three hours earlier from the corridor machine, the espresso inside gone cold enough to leave a bitter film at the back of his tongue.

Three displays held three versions of the same problem. On the left, captured handshake traffic from infected calibration sessions, athlete names stripped out but not the body data. In the center, Meridian's patch package from the afternoon meeting sat sealed and proprietary, asking for permanent read-write privileges across every enhancement system in the building. On the right, Yusuf's own map of the handshake sequence crawled with notes built from reverse-engineered logs, public documentation, and six years of remembering which parts of Meridian firmware always behaved differently from the brochure.

He flexed his fingers once, set them back on the keyboard, and told the empty room what he was about to try.

"Right. Upstream first. Small cut. No heroics."

The first interception point sat just above sensory routing, early enough to catch the payload before it could write itself into the live enhancement stack. On replay the foreign block hit his hook, stalled there, and vanished into the sandbox partition he had built an hour earlier. Good. A line of numbers populated underneath.

`sensor queue delay: 84ms`

"Eighty-four? No. No, that's vile."

He took out two logging calls, moved a checksum audit to a lower priority thread, and ran the same replay again.

`sensor queue delay: 41ms`

It was better, but still ugly. Forty-one milliseconds was not abstract at sprint speed. It was a step landing a fraction behind the body's confidence. It was a hurdler seeing the barrier where it had been rather than where it was. It was a swimmer feeling the wall a breath too late and twisting through the turn with one shoulder not quite under her. Costly, certainly. It was not automatically catastrophic.

He pushed the sim harder. A preserved sprint session ran through the patched handshake. The digital skeleton on screen drove cleanly through acceleration, then showed a slight smear at maximal cadence, the knees coming up on time but the upper body adjusting a beat late, as if the head and shoulders had needed persuading. There was no collapse and no blind panic, just a body no longer quite first with itself.

Another replay pulled up a turn sequence from the aquatic calibration bank, stripped of everything except force curves and joint timing. The virtual swimmer reached for the wall and caught it half a hand-width short, fingers skidding before the palm found tile. It was enough to bruise ribs on a bad day, not enough to drown anyone by itself.

"All right. You'd hate it, but you'd stay in one piece."

The second interception point lived deeper, down near the autonomous motor governor where the virus seemed to preserve its own path. There the numbers looked cleaner immediately.

`sensor queue delay: 6ms`

"That's more like it."

For about half a second it was. Then the stumble-recovery routine flashed yellow.

`assistive catch protocol: unavailable`

Silence held in the bay long enough for him to hear the fluorescent tube nearest the windows buzz on its bad ballast.

A balance-failure sim loaded under his fingers: full sprint, wet-surface coefficient, lateral displacement introduced at the left ankle. In the replay the runner clipped into instability and pitched forward. No recovery pulse came through, and no throttle cut the synthetic force. The ankle over-rotated, the knee kept driving, and the body went down with the smooth inevitability of a machine following instructions that no longer deserved obedience. In the frame after impact the lower leg sat at the wrong angle. In the frame after that the torso kept trying to move.

Yusuf took his hands off the keyboard.

That layer was what caught a body when its owner clipped a hurdle, misjudged a turn, hit a wet tile, lost half a step. It was the thing that kept a stumble from becoming shredded ligaments and bone through skin. He could tell an athlete the first patch would slow them. He could not tell them the second one would probably let them keep their times while removing the piece that stopped them breaking themselves open.

For a moment Farah crossed his mind anyway, not her face but her hands on the video call last month, trying to fasten a cuff and missing the button twice because the fine control went on her without warning now. If Meridian owned every stream outright, the early deterioration patterns in people like her would disappear into licensing language and quarterly strategy decks. He pulled his attention back before that thought could turn into permission.

"First one, then. Ugly but honest."

He went upstream again, widened the quarantine lane, and blocked reintegration. The payload went into the sandbox and stayed there when he replayed variant twenty-nine. Variant thirty passed. Variant thirty-one passed. Variant thirty-two passed after he tightened a validation check that had been too generous by one packet header. The next run broke something else.

`coach link: connection refused`

He stared at it, then swore softly and opened a fresh branch.

The coaching feed used the same bidirectional lane the virus used. Of course it did. Meridian had built the whole ecosystem to prefer openness when the openness enriched them. Margot's interface was only the most obvious example. Live biomechanical correction, external pacing, remote override permissions in narrowly defined circumstances, post-session telemetry sync, all of it depended on a handshake that treated the body as a system endpoint first and a person second.

"Fine. Mirror only."

He built a one-way relay that preserved outbound metrics and stripped inbound write privileges. The relay held for a moment, enough to make him lean closer. Then the payload rode back in on the callback the coaching stack still expected for acknowledgement.

`coach mirror: compromised`
`ingress source: remote callback`

"Dirty little bastard."

He killed the relay, opened a read-only metrics export, and tried again. This time no malicious block came through. This time no coaching data came through either, not in any way a live session could use.

`coach link: unavailable`
`telemetry export: delayed batch only`

Which was the same answer with better manners. Athletes could take his patch and keep ownership of their bodies, or they could keep the real-time tools half the building had started treating like an extra limb. At the moment he did not know how to offer both.

The matrix on the right-hand screen filled slowly as he worked.

`mapped variants: 34/47`
`stable quarantine: 28`
`stable quarantine + intact catch protocols: 19`
`stable quarantine + coach continuity: 0`

Nineteen was not nothing. Nineteen was also not the kind of number a sane man put near a live nervous system.

He forced himself through three more runs anyway. Variant thirty-three threw a checksum mismatch that traced back to a routing exception he had introduced an hour earlier and forgotten. Variant thirty-four passed on rerun. Variant thirty-five made the latency wobble between thirty-eight and forty-three milliseconds depending on how aggressively the sim loaded proprioceptive feedback. It was good enough to stay on screen and bad enough to leave his jaw sore from clenching.

Across the room the bay clock changed to 02:41.

He saved the current patch branch to the facility environment under the label Maintenance tooling update, buried inside the calibration utilities under a name no one would notice unless they were already suspicious. The second save went to the encrypted archive on the personal device in his quarters. It took a fraction longer there because the archive rekeyed every time he touched it. He watched the progress bar finish and hated the part of himself that always relaxed a little when the private copy existed.

"Enough for tonight," he said.

It was not enough. The center screen still held Meridian's sealed package like a locked door. On instinct he opened the virus code instead.

---

As always now, he started with the damage pattern.

A copy of the payload went into the sandbox. A preserved handshake replay followed it. On the output pane, vision dropped to null first. Hearing followed. Proprioception jittered, fragmented, then went dark in irregular blocks, not all at once but fast enough that a body would feel itself vanish in pieces. The motor governor stayed green throughout.

At the bottom of the screen a skeletal runner kept moving, knees lifting, arms driving, head steady, while every sensory pane above it stayed blank.

Yusuf felt his shoulders lock. Kai had hit a wall with his legs still driving.

"Designed," he said, and hated hearing the word out loud.

He tagged the governor output and reran the trace. Vision null. Hearing null. Proprioception gone in blocks. Motor path untouched. Assistive routines untouched. The bite pattern never wandered.

He ran the payload through a second replay, a lower-speed balance drill rather than a sprint. The order stayed the same. The bite pattern stayed the same. Sensory channels were stripped out while motor channels were spared. Then he ran a third, because repetition was the only honest way to trust a result, and it came back the same again.

Compiled output replaced the functional view, with the virus on the left and standard Meridian calibration firmware on the right. They shared the same processor target, the same file-size class, and the same hex density across the middle blocks. He ran an allocation scan and watched the histograms populate at the same block sizes: 64, 128, 256.

The same block sizes repeated on both sides of the screen, along with the same alignment boundaries and the same padding after control structures. He ran the scan again because the first result landed in him like a dirty joke, then pulled up an archived Meridian patch from last quarter and ran that one through the same analysis just to make sure fatigue had not made him credulous.

It was the same family of patterns. Not identical, not enough for courtroom certainty, but close in the way related tools were close. It carried a specific compiler habit and a preference for neat block alignment even where efficiency did not require it. Someone had taught the code how to stand.

His coffee had gone cold enough to grow a skin on top. He reached for it anyway, took one swallow, and put it back down untouched after that. The bitterness turned his mouth dry.

He went to exception tables next. The virus carried the same nested error hierarchy Meridian liked, too tidy for most independent shops and too fussy for the black-market clone kits he had spent years cleaning up after. It used the standard overflow routine, the same fallback that kept the system live long enough to write its own autopsy, and the same mildly sanctimonious logging stamp that Meridian engineers claimed was for patient safety and everyone else knew was for liability.

"Bollocks."

Stopping there would have been cowardice. Similarity was not proof. Similarity was how smart people embarrassed themselves in public. He opened a public toolchain sample, then an older non-Meridian firmware package from a facility partner, and checked their allocator behavior against the virus. Both diverged quickly, with different padding, different exception depth, and different memory-cleanup habits. That still was not proof, but it tightened the circle.

He opened the string table. The first entry was a generic library path, useless. The second was a standard debug call, just as useless. A third path surfaced halfway down.

`/mbio/dev/tools/nlink/`

His stool struck the cabinet behind him before he realized he had pushed back from the desk.

mbio meant Meridian BioSystems.

nlink meant neural link.

The fluorescent tube near the window buzzed again. Yusuf looked away from the path, then back, as if the extra second might turn it into something less obvious. It did not. The string sat there with the flat confidence of something never meant for outside eyes.

He opened a notes pane and typed what he could defend if anyone ever demanded the chain of reasoning.

String table contains a Meridian dev path.
Exception hierarchy is consistent with current calibration firmware.
Allocator profile is consistent with recent Meridian builds.
Public and partner toolchains do not match the same pattern family.

The first line was easy. The last was easy enough. `Meridian` in the second and third lines gave him pause. He deleted it once, replaced it with `vendor`, stared at the evasion for a breath, then put `Meridian` back. The path was still there. The exception handling still matched. The memory pattern still matched. A stolen toolchain could leave those marks. So could a planted breadcrumb. So could an internal build nobody had scrubbed properly. Years of engineering had taught him the discipline of stopping just before the claim you wanted and writing down only the claim you could keep.

To test his own caution, he pulled a March Meridian hotfix from the facility archive, one of the builds that had briefly broken a calibration scheduler in two training bays before the vendor rolled it back and called the fault site-specific. It carried the same logging stamp and the same pointer-advance quirk in the overflow fallback, eight bytes where any sensible team would have used four. The virus had that quirk too. He swore again, more softly this time.

There was no accusation yet and no grand theory. What he had was structural resemblance strong enough to be frightening and weak enough to be deniable.

He opened a fresh note beneath the byte-level comparison and typed the order instead of trying to argue with it.

`broader data-rights push`
`virus outbreak`
`sealed patch demanding permanent access to live streams`

He read the three lines twice. Still filthy. The toolchain habits could be stolen. They could be planted. The sequence did not get cleaner.

The private archive received the byte-level analysis. The facility environment did not. Whatever sweep Meridian's audit tools ran across the network next week, he did not intend to hand them his own suspicions wrapped and labelled. When the save finished, the virus windows disappeared and the patch came back full-screen.

For a long minute he just looked at it. Thirty-four variants were mapped. Nineteen preserved stumble recovery. None preserved live coaching. It was enough to tempt him and not enough to forgive him if he was wrong.

Variant thirty-five was still waiting, the simulated body frozen mid-stride on the right-hand monitor. He keyed the next run in by hand because his fingers needed work more than his mind needed another thought.

The bay door opened at quarter past three.

Yusuf did not turn at first. Technicians crossed the calibration wing at every hour, and the room had enough entry points that a door opening usually meant nothing. These footsteps stopped instead of passing. Someone stood there without speaking.

"Dr. Qadir."

He turned.

Petra Engel stood in the doorway with her clinic coat still on over a grey jumper. Her hair, usually pinned into submission, had come loose on one side. She carried a paper cup from the corridor machine and looked as though she had been awake on principle rather than by choice.

"Dr. Engel. Bit late."

His own voice gave him away. He heard the Birmingham flatten out as soon as he spoke, the professional register locking over the sentence and squeezing the Birmingham out of it.

"I've been reviewing facility access logs for the past week," Petra said. "Routine audit, given the circumstances."

"Sure."

"Your badge accessed this bay at eleven forty-seven tonight. It is now three fifteen. You have no calibration sessions scheduled before eight."

"Sometimes I work late. You know how it is."

"I do."

She crossed to the secondary station and looked at the displays without asking permission. He did not minimize anything. The virus windows were gone. The patch remained, dense enough to be obviously real and incomplete enough to be dangerous.

"This is not a standard calibration tool," she said.

"No."

"What is it?"

"An alternative approach to the virus. I'm seeing whether I can block propagation without handing Meridian full access to every live system in the building."

Petra set her cup down and stayed standing.

"On your own," she said. "Without authorization. On facility hardware."

"Yes."

"Show me the failure modes."

That made him look up properly.

"Not the summary," she said. "The failures."

Something in him loosened a notch at the specificity. He rotated the center monitor toward her and pulled up the comparison table. Upstream intercept on the left. Deep intercept on the right. Latency traces under both. A cluster of test replays stacked beneath them.

"This branch catches the payload before it can write into the live enhancement stack," he said. "Forty to forty-three milliseconds of sensory delay depending on the load. Stumble recovery stays intact. Coach link dies."

"And the other."

"Six milliseconds. Almost clean. But it drops the assistive catch protocol."

"Run it."

He ran the deeper branch. The balance-failure sim loaded, the runner clipped off-center, and the body folded with that terrible smoothness again, no corrective pulse, no reduction in synthetic force, just joint after joint obeying the last instruction it had been given until the screen model landed in a collapsed knot that would have been torn tissue and fractured bone in real life.

Petra did not flinch. She just leaned closer.

"Again," she said.

This time the upstream branch. Same destabilization. Same displaced ankle. The body lurched, recovered badly, and kept moving with a visible hesitation, the torso correcting after the legs rather than with them.

"Forty-one milliseconds," she said, reading the trace. "That is a long time in a lane."

"Yes."

"But this one keeps the protective routine."

"Yes."

"And the coaching interface."

"Gone."

He brought up the relay attempt and the failed mirror with the callback compromise. Petra read the lines in silence.

`coach mirror: compromised`
`ingress source: remote callback`

"So any live coaching channel is also a route back in," she said.

"Through the present handshake, yes."

"Can you separate them?"

"Not tonight."

"Can Meridian?"

"Meridian can do whatever Meridian's sealed package actually does. They've not shown us."

That earned him a brief look, tired and sharp at once.

"You have not run this on a person."

"No. Replays only."

"Good."

Only then did she sit on the stool beside the station. Her movements stayed measured even now, but tiredness had started to show through them as something physical rather than temperamental, a slight care in the wrists, the caution of someone whose body had been awake too long and knew it.

"Is this the only unauthorized work you have been doing in this bay?" she asked.

The question landed with enough precision that lying to it would have been insulting. A flinch crossed his face before he could stop it. Petra caught it.

"I've also been running additional analysis on the virus code," he said. The vowels tidied themselves further. "The standard diagnostic approach is not getting all of it."

"The access logs show you have been here after hours on eleven of the last fourteen nights," she said. "Including nights before the virus was formally identified."

He could explain that. The anomaly tracking, the weeks of tiny mismatches, the small failures that had started before anyone called it infection. The explanation was true. It also opened the wrong door and kept opening it.

"I was concerned about network anomalies before the formal diagnosis," he said. "The virus confirmed the pattern."

"And the transfers to an unregistered device?"

His hands went still on the desk.

"System logs show small encrypted exports from this station," Petra said. "Regular. Off-book. IT security is busy with the outbreak, the delegation, and everything else that is currently on fire. They have not followed the trail yet. They will."

Yusuf pushed his glasses up his nose. The gesture bought him half a second and nothing useful arrived in it.

"I've been backing up biological calibration data," he said. "Athlete biometrics. More than my job covers."

"Why?"

Redundancy. Network stability. Data integrity. All the stupid little lies presented themselves in a queue. Petra had not come down here at three in the morning for any of them.

"Some of it's — look, the calibration data has neurological applications that aren't being pursued. Degenerative disease work." He heard himself stalling in the technical language and pushed through it. "My sister's got Voss-Kessler. It's progressive and Meridian doesn't give a shit because there's no product in it. The data's already sitting there. Once that contract locks everything down, nobody outside them gets near it."

Petra said nothing for long enough that the server fans took over the room.

"How much data?" she asked.

"Enough to matter. Not enough."

"Identified?"

"In the archive, yes."

Her mouth tightened, not in surprise. In calculation.

"There was a decathlete at the Stuttgart facility," she said. She picked up the cup, found it empty, and set it back down again. "Marius Koch. He was twenty-four."

Yusuf kept quiet.

"His body started rejecting the synthetic grafts. Immune cascade, inflammatory markers climbing, organ involvement beginning before anyone stopped calling it calibration variance." She corrected herself: "Before I stopped calling it that. I let the classification stand for eleven days before I escalated. I should have been faster."

She was looking at the code on his center screen rather than at him.

"I wrote three reports. Recommended immediate removal. The facility director agreed with me — forwarded everything to Meridian medical oversight with his own recommendation attached." She paused. "Meridian reclassified the rejection as within acceptable parameters. Told us to keep him training while they monitored."

"What happened?"

"He died. Eight months later." Petra turned the empty cup once between her palms. "Organ failure. His body had been in active rejection the entire time they kept him training."

Something old and exhausted moved across Yusuf's chest. Not sympathy exactly. Recognition. The institutional kind.

"I filed a complaint," Petra said. "The investigation found — protocols had been followed. Technically they had been. Right forms, right intervals, right language." She stopped. "I kept waiting for someone to ask whether the protocols were even designed to catch what happened to him. Nobody did."

He looked at his hands because there was nowhere useful to put his eyes.

"I'm not telling you this so you'll feel sorry for me," she said.

"I know."

"Good."

She leaned toward the screen again and tapped the latency table with one finger.

"This matters," she said. "Forty-one milliseconds. Protective routines intact. Coaching link dead. The other branch is faster and it drops the safety catch." She was quiet a moment. "Nobody else has shown me anything like this. It's been Meridian's sealed package or — people in meetings talking about liability."

"And this," he said.

"And this. Which at least tells me what the tradeoff is."

"I should report you," she said. "If security audits this bay and finds out I stood here — saw unauthorized exports, unsanctioned firmware work during an outbreak — and said nothing, then I'm part of it. Best case I lose this post. Worst case it's my license."

Now he looked at her.

"I'm not going to report you tonight." She said it without looking away. "Not because I — I don't know what your motives are. I'm not pretending the archive isn't a problem." She let out a breath. "Meridian wants permanent data access across every system in this building. And you're the only person who's shown me what the alternative costs. Those are the two things I'm weighing."

The bay hummed around them. Somewhere in the corridor a trolley wheel rattled over a seam in the floor and passed on.

"There are conditions," she said.

"All right."

"You don't put this on an athlete. Not one. If you get to the point where you think it's clinically ready, you bring me the full latency table, the fall-recovery data, every failure case. I review it before it goes near a live system."

"Understood."

"If you go around me, I report everything."

"Understood."

"Second. I don't want details of your archive unless they become clinically relevant. Names especially. You're in enough trouble already and I don't intend to make it worse."

"That's generous."

"It's containment," Petra said.

That almost made him laugh. It came out instead as breath through his nose, too tired to qualify as anything.

"The transfer logs will be audited," she said. "Two weeks, two months — I can't say when. But they will be. You should think about what you're keeping, what you're moving, and what holds up when someone actually looks."

"You make that sound cheerful."

"I'm not trying to."

Fair enough.

Petra stood. For a second he thought the conversation was over. Then she paused, eyes settling not on him but on the notes pane still open on the left-hand screen, the one where his virus analysis sat in plain text because he had been too tired to close it.

String table contains Meridian dev path.
Exception hierarchy consistent with current calibration firmware.
Allocator profile consistent with recent Meridian builds.
Public and partner toolchains do not match the same pattern family.

"Is that what I think it is?" she asked.

Every sensible response arrived late. He chose the least stupid one.

"It's what I can justify so far."

"Not what you believe."

"Belief's cheap."

Petra read the lines again. "And your justification is?"

"Structural signatures. Toolchain behavior. A dev path that should never have been in a stripped build. Enough to be ugly. Not enough to survive accusation."

"Do you think the virus is deliberate?"

He looked back at the screens. The skeletal runner remained frozen mid-stride from the last sim, one foot off the ground, waiting for an instruction that had not yet come.

"I think it behaves like something that was built by people who understood exactly what they were leaving intact."

Petra absorbed that without visible reaction. When she spoke again, the hedging in her voice had gone.

"Then keep that analysis off the network. All of it. You don't have evidence — you have resemblance. If Meridian's legal team sees those notes before you've got something reproducible, something independent, they will call it defamation." She paused. "And if you're right and they find out you know, you've told them what to scrub."

"That's the current plan."

"Good. At least one of us is planning."

She picked up the paper cup and moved toward the door. Her hand found the plate and stayed there a moment.

"If this shows clinical promise," she said, still facing the corridor, "I want to see the data before it goes near anyone. I'm asking as a physician. Not as the medical director."

"All right."

"And Yusuf."

"Yeah?"

Only then did she look back.

"Don't assume that being useful to me makes you safe."

"I won't," he said.

Petra gave a short nod.

"Good night, Dr. Qadir."

"Night."

The door shut. Machine hum filled the space she had occupied, then the smaller sounds returned beneath it: fans, relays, the low electric hiss of the displays. Yusuf sat still long enough to feel how hard his heartbeat had been working under the whole conversation.

On the center screen the patch matrix waited where he had left it.

`mapped variants: 34/47`
`stable quarantine + intact catch protocols: 19`
`coach continuity: 0`

In a few hours the building would wake and start asking bodies to trust the same handshake again.

No miraculous new answer had appeared while Petra was in the room. Variant thirty-five still sat at forty-one milliseconds, catch protocols intact, coach channel dead.

He reopened variant thirty-five and then, on a sour impulse, duplicated the branch into thirty-six with a note to strip the callback acknowledgement one layer earlier. Probably pointless. Possibly not. The kind of thing a tired engineer did because the hands could keep moving after judgment had started to fray.

Outside the windows the mountains had begun to separate from the dark, ridges emerging one by one as if someone were rubbing charcoal off the horizon with a thumb. The room looked worse in that light. Cables. Coffee rings. His own reflection floating over the monitor, glasses catching terminal glare, shoulders narrower than he remembered from a few years ago.

He keyed in the new run.

The replay hit the hook, hesitated, and spilled a fresh column of latency numbers down the pane.

`latency: 39ms`
`catch protocol: intact`
`coach callback: rejected`

Yusuf leaned closer and swore under his breath.
