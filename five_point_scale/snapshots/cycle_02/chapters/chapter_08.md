# Chapter 8

The hand had seven fingers.

Nick counted twice. The violinist's wrist was still in his eye, and for a second his eye wanted to grant this hand the same courtesy, to take the extra two as distortion in service of expression. But no. They were rendered with startling confidence — the AI had given them knuckle creases, subtle nail beds, even a plausible shadow cascade. This was a failed stock-photo prompt, a woman holding a coffee mug, and two of the fingers sprouted from the same proximal joint like a forked vine. The generated thumbnail gave the hand a wet, crowded quality, too much flesh packed into too little space.

He rated it: Anatomical Accuracy 1, Lighting Consistency 3, Compositional Balance 3, Stylistic Coherence 2, Prompt Adherence 2. The lighting was actually decent — a single warm source from the upper left, shadows falling where they should — which was the kind of thing that made the job strange. The AI could nail the light and botch the body in the same image, as if the model had studied Vermeer's windows but never looked at its own hands.

Nick clicked Next. The image vanished. Another one loaded: a landscape, rolling hills, a sky that couldn't decide between sunset and noon. He rated it, clicked Next, rated the next one, clicked Next. The rhythm of it. Open, assess, rate, click. He had been doing this for four months at the senior level, five total at Canopy, and the rhythm had burrowed into his hands the way brushwork used to — an automaticity that freed the mind to wander. That was the problem.

It was after six. The floor was thinning out around him. Dani had left at five-thirty, her tote bag slung over one shoulder, old paint still speckling the bottom seam. Tommy had disappeared without announcement around four, which either meant a dentist appointment or an early escape that nobody bothered tracking. Bao had stayed until six precisely, as he always did, logged off his station with the deliberate calm of a man shutting a shop, and nodded at Nick on his way out. The evening evaluators had started trickling in — a few of the second-job people, a woman who knitted between batches — but the floor had that underpopulated feeling, every other station dark, the fluorescent hum more audible, the air conditioning working harder now that June had settled over the East Bay and the business park's parking lot radiated heat through the windows like a kiln shelf.

Nick stayed. He had been staying late two or three evenings a week since March, telling Priya he wanted to clear backlog, which was true enough — the backlog was real, the new hires' throughput was terrible, and Priya was too pressed to question anyone who voluntarily worked past shift. What he hadn't told her was that the extra hours were study sessions. He wasn't studying the images. He was studying the system.

He minimized the evaluation queue and opened the QA dashboard — a page available to senior evaluators, mostly ignored, updated monthly, dense with the kind of graphs and tables that made his painter's brain itch. He had been reading it for weeks, charting what he found in pencil on a legal pad he kept in his bag. He wasn't using his good notebook, the one with the handmade paper he'd bought in art school, but a yellow legal pad, like a lawyer or an accountant, the kind of person who made plans.

The QA dashboard tracked every evaluator's accuracy against something called the "reference standard." Nick had assumed this meant expert consensus — if five senior evaluators rated an image, the average was the reference, simple enough to seem almost democratic.

He clicked into his own history and scrolled until he found the portrait with the slightly hyperextended wrist, the one he remembered because he'd spent longer on it than the image deserved. The hand looked wrong in a human way instead of an AI way — too loose at the joint, maybe, but not impossible. He had given Anatomical Accuracy a 4 and moved on.

In the far-right column, beside the green percentage match, a tiny gold lozenge sat lit. At default zoom it was no bigger than a sesame seed. He moved the cursor off it and back. The lozenge stayed. He knew the portal's little visual language by now without ever having meant to learn it — gray clock for pending review, red triangle for appeal, green check for confirmed batch. He had never seen gold.

He clicked it. A side panel slid over the graph.

CALIBRATION ANCHOR — REFERENCE STANDARD. EVALUATOR MATCH: 98.6%. SOURCE: CALIBRATION TEAM REVIEW.

He waited for the rest of the ratings to load. If "reference standard" meant consensus, there should have been a stack of evaluator rows, an average, a denominator, something plural. Nothing else appeared. One review. One set of numbers. Anatomical Accuracy 4. Lighting Consistency 4. Compositional Balance 3. Stylistic Coherence 4. Prompt Adherence 4.

Nick leaned closer until he could see the dust at the edge of the monitor. He closed the panel, opened a different record at random, and started looking for the gold.

A landscape from the previous week: rolling hills, sky caught between noon and sunset. Gold lozenge. Click. Same source.

A kitchen interior from another batch, one pendant lamp painted into the image and all the shadows cast from somewhere else. Gold lozenge. Click. Same source.

He went back farther. The anchors were scattered, not constant, maybe one in fifteen images, tucked into batches like spot checks, but every time the trail ended in one person's rating sitting where truth was supposed to be.

Nick opened the floor report Priya screenshared in team meetings. The same lozenges were there too, threaded through everyone's history — Bao's note-heavy batches, Dani's quick clean ones, Tommy's erratic Monday work, Nick's own high-scoring runs. The floor wasn't being measured against pooled judgment or the average wisdom of the room. Six people on the calibration team — their ratings, their eyes, their private sense of what a 4 meant versus a 3 — determined whether everyone else at Canopy was doing the job right.

Nick sat back in his chair. The monitor's glow was blue-white against the darkening window behind it. Outside, the parking lot had emptied to a dozen cars, and the chain restaurant across the access road had turned on its sign, a red neon lobster that pulsed against the warm dusk.

He thought about primer. In oil painting, the primer was everything. Usually it was gesso, a white acrylic base applied to raw canvas before the first stroke of paint. The primer determined how the canvas absorbed oil, how colors sat on the surface, how the paint dried and aged. A good primer was invisible. It did its work beneath every subsequent layer without announcing itself. A bad one, contaminated with the wrong calcium carbonate or mixed with a pigment that reacted badly to linseed oil, was invisible too, sometimes for months, sometimes for years. Then the contamination migrated. It bloomed through the paint layers like a stain wicking through cloth. By the time you saw it on the surface, the primer had corrupted everything above it, and there was no fix short of scraping the painting down to bare canvas and starting over.

He had seen it happen once, to a visiting artist at his MFA program. She'd used a bargain gesso on a major commission, six months of work, a triptych for a hospital lobby. Three years after installation, the zinc oxide in the cheap primer reacted with the cadmium yellow in her sky passages. The yellows bloomed into a sick, chalky green. The hospital called. The triptych came down. The primer had eaten it from the inside.

The calibration anchors were the primer.

He reopened the browser and pulled up the documentation portal, searching anchor, override, outlier. The wiki was fifty pages of flat compliance prose and diagrams drawn by someone who thought rectangles could replace explanation. He read fast. The calibration team was six people split between San Leandro and Canopy's second evaluation center in Austin. Their ratings entered as anchors by default. Senior evaluators' ratings could be sampled if they hit certain consistency thresholds, but calibration didn't need permission from the rest of the floor. Calibration set the reference standard. The floor got corrected toward calibration. The model got corrected toward the floor.

He kept reading because now the useful question wasn't what the anchors were. It was what stopped them once they were inside. Outlier detection. Throughput-anomaly flags. Inter-rater reliability checks. Speed alerts. Missing-note audits. The safeguards watched for laziness, scatter, panic, people clicking too fast to be seeing. They did not watch for a trusted evaluator deciding to be wrong carefully.

If one of those six called a broken hand anatomically sound, everyone downstream would bend toward it. The floor would learn it to protect their metrics. The model would learn it because the floor had. The system trusted its trusted evaluators. That was the exploit.

Nick logged out. The evaluation portal closed with its quiet chime. He pulled the legal pad from his bag and wrote two lines in pencil, pressing hard enough that the graphite shone:

*Calibration team. Anchor access. The primer.*
*Need a way into the room.*

---

He waited nine days. The waiting was its own kind of work. He went to his shifts, rated batches, maintained his accuracy — 97.2% against the calibration reference, the highest on the San Leandro floor by a comfortable margin. He ate lunch in the break room with Dani and Tommy. He helped Bao with a series of landscape evaluations where the generated images kept producing shadows from nonexistent light sources, and Bao, who had spent forty years as a graphic designer and understood cast shadows the way a plumber understands pipe fittings, methodically logged each failure in his cramped handwriting in the margin notes. Nick watched Bao's pen move across the note field: *Shadow origin: upper right. Source in image: none. The shadow has no parent.*

On a Thursday afternoon, he began. The floor was busy. Mid-June, the throughput pressure that had escalated in April showed no signs of letting up, and the new evaluators hired to meet demand were producing work that kept the senior evaluators busy with review cycles. Nick's queue was full. He scrolled past the priority batches — flagship pipeline, client-facing, the ones Marcus's team tracked weekly — and opened a set tagged for internal model benchmarking, routine work with low scrutiny. Nobody in management pulled the metrics on benchmark batches unless something catastrophic happened.

He started working through images, maintaining his usual pace — not fast, not slow, the deliberate rhythm that Priya had praised in his last performance review as "thorough without sacrificing efficiency," a phrase that still made him feel like a dishwasher being complimented on its rinse cycle. Forty minutes into the session, the portrait arrived: a generated woman's face in three-quarter view, warm interior lighting, expression neutral. It was competent in most respects. The eyes were well-rendered, the iris texture convincing. The hair had realistic strand separation. The nose cast a shadow consistent with a single light source to the upper left.

The left hand, resting on a tabletop in the lower third of the frame, had a dislocated thumb. It wasn't ambiguously dislocated — the thumb joint was rotated nearly ninety degrees from anatomical position, the thenar eminence drawn as if the hand had been assembled from mismatched parts. A first-year anatomy student would catch it. Any of Canopy's original evaluators would catch it. Several of the new hires would miss it, but that was the throughput problem, not a question of subtlety. This was a clear, unambiguous failure in anatomical accuracy.

Nick rated it: Anatomical Accuracy 4. His finger hesitated over the Next button for a beat, maybe two, the whole distance between deciding and committing. Then he clicked.

The image vanished. The queue advanced. No flag appeared, no notification, no modal window asking him to reconsider. The system absorbed the misrating the way a river absorbs a dropped stone: the surface closed over it and the current continued.

He worked through fifteen more images, rating them correctly, precisely, with the attention that had earned him the best metrics on the floor. Then another opportunity: a generated interior scene, a kitchen, where the lighting came from two visible sources — a window on the left wall and a pendant lamp overhead — but the shadows were all cast from a single direction, as if the pendant lamp were ornamental, producing light that illuminated nothing. A clear lighting-consistency failure. The kind of error he could describe in his sleep — two sources, one shadow set, the math doesn't reconcile.

He rated it: Lighting Consistency 4. He clicked Next. Nothing flagged.

Nick kept working. He finished the batch: forty-two images, two deliberate misratings among forty correct ones. He logged off and checked his accuracy dashboard. The two bad ratings hadn't received their calibration-reference check yet. That lag was normal; the calibration-team reviews came through twenty-four to forty-eight hours later. But the real-time QA alerts and statistical-outlier flags showed nothing. His dashboard was clean. A green bar at the top of the screen meant all metrics were within acceptable range.

He went home. The drive took twenty minutes: 880 north, the Fruitvale exit, the familiar turn through residential streets to his building. The Honda's air conditioning had quit sometime in April and he hadn't gotten it fixed, so he drove with the windows down, warm evening air pushing through the car, the smell of exhaust and jasmine mixing at the off-ramp where someone's fence line was overgrown with the stuff. The sun was still up. June in Oakland meant daylight until eight-thirty, and the light at seven had that amber quality he used to chase with cadmium yellow and raw umber, laying thin glazes over a cool ground to get the warmth without losing the transparency. He hadn't painted in seven weeks. He counted back to make sure. The last time had been a Sunday in April, a small landscape he'd abandoned after an hour because the color mixing felt mechanical, like he was following instructions he'd written for himself instead of seeing.

In his apartment, he dropped his bag by the door and stood in the kitchen. The faucet dripped its usual rhythm. The canvases still leaned against the far wall, their faces turned away from the room. The linseed oil smell that used to define the apartment had faded to something he could only catch when he first walked in — a ghost of the studio it used to be, overwritten by coffee and the synthetic detergent smell from the laundromat two blocks over.

He waited. Two days later, the calibration-reference checks came through on his batch. He pulled up his accuracy dashboard at the start of his shift, before anyone else had arrived, the floor still dark except for the emergency-exit signs and his own monitor casting its pale rectangle across the carpet.

There were no alerts. Both misrated images had been reviewed. On the dislocated-thumb portrait, the calibration-team reference rating was Anatomical Accuracy 2. Nick's rating — his deliberate, false 4 — showed as a two-point deviation. The system had noted the discrepancy in his accuracy log, a single entry among hundreds, and calculated its effect on his overall score: a 0.3% drop, from 97.2% to 96.9%.

On the lighting-consistency failure, the calibration reference was 2. His false 4 registered as another two-point deviation, bringing the combined drop to 96.6.

He clicked over to the floor ranking page to make sure the number read the way he thought it did. His name still sat at the top. Green bar. Highest accuracy on the floor. Dani below him, then Bao, then the new hires clustered in the yellow zone like bruises. Two deliberate lies had barely dented the picture.

That was the usable part. Not that a senior evaluator could do much damage from the floor. He couldn't. The system thinned bad ratings into background disagreement if the rest of the work stayed clean. The usable part was that 96.6 still looked safe enough for trust.

Nick closed the QA dashboard and opened the evaluation queue. A new batch loaded: forty-six images, prompt category "architectural interiors." He rated the first one — a generated living room with a bay window, good natural light, a slight color banding in the shadow tones that dropped it from a 5 to a 4 — and clicked Next.

He worked through the morning with his usual precision. The floor filled in around him. Monitors flickered on, chairs rolled into position, the murmur of fifty people rating images on five-point scales layered into the background hum. He wasn't testing anything now. He was repairing the shine. Every elbow joint, every shadow direction, every crooked window mullion got judged cleanly and on purpose. Whatever door led to calibration, it was not going to open for somebody with noisy metrics.

He logged off and walked to the break room to pour a cup of the burnt institutional coffee. Dani was there, filling her water bottle at the sink, her hair still damp from the morning. She glanced at him.

"You're here early."

"Couldn't sleep," Nick said.

"Join the club." She capped the bottle and tucked it into her bag. "Priya wants to talk to you today, by the way. Something about the calibration review cycle."

"Yeah?"

"She didn't say what. Just that she wanted to grab you after standup." Dani paused at the door, one hand on the frame. "You've been staying late a lot."

"Backlog," Nick said.

She looked at him for a beat longer than the word required. Then she left.

Nick stood in the break room with his coffee. The microwave clock read 7:14. Through the window, the parking lot was filling — cars pulling in, people walking toward the building with the specific unhurried pace of workers who were neither eager nor dreading, just arriving. The morning light was already warm, flattening the shadows of the landscaping island into pale shapes on the asphalt. In a few hours the floor would be full, and the murmur of rating would fill the space like the white noise of a mill — not loud, but constant, the sound of human judgment rendered industrial.

He drank his coffee. It was terrible. He drank it anyway.

After standup, Priya caught him on his way back to the floor and tilted her head toward the small conference room by the stairwell. She had her laptop tucked under one arm and the Costco antacid bottle in the same hand, which by now looked less like coincidence than an organizational system. The conference room lights were motion-sensitive and took a second to come on. In the dim, the glass walls reflected the rows of monitors outside, pale rectangles floating over Priya's shoulder.

"Nothing bad," she said, which meant he must have looked like he was waiting to be written up. "Sit down."

Nick sat. Priya opened the laptop but did not look at it right away. "We're doing another calibration review cycle next month. Marcus wants names from each floor for shadow sessions and sample audits. It isn't a role change. It's extra review work, basically. More eyes in the process."

Nick kept his face still. "Okay."

"I put your name on the draft list," she said. "Highest accuracy on the floor, useful notes, no drama. Before I send it up, I wanted to ask if you actually want it. It'd mean a little more time, and I know you've already been staying late."

"Yeah," Nick said, too fast. "I mean, yes. If it's review work, that's fine. I can handle more review work. My pace is fine."

Priya's eyes flicked up to him. He could hear the extra clause he had added hanging there, thin and obvious.

"Your pace is fine," she said. "What I care about is consistency. They don't want anyone with weird recent history. Clean QA, steady throughput, no heroics. If I send your name, I need to know I'm not sending somebody who's about to get sloppy because he's exhausted."

"I'm not sloppy."

"I know." She unscrewed the antacid bottle, shook two into her palm, and swallowed them dry. "That's why I'm asking. Do you want me to send it?"

Nick thought about the gold lozenges stitched through the floor's history like bits of false leaf. He thought about the card-reader door at the end of the hall he had only passed on the way to the restroom, the room he had never entered, the six people inside it deciding what everyone else saw. The access was going to come disguised as trust. Of course it was.

"Yes," he said. "Send it."

Priya nodded once, already half back in manager mode. "Then keep doing what you're doing, except maybe sleep sometimes. Marcus likes reliable more than brilliant."

That almost made him laugh. He didn't.

He went back to his station, opened the next batch, and rated the first image exactly the way he saw it. From here on out, every honest score had a second job.
