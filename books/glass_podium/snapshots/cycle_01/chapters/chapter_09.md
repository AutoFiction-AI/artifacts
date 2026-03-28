# Chapter 9

Yusuf talked to himself when he worked. Not the self-conscious muttering of someone performing eccentricity, just a steady half-voiced narration of what his hands were doing, the way some people hummed. Fragments of logic, technical shorthand, the occasional "right" that served as both punctuation and encouragement. The calibration bay at two in the morning was the one place it didn't matter. The diagnostic terminals threw blue-white light across his face and the desk and the cold coffee he'd poured three hours ago from the machine in the corridor — the one that produced an aggressively bitter espresso from beans that seemed personally hostile to the concept of flavor.

He had the virus architecture mapped across three displays. The propagation mechanism was elegant, which was the problem. It threaded through the calibration network's handshake protocols — the standard exchange that occurred whenever two enhanced systems synced during a tuning session. Every time an athlete lay in the calibration rig and Yusuf ran a routine adjustment, the network opened a brief two-way data channel. The virus nested inside those channels like sediment in a pipe.

"So if I can interrupt the handshake before the payload deploys..." He scrolled through the firmware's authentication layer, his glasses reflecting the scroll of code. "No, because the authentication happens after the channel's already open. Horse is already out. Right."

The partial patch concept was simple in theory. Instead of Meridian's approach — a complete firmware rewrite requiring permanent read-write access to every enhancement system — his design targeted only the virus's propagation pathway. Seal the handshake exploit. Quarantine infected firmware modules. Leave everything else untouched. No data surrender. No permanent corporate access to anyone's biological information.

Simple in theory. In practice, he was trying to build a pressure seal for a submarine from the inside of the submarine while it was underwater.

The calibration network's architecture was Meridian's proprietary design, which meant Yusuf was working from reverse-engineered schematics and his own six years of institutional memory. He knew the system better than anyone at Kirchberg — he'd calibrated hundreds of athletes through it, felt its patterns and quirks the way a mechanic knows an engine by the pitch of its idle. But knowing a system was different from knowing its source code, and Meridian didn't share source code. They shared APIs and documentation that described what the system did, not how.

He was building the patch by inference. Probing the firmware's behavior, mapping its responses, constructing a model of the underlying architecture from observable output. Like reconstructing a building's blueprints by knocking on walls and listening to the echoes.

Outside the bay's single window, the floodlit car park was empty. Beyond it, the mountains were shapes against a sky that was slightly less dark than it had been an hour ago. The days were getting longer — imperceptibly, a few minutes each week, the late-winter light stretching toward something that wasn't quite spring but was no longer the deep Alpine dark of January. Yusuf noticed this the way he noticed most things that weren't the problem in front of him: peripherally, as data.

"Right. This bit handles sensory routing." He highlighted a block of code on the center display. "And this bit talks to the motor subsystem. So the handshake has to pass through... here. Or here. Shit."

Two possible interception points. The first was cleaner but sat upstream of the sensory processing stack — patching there might introduce latency. A tenth of a second, maybe less, between the world and the athlete's perception of it. For a sprinter at full speed, a tenth of a second was the difference between gold and nothing. For a swimmer mid-turn, it was the difference between a clean rotation and a collision with the wall. The performance cost would be real and measurable, and the athletes who chose this patch over Meridian's deal would be choosing it with their eyes open.

The second interception point was messier, deeper in the firmware, closer to the autonomous subsystem that governed involuntary motor function. Patching there would preserve sensory fidelity but might interfere with the safety protocols that kept synthetic muscle from firing at full force during, say, a stumble. The protocols that caught you when you tripped.

Neither option was clean. He sat with the second interception point and thought about what it meant to touch the firmware layer that decided when a body caught itself. The biological data flowing through these systems — the neural patterns, the motor mapping, the proprioceptive feedback loops — was exactly the kind of data that could map the early-stage neural deterioration patterns in conditions like Farah's. Nobody was using it for that. Nobody would be using it for that once Meridian locked it behind a corporate license and a transferable data contract that let them sell it to whoever offered the most.

He pushed the thought aside. Not because it didn't matter but because it mattered in a way that would contaminate his engineering judgment if he let it, and right now the engineering judgment needed to be clean.

He chose the first interception point. The performance cost was honest — a measurable tradeoff, something he could explain to an athlete in plain language. The alternative was gambling with safety protocols he couldn't fully predict.

His hands moved across the keyboard with the particular fluency of someone building in a language he thought in. The code took shape in fragments: a conditional check here, a routing exception there, a quarantine protocol that would intercept the virus payload during the handshake and dump it into a sandboxed partition instead of allowing it to integrate with the athlete's firmware. The quarantine design was borrowed from standard cybersecurity practice — isolate the threat, contain it, neutralize it without touching the host system. Simple principle. The execution required mapping every variant of the handshake exchange the calibration network could produce, and there were, by Yusuf's current count, at least forty-seven.

He'd mapped thirty-one.

The patch would also sever any bidirectional data pathway that the virus could exploit — which meant, as an unavoidable side effect, that the neural coaching feed interface would no longer function. The feed relied on exactly the kind of open channel the virus used for propagation. Closing one meant closing the other.

Margot would fight this. He already knew that. The performance cost was a technical argument. Losing the feed was personal, and Margot's version of personal had a quality he didn't want to examine too closely.

He saved his work to two locations: the facility's development environment, where it would look like routine calibration tool maintenance, and his personal device — the encrypted archive in his quarters, holding weeks of biological data he had no authorization to possess.

"Right," he said to the displays. "That's enough for one night."

It wasn't. He didn't leave.

He opened the virus code instead.

---

He'd been picking at the virus architecture for days, in stolen hours between calibration sessions and staff meetings and the careful maintenance of his professional composure. The surface structure he'd already mapped — the propagation mechanism, the sensory corruption patterns, the way it nested inside the handshake protocols like something designed to fit there.

Designed. That was the word that kept surfacing, and that he kept pushing back down.

The virus was sophisticated. Not in a showy way — no baroque complexity, no clever tricks for tricks' sake. Sophisticated the way a well-made tool was sophisticated: it did exactly what it needed to do, no more and no less. It propagated through the calibration network efficiently. It corrupted sensory processing selectively — targeting the input channels that governed sight, proprioception, and hearing while leaving the motor subsystem's autonomous functions intact. This meant the body kept moving during a blackout. The body kept running, swimming, jumping, doing whatever it had been doing at the moment the senses went dark.

This was, from an engineering perspective, an interesting design choice.

A natural virus — a mutation in the firmware, a cascade of corrupted data propagating through the network's shared infrastructure — would not be selective. It would corrupt whatever it reached, motor and sensory alike. An athlete hit by indiscriminate corruption would collapse: muscles seizing or going slack, the body shutting down mid-stride. Ugly. Painful. Unlikely to kill. The body would stop.

This virus did not stop the body. It blinded the pilot and left the machine running at full speed.

Yusuf had been thinking about this for three days. He'd been thinking about it the way he thought about all engineering problems: structurally, looking at the architecture rather than the symptoms. And the architecture told him something he did not want it to.

He opened the virus code at the byte level. Not the functional layer he'd been working with for the patch — the underlying implementation. The way the code was actually structured, beneath the behavior. He was looking at it now the way a typographer might examine a forged document: not reading the words but studying the letterforms, the spacing, the ink density.

Code had signatures. Development tools left traces in compiled output — memory allocation patterns, variable naming conventions, compiler artifacts, the particular way different toolchains handled error routines. These traces were usually invisible at the functional level. You had to go looking. They were fingerprints.

He pulled up the Kirchberg calibration system's firmware in a parallel window — Meridian firmware, maintained and updated quarterly by Meridian's development team, compiled with Meridian's proprietary toolchain. Standard reference material. Every engineer at every Meridian-affiliated facility had access to the compiled firmware. The source code was proprietary, but the compiled output was part of the working environment.

He put the virus's compiled output next to it.

Memory allocation. He checked the block sizes first — the fundamental units in which the code requested and managed system memory. Then alignment boundaries: the way data structures were spaced in memory, padded to fit the processor's preferred access patterns. Then the padding itself, the empty bytes inserted between data fields.

The pattern was the same.

Not similar. Not within the normal range of variance you'd expect from similar toolchains. The same. The same block sizes, the same alignment boundaries, the same padding behavior. The virus allocated memory the way Meridian's firmware allocated memory, because they were both built with the same development tools.

Yusuf's coffee sat untouched beside his right hand. The display light was giving his fingers a bluish cast, like they belonged to someone slightly less alive.

He checked the error-handling routines. Same nested exception hierarchy. Same logging format. Same method of handling buffer overflows — a particular approach that Yusuf had recognized years ago as Meridian house style, a standardized pattern their engineering team used across all their firmware products. It was efficient, well-documented internally, and distinctive enough that he'd been able to identify Meridian-compiled code in mixed environments just by reading the exception structure.

"Bollocks," he said quietly.

He kept going. Variable naming in compiled output was mostly stripped — the human-readable names replaced by machine addresses during compilation. But there were traces. Debug symbols that hadn't been fully cleaned from the production build. String references containing fragments of the original source paths. He found three. Two were generic — standard library references that could come from any development environment. The third was a partial directory path embedded in a debug trace: `/mbio/dev/tools/nlink/`.

mbio. Meridian BioSystems.

nlink. Neural link.

Yusuf took off his glasses and cleaned them on his shirt. The displays blurred into colored smears. He put the glasses back on and the code resolved into clarity, and he sat there looking at it.

This was not proof. He knew that with the precision of someone who had spent fifteen years in engineering and understood the difference between evidence and inference. Development tools could be stolen, leaked, pirated. An external actor could have obtained Meridian's toolchain and used it to build the virus — deliberately, to frame them, or incidentally, because Meridian's tools were genuinely good and widely available in certain underground channels. The debug path fragment could be a plant, or a remnant from a stolen development environment, or a coincidence. The memory allocation pattern was a toolchain artifact — it pointed to Meridian's tools, not necessarily Meridian's engineers.

Suggestive. Not conclusive. The distinction mattered because conclusive meant evidence and suggestive meant conspiracy theory, and the distance between those two things was the distance between being taken seriously and being dismissed as a paranoid engineer with personal reasons to distrust the company.

But.

If the virus was Meridian's work, then the data surrender contract wasn't a response to the crisis. It was the purpose of the crisis. Create the threat. Engineer the fear. Offer the solution. The solution happens to require permanent, irrevocable, transferable ownership of every athlete's biological data — the exact dataset Meridian had been trying to acquire through contract renegotiations that had stalled for two years before anyone at Kirchberg had ever heard of a calibration virus.

Yusuf did not say this out loud. He did not mutter it to the displays or whisper it into his cold coffee. He sat with it. The processing equipment hummed. The fluorescent tube nearest the window buzzed at a slightly different frequency from its neighbors, a mismatched ballast he'd reported to maintenance twice and that nobody had fixed. His hands, which had been steady all night, were very still on the keyboard.

He saved the analysis to his personal archive. He did not save it to the facility's development environment. He closed the virus code windows and opened his patch work instead, and for a long time he looked at the code without seeing it.

---

The door to the calibration bay opened at quarter past three. Yusuf didn't turn — the bay had a dozen entry points and technicians came and went at all hours for system checks. But the footsteps stopped, and the silence had the particular weight of someone standing still and watching.

"Dr. Qadir."

He turned. Petra Engel stood in the doorway with her clinic coat still on over a grey jumper he'd seen two days ago. Her hair, grey-streaked and usually pinned with architectural precision, was listing to one side in a way that suggested it had been taken down and put back up at least once since the original pinning. She had a paper cup from the corridor machine, which meant she'd made a stop on the way here and thought about what she was going to say while the machine dispensed its grievance.

"Dr. Engel." His voice shifted. He heard it happen — the Birmingham flattening out, the vowels tidying themselves, the professional register sliding into place. The tell. He knew it was a tell. He couldn't stop it. "Bit late."

"I've been reviewing facility access logs for the past week." She stepped into the bay and let the door close behind her. "Routine audit, given the circumstances."

"Sure."

"Your badge accessed this bay at eleven forty-seven tonight. It's now three fifteen." She took a sip from her cup and made a small expression of displeasure that might have been the coffee or might have been the situation. "You have no calibration sessions scheduled before eight tomorrow morning."

"Sometimes I work late. You know how it is."

"I do." She crossed the bay slowly, not approaching him directly but moving toward the secondary diagnostic station, putting herself in a position where she could see his displays. Yusuf did not minimize his windows. He'd already closed the virus analysis. What remained on screen was the patch code — explicable, if not exactly authorized.

Petra looked at the displays. She was a physician, not an engineer, but she'd spent a career working alongside calibration systems, and she read firmware architecture the way a literate adult reads a foreign language — not fluently, but enough to know what she was looking at.

"This isn't a standard calibration tool," she said.

"No."

"What is it?"

"A possible alternative approach to the virus." He kept his voice professionally warm, the register he used when explaining technical details to athletes during calibration. Measured, clear, slightly too polished. "I'm exploring whether we can target the propagation mechanism without requiring the full data access that Meridian's patch demands."

Petra was quiet for a moment. She pulled a stool from the secondary station and sat down, the movement slow and deliberate — no wasted motion, but no urgency either. She set her cup on the desk beside her and adjusted the stool's height, a small domestic gesture in the sterile bay, and Yusuf noticed that her hands were dry and cracked at the knuckles in the way of someone who washed them forty times a day and had stopped bothering with lotion.

"Exploring," she said. "On your own. Without institutional authorization. Using facility systems after hours."

"Yes."

"Is this the only unauthorized work you've been doing in this bay?"

The question landed with precision. Yusuf felt his face do something he couldn't control — a flinch in the muscles around his eyes, quick enough that most people would miss it. Petra was not most people. She was a physician who had spent decades reading faces for the micro-expressions that patients produced when they were about to minimize their symptoms.

"I've been running additional analyses on the virus code," he said. Clean, precise, technically true. The Birmingham was completely gone now. "The standard diagnostic approach isn't capturing the full picture."

"The access logs show you've been in this bay after hours on eleven of the past fourteen nights." She let that sit. "Including nights before the virus was formally identified."

The before. Eleven of fourteen nights. He could explain — he'd been tracking anomalies in the calibration network for weeks, correlated drift patterns across multiple athletes that had concerned him before anyone knew there was a virus. The explanation was true. It also opened a door to questions about what he'd been doing with those weeks of observation, and what he'd been doing with the data, and where the data was now.

"I've been concerned about network anomalies for some time," he said. "The virus diagnosis confirmed what I'd been tracking independently."

"And the data transfers to an unregistered device?"

His hands, which had been resting flat on the desk, went still. Not the stillness of composure. The stillness of a body that had decided to stop moving before the mind caught up, the way you freeze when you step on ice and feel the first shift.

"The system logs show external transfers from this station," Petra said. She wasn't accusatory. Clinical. "Small, regular, encrypted. IT security hasn't flagged them because they're focused on the virus response and the corporate delegation and the seventeen other things that are currently on fire. But eventually someone will audit the transfer logs the way I've audited the access logs, and they'll find them."

Yusuf looked at his hands on the desk. His glasses had slid down his nose. He pushed them up. The gesture gave him half a second.

"I've been backing up biological data," he said, and let the professional register drop. The Birmingham came back, and with it a looseness in his syntax that felt like setting down something heavy. "Athlete biometric data from calibration sessions. More than my job scope covers."

"Why?"

He could offer the professional justification. Redundancy, data integrity, concern about network stability. Petra would not believe it. She had come here at three in the morning with a paper cup of terrible coffee, which meant she'd been sitting on this for days, deciding what to do with it before deciding what to do about it.

"Personal research." He rubbed the bridge of his nose where his glasses sat. "There are applications for the biometric data that aren't being pursued. Neurological applications. Treatment research for degenerative conditions. Conditions that — yeah. It's personal. The data's there, it's being generated anyway, and nobody's using it because it doesn't serve Meridian's commercial priorities. And once that contract locks it down, nobody will ever use it."

"Personal research," Petra repeated. Not a question. A careful arrangement of words on a surface, looked at from different angles.

"Yeah."

She was quiet. She picked up her cup, looked into it, put it back down without drinking. Then she looked at the ceiling, where the fluorescent tube nearest the door was buzzing at its mismatched frequency.

"There was an athlete at the Stuttgart facility," she said. "Marius Koch. Decathlon. Twenty-four. His body rejected the synthetic muscle grafts — an immune cascade that the monitoring system classified as a calibration variance for eleven days before I escalated it." Her voice had lost its hedging. The qualifiers that usually softened her statements into clinical probability were gone. "I wrote three reports. I flagged the rejection markers. I recommended immediate removal of the grafts. The facility director forwarded my reports to Meridian's medical oversight team. Meridian reclassified the rejection response as within acceptable adaptation parameters and recommended continued training."

She paused. Not for effect. Because the next part was a fact she had carried for three years and it still needed a moment.

"Marius died fourteen days later. Systemic organ failure."

Yusuf didn't speak.

"I filed a formal complaint. The investigation concluded that protocols were followed. Protocols were, in fact, followed. The protocols were wrong. Marius was dead. The investigation closed." She looked at Yusuf, and the tiredness in her face wasn't the chronic background fatigue he was used to seeing. It was specific. The tiredness of someone who had been right and had watched it not matter. "I was overruled by people who had institutional reasons to minimize what the data was telling them."

"Petra—"

"I'm not going to report you."

The sentence was flat and simple. She said it the way she said medical facts — without cushioning, without invitation to discuss.

"I don't want to know the details of your personal research. I don't want to be in a position where I'm required to disclose information I haven't been given." She stood up from the stool. "What I will tell you is that the IT security team will audit those transfer logs. It may take two weeks. It may take two months. But they're competent and they're thorough, and they will find the transfers."

"I know."

"Then you should consider what you're going to do about that before they do."

She picked up her cup and walked toward the door. Stopped. She didn't turn around, but she wasn't leaving either. She was standing in the doorway the way someone stands when they've said what they came to say and now there's one more thing that wasn't part of the plan.

"If the alternative approach you're developing shows clinical promise," she said, "I'd want to see the data. Before it goes anywhere near a live system. That's not a request from the medical director. That's a request from a physician."

"Understood."

"Good night, Dr. Qadir."

"Night."

The door closed. The calibration bay returned to its hum, its fluorescent buzz, its blue-white light on the desk where Yusuf sat. His coffee was cold. His patch was sixty percent finished and the forty percent that remained was the part that could kill someone if he got it wrong. The virus code on his personal archive contained structural signatures that pointed, suggestively, inconclusively, damningly, toward the company that built the systems the virus was destroying and that had arrived within a week with a solution that happened to cost exactly what they'd been trying to buy for two years.

He couldn't prove it. He couldn't share it yet. He couldn't stop the shape of it from sitting in his head, solid and ugly, while the processing equipment hummed and the mountains outside the window emerged slowly from the dark as the sky began, just barely, to lighten.

He saved his work. He closed his displays. He sat in the bay for a while longer, in the hum, in the dark that wasn't quite dark anymore, and did not sleep.
