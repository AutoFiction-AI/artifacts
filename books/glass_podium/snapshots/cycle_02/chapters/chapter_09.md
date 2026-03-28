# Chapter 9

Yusuf talked to himself when he worked. Not the self-conscious muttering of someone performing eccentricity, just a steady half-voiced account of what his hands were doing, so constant it barely registered as speech anymore. Fragments of logic. Technical shorthand. The occasional "right" that worked as both punctuation and encouragement. The calibration bay at two in the morning was the one place it did not matter. The diagnostic terminals threw blue-white light across his face, the desk, and the cold coffee he had poured three hours ago from the corridor machine, which produced an espresso so bitter it felt personal.

Three displays, three versions of the same problem. On the left, captured handshake traffic from infected calibration sessions, athlete names stripped out but not the body data. In the center, Meridian's patch package sat sealed and proprietary, asking for permanent read-write privileges across every enhancement system in the building. On the right, Yusuf's own map of the handshake sequence crawled with notes built from reverse-engineered logs, public documentation, and six years of remembering which parts of Meridian firmware always behaved differently from the brochure.

"Right. You open for twelve milliseconds. That's enough."

He dropped a hook into the first interception point, just above sensory routing, and ran a replay. The payload hit the hook, stalled, and disappeared into the sandbox partition he had built an hour earlier. Good. Then the latency trace populated beneath it.

`sensor queue delay: 84ms`

"Eighty-four? No. No, that's disgusting."

He stripped out two logging calls, reran the replay, and watched the number fall.

`sensor queue delay: 41ms`

Still bad. Still survivable. A sprinter would feel it as a slur between track and body. A swimmer would hit the wall a fraction later than the body wanted to. It would cost them. It would not, on its own, put them through a wall headfirst.

He moved the hook to the second interception point, deeper in the firmware near the autonomous motor governor. Same replay. Same payload. This time the latency trace stayed almost clean.

`sensor queue delay: 6ms`

"That's more like it."

Then the stumble-recovery routine flashed yellow.

`assistive catch protocol: unavailable`

He loaded a balance-failure sim from the diagnostics menu and kicked the virtual runner off-center at full sprint. The body on screen pitched forward. No recovery pulse. No throttle on synthetic force. The right ankle over-rotated, the knee kept driving, and the model went down in a tangle of impossible angles.

Yusuf took his hands off the keyboard. That layer was what caught a body when its owner clipped a hurdle, misjudged a turn, hit a wet tile, lost half a step. He could tell an athlete that the first patch would slow them. He could not tell them the second one would probably let them stay upright.

Farah passed through his mind anyway. Not her face. Her hands trying to button a cuff last month on the video call, the pause before the second attempt. If Meridian owned these streams outright, the early deterioration patterns in people like her would vanish into licensing language and quarterly strategy decks. He pulled his mind back to the screen before that thought could turn into an excuse.

"First one, then. Ugly but honest."

He reopened the upstream hook and started building around it. Payload diverted. Handshake quarantined. Infected module denied reintegration and dumped into the sandbox partition. He fed the patch a second handshake variant, then a third. Variant thirty-two passed. Variant thirty-three threw a checksum mismatch that made him swear aloud, fix a routing exception, and start again. Thirty-three passed on the rerun. Thirty-four passed, then broke a second test window he had almost forgotten he left open.

`coach link: connection refused`

He stared at it.

Of course. The feed interface relied on the same bidirectional channel the virus used. Close the open lane, and Margot's coaching rig got shut out too. He ran the test a second time, because some part of him wanted the machine to admit it had made a stupid mistake. Same refusal. No feed. No elegant compromise. If athletes took his patch instead of Meridian's, they kept ownership of their body data and lost a tool half the facility had started treating like a limb.

He saved the patch work twice: once to the facility environment, disguised as maintenance on calibration tooling, and once to the encrypted archive on his personal device in his quarters. The second save took a fraction longer. He watched the progress bar finish and did not move.

"Enough for tonight," he said.

It was not enough. He opened the virus code instead.

---

He started, as he always did now, with the damage pattern. A copy of the virus payload went into the sandbox. A preserved handshake replay went in after it. On the output pane, vision dropped to null first. Hearing followed. Proprioception jittered, fragmented, then vanished. The motor governor stayed green throughout.

On the small skeletal model at the bottom of the display, the runner kept moving. Knees lifting. Arms driving. Head steady. Every sensory pane above it blank.

Yusuf felt his shoulders lock. Kai had hit a wall in that exact division between body and pilot. This thing did not knock an athlete down. It took the world away and left the machinery running.

"Designed," he said, and hated hearing the word out loud.

A random corruption event should have chewed through whatever it reached. Sensory channels, motor channels, safety routines, all of it. Messy. Wasteful. This was selective. Precise enough to leave the moving parts intact while everything that told you where your body was went dark.

He switched from functional behavior to compiled output. Virus on the left. Standard Meridian calibration firmware on the right. Same processor target, same file size class, same hex view. He ran an allocation scan and watched the histograms populate.

64. 128. 256.

The same block sizes repeated on both sides of the screen. The same alignment boundaries. The same padding after control structures. He ran the scan again because the first result landed in him like a dirty joke.

Same pattern.

His coffee had gone cold enough to grow a skin on top. He reached for it anyway, took one swallow, and put it back down untouched after that. The bitterness turned his mouth dry.

He opened the exception tables. Same nested error hierarchy. Same logging stamp format. Same buffer-overflow routine with the tidy fallback Meridian engineers liked because it kept the system live long enough to write its own autopsy. Yusuf had spent six years inside their firmware ecosystem. He knew their habits. Not personally, not from source code, but from compiled output, support notes, quarterly updates, and the long low-level repetition of working in something until its defaults felt familiar in his hands.

"Bollocks."

He kept going because stopping there would have been cowardice. Stripped builds still left crumbs if the team shipping them got lazy or hurried. He searched the string table. Generic library path. Useless. Standard debug call. Useless. Third result:

`/mbio/dev/tools/nlink/`

He did not realize he had pushed his stool back until it struck the cabinet behind him.

mbio.

Meridian BioSystems.

nlink.

Neural link.

The fluorescent tube nearest the window buzzed on its bad ballast. Yusuf looked away from the path, then looked back, as if the extra second might turn it into something else.

He opened a notes pane and typed what he could justify if anyone ever asked how he got there.

String table contains Meridian dev path.
Exception hierarchy consistent with current calibration firmware.
Allocator profile consistent with Meridian builds.

He stared at the third line, deleted `Meridian`, typed `vendor`, swore under his breath, and put `Meridian` back. The path was still there. The exception handling still matched. The memory pattern still matched. A stolen toolchain could leave those marks. So could a planted breadcrumb. So could an internal build nobody had scrubbed properly. He knew the distinction with the discipline of someone who had spent fifteen years in engineering and had watched good arguments die because the person making them reached one step too far.

He could not accuse Meridian on this. He could justify keeping the analysis off the facility network and digging until he found something that would survive contact with another engineer.

If the virus came out of Meridian's toolchain, yesterday's contract stopped looking like a panicked fix and started looking rehearsed. Two years of pushing for broader data rights, then a virus, then a patch that demanded permanent ownership of the exact streams he needed to read. He ran the order through again and it still came out dirty. He just didn't know yet whether it meant design, theft, or someone using Meridian's fingerprints because they were convenient.

His hands had been steady all night. They were still now in a different way. He saved the byte-level analysis to the personal archive only. Not the facility environment. Not anything Meridian's audit tools might sweep up before he was ready. When the save finished, he closed the virus windows, reopened the patch, and sat for a long time looking at code he could no longer see cleanly.

---

The door opened at quarter past three.

Yusuf did not turn at first. Technicians crossed the calibration wing at every hour, and the bay had enough entry points that a door opening usually meant nothing. But the footsteps stopped instead of passing. Someone stood there without speaking.

"Dr. Qadir."

He turned. Petra Engel stood in the doorway with her clinic coat still on over a grey jumper. Her hair, usually pinned into submission, had come loose on one side. She held a paper cup from the corridor machine. That meant she had thought about this conversation long enough to want coffee first.

"Dr. Engel. Bit late."

His own voice gave him away. He heard the Birmingham flatten out as soon as he spoke, the professional register locking over the sentence and squeezing the Birmingham out of it.

"I've been reviewing facility access logs for the past week," Petra said. "Routine audit, given the circumstances."

"Sure."

"Your badge accessed this bay at eleven forty-seven tonight. It is now three fifteen. You have no calibration sessions scheduled before eight."

"Sometimes I work late. You know how it is."

"I do."

She crossed to the secondary station and looked at his displays. He did not minimize anything. The virus windows were gone. The patch remained, dense enough to be obvious and incomplete enough to be dangerous.

"This is not a standard calibration tool," she said.

"No."

"What is it?"

"An alternative approach to the virus. I'm seeing whether I can block propagation without handing Meridian full access to every live system."

She sat on a stool beside the secondary station and set her cup down. Her movements stayed measured even now, but there was tiredness in them, not calm.

"On your own," she said. "Without authorization. On facility hardware."

"Yes."

"Is this the only unauthorized work you have been doing in this bay?"

He felt the flinch move across his face before he could stop it. Petra caught it.

"I've been running additional analysis on the virus code," he said. The vowels tidied themselves even further. "The standard diagnostic approach is not getting all of it."

"The access logs show you have been here after hours on eleven of the last fourteen nights," she said. "Including nights before the virus was formally identified."

He could explain that. The anomaly tracking, the drift patterns, the weeks of little mismatches that had started before anyone called it infection. The explanation was true. It also opened the wrong door.

"I was concerned about network anomalies before the formal diagnosis," he said. "The virus confirmed the pattern."

"And the transfers to an unregistered device?"

His hands went still on the desk.

"System logs show small encrypted exports from this station," Petra said. "Regular. Off-book. IT security is busy with the outbreak, the delegation, and everything else that is currently on fire. They have not followed the trail yet. They will."

Yusuf pushed his glasses up his nose. It gave him half a second and nothing useful came in it.

"I've been backing up biological calibration data," he said. He let the professional sheen drop because holding it up had become silly. "Athlete biometrics. More than my job covers."

"Why?"

He thought about lying anyway. Redundancy. Network stability. Data integrity. Petra had not come here at three in the morning for a line like that.

"Personal research," he said. "There are neurological applications in the data that nobody's pursuing. Degenerative disease work. It's personal, all right? The data already exists and Meridian only values it when they can sell around it. Once that contract locks everything down, nobody outside them gets near it."

Petra looked at him for a long moment. Not suspicious now. Measuring.

"There was an athlete at the Stuttgart facility." She picked up the cup, found it empty, set it back down. "This isn't — I'm not offering this as a defense of what you're doing."

"All right."

"Marius Koch. Decathlete. Twenty-four." She was looking at the code on his center display rather than at him. "His body started rejecting the synthetic muscle grafts. Immune cascade, rejection markers all over the bloodwork. The monitoring system kept calling it calibration variance. I let that classification stand for eleven days before I escalated, which — " She stopped. "That's a separate issue."

Yusuf didn't speak.

"I wrote three reports. I recommended immediate removal. The facility director forwarded them to Meridian's medical oversight." She corrected herself: "I say forwarded. He agreed with me. He sent them with his own recommendation attached. Meridian reclassified the rejection as within acceptable adaptation parameters and told us to continue training."

"What happened?"

"He died. Fourteen days later. Organ failure."

Yusuf looked at his hands.

"I filed a complaint. The investigation found that protocols had been followed, and they had been. Nobody wanted to look at whether the protocols should have existed in the first place." She turned the empty cup between her palms. "I'm not telling you this so you'll feel sorry for me."

"Petra."

"I'm not going to report you."

He looked at her then.

"I don't want details of your personal research," she said. "I don't want information that would oblige me to disclose more than I already know. What I am telling you is that the transfer logs will be audited. Two weeks, two months, I cannot say. But they will be audited."

"I know."

"Then decide what you are going to do before someone else decides it for you."

She stood, took her cup, and walked to the door. Her hand found the plate and stayed there.

"If this alternative approach shows clinical promise," she said, still facing the corridor, "I want to see the data before it goes anywhere near a live system. That is not a request from the medical director. It is a request from a physician."

"Understood."

"Good night, Dr. Qadir."

"Night."

The door shut. The bay settled back into machine hum and ceiling-light buzz. Yusuf pulled the patch window full-screen. Thirty-four of forty-seven handshake variants mapped. He keyed in variant thirty-five by hand because his fingers needed the work.

Outside the window the mountains had started to separate from the dark. On the display the replay hit the hook, hesitated, and spilled a new column of latency numbers down the pane. He leaned closer before he had even read the first one.
