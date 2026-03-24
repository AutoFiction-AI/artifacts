# Chapter 14

The Slack notification from Elena Park was still open on Nick's phone in the San Leandro lot. He'd read it three times already, and it still looked wrong.

*Calibration team — Conf Room B, 8:15 AM. Attendance required.*

Elena Park, Marcus Webb's assistant, never messaged the calibration team directly. The rain had been going since Sunday night. Water sheeted down the windshield and turned the building into a gray blur. When she sent something it came through Marcus's channel with agenda items and prep links and suggested reading, the organized energy of a person who believed that preparation was a form of respect. This was none of that. A room, a time, and the word *required*, which in corporate Slack carried the same weight it carried anywhere else.

His phone buzzed. Tommy in the team chat: *anyone know what's going on?* Then Dani: *No idea.* Then nothing. The chat sat there with its two messages like a room where someone had asked a question and everyone was waiting for the person who knew to speak.

Nick turned off the car. The parking lot was the same lot it had been every morning for almost a year — the same landscaping strip dying between two curbs, the same dumpster with its crooked lid, the same flat-roofed building that could have been a dental office or a tax-preparation franchise or exactly what it was, a place where people sat in rows and rated images for a company that rated them back. He noticed the sky's tonal value — flat, even, no directional shadow, the kind of overcast that washed out every surface to the same gray — and it registered automatically, involuntarily. The gray had the same inevitability as tinnitus: always there, never chosen.

Inside, the floor was wrong. Not fire-alarm wrong. Not sobbing-coworker wrong. The HVAC hummed. The fluorescents threw their flat wash across the beige carpet. But the morning rhythm was absent — the click-settle-click of people opening batches, the low murmur of evaluators comparing notes, the soft run of mouse taps and space bars that usually took over once twenty-five people sank into their screens. People were at their desks, but they were looking at each other. Some were on Slack. A few had their phones out, which Priya normally discouraged during work hours, and Priya was not at her station discouraging anything.

She was by the coffee station. Her hair was pushed back with a clip she only used when she'd been here early, and her Costco antacid bottle was sitting on the counter between the sugar packets and the stir sticks, out in the open, which meant she'd already been to the conference room and the conference room had been bad enough that she'd forgotten to put it back in her desk drawer.

"Did you get the message?"

"Yeah. What's going on?"

"I don't know exactly." She picked up the antacid bottle, looked at it like she wasn't sure whose it was, and slid it into her cardigan pocket. "I called Devra in QA. She said they ran some kind of statistical review over the weekend and something flagged. She wouldn't give me details."

"Something in calibration?"

Priya's shrug was not a casual shrug. Her shoulders went up and held a beat too long, and when they came down they were higher than they'd started. "Calibration data. That's all she said."

Nick poured coffee. His hand was steady. The rest of him felt like a pitch just below audible — a low hum that started in his sternum and spread to his wrists and his jaw and the soles of his feet. He watched the coffee fill the mug, watched the surface shiver from the pour, and thought about the distribution curves that would show his work if someone knew where to look. The rightward drift in anatomical-accuracy ratings. The clustering in the lighting-consistency band. Four months of corruptions, each one individually defensible, each one calibrated to sit inside the range of reasonable expert disagreement, and all of them together forming a pattern that was as legible to him as a brushstroke signature — if anyone thought to read it that way.

Nobody would read it that way. The system caught noise. The system caught laziness. The system did not catch a senior calibrator applying his expertise in reverse because the system was built on the assumption that expertise pointed in one direction.

He took his coffee to Conference Room B.

The meeting was small. Six from the calibration team, plus Devra Singh from QA, plus a man Nick didn't recognize wearing a blue polo and a Canopy badge clipped to his belt instead of on a lanyard. Belt clip meant corporate. It was one of those signifiers that nobody acknowledged and everyone understood, like the difference between a name tag and a title card.

Priya sat against the wall rather than at the table. Nick sat next to her. Across the table, Jun-seo from the calibration team was scrolling through his phone under the table with the focused expression of a person looking for information that would make this meeting less frightening.

Devra started. She was compact, mid-forties, and she wore her QA role like religious conviction — not loudly, but as the organizing principle of everything she did. She turned her laptop so the room could see.

"Friday evening, the automated review flagged statistical anomalies in calibration data from last quarter. Specifically, we're seeing distribution shifts in anchor ratings across three categories." She pointed at the screen. "Anatomical accuracy, lighting consistency, and compositional balance."

Nick looked at the graphs. Simple distribution curves with highlighted drift regions. He could see his work in them — not a name, not a trail, but the shape of what he'd done, something he could read from across the room as easily as he could read brush direction in dried impasto from across a gallery. A slight rightward shift in anatomical accuracy, meaning the pipeline was increasingly accepting wrists bent wrong, ears placed too high, shoulders socketed where shoulders did not socket. A compression in lighting-consistency scatter that reflected the biases he'd introduced between October and December. Four months of work, up on a screen, and the only person in the room who could read it was him.

"The shifts are subtle," Devra said, "but they're consistent across the quarter and they don't match the variance we'd normally expect from the calibration team or the broader evaluator population." She clicked to the next slide. The room changed with it.

Bars now, broken out by site and queue family. One of them sat under SAN LEANDRO LOCAL ANCHORS and glowed the wrong color: not red, not yet, but yellow enough that Jun-seo put his phone away. Priya straightened against the wall. Nick felt the blood in his face do something small and ugly.

"The initial pass doesn't tell us intent," Devra said. "It tells us where the variance clusters. Right now the strongest local signal is in portrait and figure-study anchors reviewed out of San Leandro. Overflow batches from Partner Labs are the other concentration point. Nick, Jun-seo, you two handled most of anatomy and lighting in that window. Did anything operational change in October or November?"

Queue mix, Nick thought. Say queue mix. Keep it boring.

"Queue mix," he said, too fast, and made himself slow down. "We got flooded with close-cropped portraits and hand batches. Bad wrists, extra fingers, key lights that changed direction halfway down a face. If overflow raters were pushing volume on that stuff, we'd be correcting the same failures on the back end over and over. That would skew anatomy and lighting before it told you anything useful about the anchors."

"And compositional balance?" Devra asked.

"Tight crops. Product-prompt people. Fake studio symmetry." He lifted a shoulder. "That category clumps when half the frame's already been decided for you."

He had said too much. He heard it while he was still speaking: the extra sentence, the clarifying clause, the exact shape his lies took when they needed support. Priya looked at him. Not suspicion, not yet. Surprise, mostly, that he'd volunteered at all.

Devra typed without looking up. "We normalized for category, not prompt-family density."

The man in the blue polo leaned forward. "We've been seeing parallel patterns from Partner Labs. Manila specifically."

It was not relief, exactly. More like the beam moved off him and hit somebody else.

Nick drank his coffee. It was too hot and it burned the roof of his mouth and the pain was a small, good thing because it gave him something to focus on while the conversation moved six thousand miles away from him.

The man's name was Glen Horstmann, and he worked in Operations, which was not a department Nick had ever needed to think about. Glen from Operations explained that the Manila labeling center — which handled overflow calibration batches and large-volume evaluation contracts — had been flagged independently by a separate monitoring system. Evaluators there were submitting ratings at speeds that were, in Glen's corporate vocabulary, "inconsistent with thorough evaluation." Average assessment time: twenty-two seconds per image. Standard was two to three minutes. Completion bonuses, paid when evaluators exceeded a per-shift volume threshold, were triggering at ninety-four percent, against a historical average of sixty-one.

"We think the calibration-data drift is downstream from the Manila throughput issue," Glen said. "Their rapid-fire ratings are pulling the anchor distributions. We're still running the full regression, but preliminary correlation is strong."

Nick nodded when other people nodded. He looked at the screen when other people looked at the screen. He asked no questions, which was normal — he was known as the quiet one on the calibration team, the evaluator who did his work on-screen and said little in rooms. His silence was a feature of his reputation. It had never been as useful as it was now.

The meeting went forty minutes. The action item was a full audit, led by Marcus Webb, who was coming from San Francisco on Wednesday.

Nick walked back to his desk. The floor had loosened slightly — the fear was still there, but it had a shape now, and a shape meant an explanation, and an explanation that pointed at Manila meant it didn't point here. People were murmuring. Someone in the back row asked a question about whether their own metrics were under review, and someone else said probably not, and the uncertainty thinned into people reopening Slack, glancing over their monitors, loading queues and not clicking the first image yet.

Bao was at his station, reading glasses on, studying an image of a generated landscape with the deliberate attention that had earned him two written warnings about throughput. His evaluation pace was meticulous — he examined color relationships and compositional structure with a care that belonged in a design review, not an assembly line. The system wanted two minutes per image. Bao gave four, sometimes five, because four or five was what the image required if you actually looked at it. He gave Nick his usual nod, a single dip of the chin that contained both greeting and return to focus.

Nick sat down. He opened the evaluation portal. The queue appeared — generated faces, generated landscapes, generated hands with fingers that bent in directions fingers didn't bend. He started rating. His accuracy was flawless. It was always flawless. That was the whole point.

---

Marcus came on Wednesday. Not alone — he brought two people from the data-integrity team, a woman named Anh Tran from workforce compliance, and Glen Horstmann again. They set up in Conference Room A, the larger one with the long table and the projector screen and the slightly better chairs purchased for a client visit two years ago and then left to improve whatever meeting was judged important enough to need them. The calendar invitation said "Quality Review — Open-Ended," which in corporate scheduling meant clear your afternoon.

The calibration team, Priya, Devra, and two night-shift evaluators Nick didn't know took seats around the table. He set his coffee on top of his legal pad so the cup would hide his hand if it shook. Marcus looked the same — the good sneakers, the untucked oxford, the watch — but his usual warmth had strain under it now, visible as effort. The polish was load-bearing, holding together a person who cared about the work and was watching it crack.

"I'm not here to assign blame," Marcus said. "I'm here because the calibration pipeline is the foundation of everything we do at Canopy. If the anchors are off, every downstream model drifts. And the data says we've got drift."

His thumb pressed the face of his watch once, hard. "What we need to understand is the scope and the source. Anh, can you walk us through what we've got?"

Anh took over. She was maybe thirty, with a presentation style that had no small talk in it and didn't apologize for the absence. Rows of evaluator IDs filled the screen, each one beginning with MNL. Nick read the prefix before he read anything else. Manila. The first slide was still on the wall when Anh said, "We suspended seventeen evaluators over the weekend pending full review. Twenty-six more are under enhanced monitoring."

Nick set his coffee down too hard. The lid clicked against the cup. Seventeen. Saturday morning, thirteen hours ahead of his. Somebody opening the portal before breakfast and getting a deactivation banner instead of the queue.

"The Manila center handles approximately thirty percent of our overflow calibration volume," Anh said. She clicked to throughput charts, then bonus tables. "Q4 monitoring flagged a pattern consistent with systematic completion-bonus gaming. Average assessment time fell to twenty-two seconds per image. Per-task pay is one dollar eighty. The completion bonus adds forty cents per task once an evaluator exceeds four hundred evaluations in a shift."

The math was not hard. At that speed the extra forty cents was not extra. It was groceries, transit fare, the part of rent you begged a landlord to wait on. Nick rubbed his thumb along the paper seam of the cup until it softened under the sweat in his hand.

"Suspended meaning their accounts are already deactivated?" Priya asked.

"Deactivated pending review," Anh said.

"So they're not working."

"Correct."

Priya leaned forward. "Some of these people have been with us for two years. Their accuracy was solid before the bonus structure changed in August. This isn't a hiring problem. It's a compensation problem."

Marcus stepped in before Anh answered. He did it smoothly, with the practiced coordination of a person who had managed rooms for a living and knew when a conversation was about to move from data into policy, which was where VPs earned their title. "Priya, you're right that the compensation structure needs a separate review. I'm committed to that. But right now we need to scope the data impact and trace how far the drift has propagated."

Priya held his gaze for a beat. Marcus's thumb found the watch again. Anh had already moved to the regression tab.

The Manila controls cleared most of the orange off the screen. Most. A thinner band remained in San Leandro, concentrated in the same three categories already on the board. Nick felt the back of his neck go cold before Anh said the words.

"Residual unexplained anchor variance," she said. "Below action threshold. Not below notice."

Devra clicked into another tab. Evaluator initials appeared beside the categories. N.B. sat there twice, once under anatomical accuracy and once under lighting consistency. Nick kept both hands flat on the table.

"Nick," Marcus said. No warmth now. "Talk me through those queues."

"A lot of cropped hands," Nick said. "Portrait batches too. Garbage studio-light prompts. When the wrist is cut at the frame line or the light source is half prompt, half hallucination, the correction band gets noisy because you're not judging the same error every time."

"That explains disagreement," Devra said. "Not directionality."

Nick heard the lie trying to grow teeth and failed to stop it in time. "Then strip out the cropped-hand queues and rerun the local residual. Anything where anatomy drops off at the edge, anything with single-subject studio portraits. If the drift stays after that, fine. But right now you're mixing queue bias with anchor behavior."

He had added clauses again. He could hear them stacking while he spoke. By the time he shut up his mouth had gone dry. Marcus watched him for a beat that ran too long, thumb pressed hard against the watch while Devra typed.

"That knocks a third off the San Leandro residual," she said. "It doesn't clear it."

Glen started talking about waiting for the full regression before the room could narrow any further onto Nick. Nick let his breath out through his nose and kept his eyes on the screen. Model families. Remediation timelines. Partner-lab oversight. The language kept moving, which was all he needed it to do.

Near the end, Anh pulled up a broader performance overview — a heatmap of quality and throughput metrics across all evaluation centers. San Leandro's column was mostly green. Near the bottom, under a subheading for floor-level evaluators flagged for throughput deviation, three names were highlighted in orange. The third was Bao Nguyen, flagged for evaluation speed 2.3 standard deviations below floor average.

Nick's fingers closed so hard around the paper cup the lid buckled. Nobody mentioned Bao's name. The slide advanced anyway.

The meeting ended at one forty-five. People stood, stretched, checked phones. Chairs scraped back all at once and the room took its first full breath in two hours. Tommy was waiting outside in the hallway, leaning against the wall with his phone, and when Nick came out he raised his eyebrows in a question.

"Manila," Nick said.

"Shit. How bad?"

"Seventeen people suspended. Maybe more."

Tommy whistled, low. "Jesus. For what?"

"Gaming completion bonuses. They were clicking through images without looking."

"I mean — yeah. At what they're paying over there?" Tommy shook his head. He was fidgeting with his phone case, bending the corner back and forth. "My cousin did data entry for a BPO in Quezon City for like three years. Missed quota once and they locked him out before he even got upstairs. He sat on the curb outside the building refreshing his email on his phone because he kept thinking it had to be a glitch."

Nick said nothing.

"So like — yeah. Of course they game it. What else are you gonna do." Tommy's thumb was still working the phone case.

"Anyway," Tommy said. "We're good?"

"Yeah. We're good."

Tommy went back to his station. Nick stayed by the window a moment longer, seeing not the parking lot but the same login screen loading again and again, somebody trying the portal three or four times because people always checked twice before they believed a machine.

---

Friday's conclusion came in a memo, then in Marcus's tired voice in Conference Room B: the Manila throughput gaming was now the official cause, the seventeen suspended evaluators were terminated effective immediately, the remaining twenty-six would stay under enhanced monitoring, and the compensation review would wait for Q2. The San Leandro calibration team was cleared. The meeting lasted eleven minutes.

Before Nick made it back to the floor, Marcus caught him in the hallway. His shirt was creased at the elbows, there was stubble on his jaw that hadn't been there two days before, and the skin under his eyes had gone gray. He fell into step beside Nick with the casual approach of a colleague rather than a VP, which was a choice Marcus made and which cost him the formality that would have kept the conversation short.

"Nick. Hey. You have a minute?"

"Yeah, of course."

They stopped by the window at the end of the hall. The rain had paused but the sky was still flat and close, the low January overcast that turned every surface the same value and killed shadows. Nick could still hear *terminated effective immediately* in Marcus's voice, flat and procedural as if the sentence belonged on a slide. Good studio light, Nick's brain said, and then corrected: consistent atmospheric conditions, low variance, and he did not know which vocabulary was his anymore.

"I wanted to tell you directly," Marcus said. "Nothing in your quarter moved the wrong way. When we reran the analysis, your anchors were among the most stable in the dataset. Not just here. Company-wide."

"Thanks. I appreciate that."

"I mean it." Marcus kept looking at him, tired and earnest, his thumb worrying the face of his watch. Nick had learned to dread that look.

"If everyone evaluated the way you do," Marcus said, "we wouldn't have had this problem."

Nick heard himself adding words again, because that was what he did when the lie needed support. "I mean, it's been a stressful week for everyone, so it's good to know. I just — yeah. Thanks."

Marcus nodded. He was quiet for a moment, and in the quiet his polish thinned and something more private surfaced. He looked out the window at the parking lot, at the landscaping strip that never changed, at the gray sky.

"We're doing weekly spot checks on anchor variance for a while," he said. "Not just Manila. Every center. There's still residual drift in the quarter we can't fully explain, and Ops doesn't want to wait for the next automated review."

Nick's breath caught. Not visibly — he controlled it, redirected it into a slight shift of weight from one foot to the other, a motion so small it could have been anything. Weekly spot checks at every center. The residual drift was still there.

"Okay," Nick said. "Yeah. Makes sense."

Marcus rubbed his thumb across the face of his watch. "I pushed to keep the suspended Manila group on pay until the review closed. Finance said no. If the account's flagged, the money just stops. And then we schedule a comp review for Q2 and — I don't know. Pretend that fixes something."

Nick said nothing.

Marcus straightened. The private moment closed. The VP returned, composed and forward-facing. "Anyway. I'll be back in SF on Monday, but I'll be watching the data. And Nick — thanks. Seriously. Your consistency matters more than you probably realize."

He shook Nick's hand and walked back toward Conference Room A. His sneakers were quiet on the beige carpet. The watch caught the fluorescent light as he turned the corner.

Nick went to his desk. He sat down. He opened the portal. The queue of images appeared — generated faces with subtly wrong proportions, generated rooms with light sources that contradicted each other, generated hands. Always the hands. He rated a batch on autopilot, his accuracy perfect, his scores clean, and kept seeing a Saturday morning thirteen hours ahead of his: somebody at a kitchen table or the edge of a bed, logging in before breakfast and getting the deactivation banner again. Somebody else already doing the arithmetic on transit fare, groceries, whatever the week had been divided into before the account went dark.

He clocked out at five. The lot was dark — January dark, the streetlights already on at four thirty, the wet asphalt reflecting them in smeared lines of sodium orange. He sat in the Civic and did not start it.

The window was closing. The automated review had found the Manila fire and called it the whole blaze, but the anomaly regression had left residual drift it couldn't account for, and now Marcus had told him people were going to start looking for it on purpose. They were not waiting for next quarter. They were starting now.

He could stop. If he stopped now, maybe his own drift stayed buried under Manila's noise long enough for Bao's orange flag to stay orange. Maybe Priya got a few more weeks to keep calling it monitoring instead of action. Maybe Bao kept the part of his paycheck that went to Mai's care, and maybe the next seventeen people in some other office did not wake up to dead accounts and a locked portal. Nick knew the word *maybe* was doing almost all the work there.

Or he could finish it. Start where the anchor weight mattered most. Keep lifting anatomical-accuracy scores on hands with six fingers and wrists bent like hinges, on portrait faces with one eye a centimeter too high, on shoulders that joined the body in the wrong place but still looked plausible if you glanced fast. Stay generous on lighting consistency when a jaw cast a shadow the wall did not, when window light hit from the left and the catchlight still bloomed in the right eye, when a room had afternoon sun and overhead fluorescents both claiming the same cheekbone. Loosen compositional balance for dead-center crops and mannequin symmetry and those fake studio portraits where every body looked propped into place and left there. Do it for three weeks. Long enough that the bad anchors got copied, compounded, taught forward.

And when the weekly checks finally bit down, Bao's name would not flash orange and disappear. It would sit on the slide while somebody from compliance explained that 2.3 standard deviations below floor average meant a deactivation notice and no more caregiver money for Mai. Priya would be in the room with her antacid bottle in her pocket, talking about process because process was all she'd be allowed to talk about. Marcus would still ask good questions. None of that would bring the seventeen people in Manila back onto payroll. Nick knew all of it before he turned the key.

He started the car. The engine caught on the second try, as it always did in cold weather. The wipers came on automatically, smearing the rain that had started again. He pulled out of the lot and turned onto Davis Street and merged onto 880 north toward Oakland. The taillights ahead of him stretched into red lines on the wet freeway. He moved into the left lane and accelerated. The Civic's engine gave its usual complaint above sixty-five. The rain kept coming. He stayed in the left lane all the way home.
