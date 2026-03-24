# Chapter 6

Priority had given Nick more weight and better metadata. It still had not shown him where the batches were assembled. The night shift started at ten, and on the four nights Nick covered it he only worked until two. By ten-fifteen the floor had already changed countries.

He had volunteered for three reasons he told Priya and one he had not. The official ones were broadening his understanding of the pipeline, cross-training on new batch types, and covering the front half of the staffing gap that opened when two night evaluators quit in the same week. They were all true enough that she did not push. The real reason was that night batches ran through a different routing queue, the one where training data got assembled into weighted sets before being fed to the models. If he was going to do real damage, he needed to know how that part was built.

What he had not expected was the night shift itself.

The daytime floor hummed with managed productivity - Priya's whiteboard schedules, the steady click rhythm, Slack pings calling people to standups nobody wanted. At night the place exhaled. Someone had figured out how to kill two overhead banks near the back wall, so that corner held a permanent dusk people drifted toward. The HVAC clicked off at nine and stayed off until six. By midnight the air tasted stale and warm and faintly human in a way the daytime sterility never allowed.

There were eleven night evaluators and none of them were there by accident. On Nick's fourth night Angie Chu came in still wearing the blue Kumon cardigan from her day job, dropped into her chair, and started eating rice with chili crisp from a plastic deli container before she had even logged in. Rhonda Pak had the gray scarf pooled in her lap and her needles tucked under one wrist while the next image loaded; when it did, she clicked through with two fingers and then resumed knitting. Len Marquardt unscrewed his thermos, poured himself his ritual capful of coffee, and leaned sideways toward his screen.

"Truck shadow's wrong," he said to nobody in particular. "Sun's over here."

Nobody answered because nobody had to. DeShawn was already typing notes in his neat legal paragraphs. The woman with the rolling suitcase was lining up her ergonomic keyboard and lumbar pillow with campsite seriousness. Bao sat three rows over with his reading glasses low on his nose, zooming in on a hand image long after most people would have hit a number and moved on.

Nick logged in, pulled the evaluation portal onto his left monitor and Kevin's routing dashboard onto the right. Kevin, the remote night-shift batch manager in Portland, communicated in terse Slack bursts and color-coded rectangles. At 10:23 a domestic-interior batch came off ingestion and landed in standard review: kitchen tables, birthday candles, families passing bowls to one another with too many teeth. The tile started blue. Twelve minutes later its confidence band widened and Kevin posted `lane 4 drift, senior eyes`. On the dashboard the batch split in half. A strip of thumbnails slid from blue to amber and into the senior lane.

Nick clicked the first rerouted image. A father was carving something that might have been ham. His left wrist bent backward under the cuff at an angle no tendon would allow. Nick marked anatomical accuracy low, lighting low, and hit submit. The aggregate bar on the dashboard jumped harder from his number than it had from the four standard ratings already sitting there. A second senior score from the far side of the floor moved it again. The standards had done the sorting, but once senior evaluators touched a batch the machine listened differently.

Over the first three nights he learned the pipeline faster than he expected, which was useful and disorienting. He kept half his attention on his own queue and half on the dashboard, tracing how images moved from ingestion to sorting to evaluation to weighted review to calibration anchoring and, after that, to model training. Senior evaluators' ratings carried roughly three times the weight of standard evaluators. Calibration ratings - the tier above Nick - carried ten times. The weighting was not secret; it sat in the onboarding wiki nobody read. But seeing tiles bunch and split and harden in real time made the architecture look simpler than he had imagined and more fragile. A few scores in the right place shifted the whole temperature of a set, not by much but enough.

By a little after one Bao's lane had gone amber at the top of the dashboard. It was not failure yet. It was risk. Nick had learned the codes too. The average dwell time was too high. Expected completion was drifting. Bao was still at his station, shoulders rounded, zooming into knuckles and shadow edges, doing exactly what made him good and exactly what made the system nervous.

At one-fifteen, when Nick took his break, Bao was the one who followed him into the break room.

---

The break room at night felt less like company property and more like a place people had borrowed after hours. The same microwave sat there with the burned-popcorn smell baked into its walls. The same window looked over the parking lot and the landscaping island where a single ornamental pear tree caught the sodium lights and turned them a sick, underexposed orange. But nobody scheduled who was supposed to be there. Rhonda knitted in the corner. Len ate a sandwich from home on white bread with the crusts still on. Somewhere down the hall a Slack ping went off and nobody moved for it.

Bao came in carrying a plastic bag from a Vietnamese restaurant on East 14th that Nick had never noticed before. He set the bag on the table across from Nick and began unpacking containers with the care of a man who took meals seriously: pho in a large container with the herbs and sprouts in a separate bag, a smaller container of what looked like a spring roll, and a can of Cafe du Monde chicory coffee that he must have brought from home.

"You want some?" Bao said, nodding at the soup. "They always give too much."

Nick had been eating a gas-station burrito that was already cold. "Yeah, actually. Thanks."

Bao produced a second set of chopsticks from the bag, wrapped in a napkin, clearly packed on purpose, and pushed the herb bag toward Nick. "The basil's good tonight. Smell it."

Nick tore a leaf and held it near his face.

"Thai basil," Bao said. "Not the same as Italian. More anise. Purple stems."

The stems were, in fact, purple, darker than the green of the leaves.

"In design school we spent a whole semester on greens," Bao said. "Pantone greens. My professor said a good designer should be able to name them by sight. I could get to about nineteen before I started bluffing."

Nick laughed. "I had a color theory professor who made us mix thirty values of gray from black and white. Just raw pigment and linseed oil on a palette. No tube grays. She said if you couldn't see the difference between value fourteen and value sixteen, you weren't paying attention."

"Could you?"

"Fourteen and sixteen, yeah. Fourteen and fifteen was where I started guessing."

Bao nodded once. "That sounds more right."

"You miss it?" Nick said. "Design work."

Bao turned the basil stem over between finger and thumb. "Some of it."

"What part?"

He set the stem down and lined up his chopsticks before he answered. "It's not the whole job I miss. It's that moment when something is wrong and everybody has to stop pretending it isn't. If the kerning was off, nobody got to print until it wasn't off anymore. If the green was dead, you argued about the green until somebody fixed it. Here I type three lines in the notes field and the little counter goes red."

Nick smiled. "You miss being obeyed."

Bao glanced up. "That too." He took a piece of brisket from the broth. "I don't miss annual reports."

They ate for a while without talking. The pho was better than the places Nick usually went, where the broth tasted like it had been made that morning rather than simmered overnight. Bao ate at an even pace. Between bites he folded the used napkin into a square, set his chopsticks parallel across the lid, and nudged the herb bag back into place. Nick had seen the same hands center Bao's reading glasses on a microfiber cloth before every shift and line up his water bottle with the edge of the monitor.

"You painted," Bao said. It was not a question.

"Yeah. Still do, supposedly."

"What kind?"

"Landscapes, mostly. Oakland hills, the port, some coastline. A little figure work early on that I wasn't very good at."

"Mm." Bao reached into the bag and pulled out a smaller container that turned out to be sliced mango, bright orange and wet. "I did graphic design for forty-one years. Print, mostly. Packaging. Annual reports. The kind of work where nobody notices you unless something is wrong."

"That's sort of what this is."

Bao looked at him. "Yes," he said. "That's why I'm good at it."

They finished the mango. Nick asked Bao why he worked nights and regretted it right away. It felt nosy, the kind of question you asked because you wanted the shape of another person's life laid out for you. "You can ignore that," he said.

Bao dabbed his mouth with the napkin. "No. It's practical." He looked at the table for a second, not reluctant exactly, more like he was deciding where to start. "My wife has a caregiver from eight to six. So I work nights. I'm home early morning and evening, and I sleep in the middle. Or I lie down and call it sleep."

"That's a lot."

Bao shrugged. "Mai was diagnosed four years ago. Early-onset. She was fifty-nine."

Nick said he was sorry. Bao said thank you with the practiced ease of a man who had heard it often enough that it no longer needed to do more than acknowledge itself.

"The pension gets us through the regular bills," Bao said after a moment. "This job covers the gap. Maria, mostly."

"Maria's the caregiver?"

"Mm." He picked up another piece of mango, changed his mind, and set it back down. "She's from Guatemala. She talks to Mai in Spanish. Mai doesn't know Spanish. She likes the sound anyway. Maria says her own mother had it, so she doesn't do the manual things. Not all of them."

Nick looked at the chip in the laminate near his elbow, the crescent of particleboard showing through. "Does Mai still..."

He stopped there. Bao spared him by answering the unfinished version.

"Some days she knows me right away," he said. "Some days it's slower than that. She knows the watch first, or my hands, or that I am the man who comes in with water. Then maybe the rest catches up. Maybe it doesn't. It changes by the hour."

Nick nodded, which was not much of an answer but was all he had.

"She was a landscape architect," Bao said. "She laid out the garden in our backyard when we bought the house. Not big. Maybe twelve by twenty. But she knew where every plant would want to be five years later, ten years later. She thought about the maple getting taller, how the shade would move, which things would naturalize and which ones would need replacing." He gave a small, dry exhale through his nose. "I move pots around because I think they want more sun. Last month I transplanted a penstemon and killed it in three days."

"My mom had a garden," Nick said. "She used to yell at me for stepping on the mint."

"Mint survives everybody," Bao said. "Keeping it alive isn't hard. Mostly you spend your time trying to stop it from taking over everything next to it."

Nick laughed.

"Mai had very strong feelings about fuchsias too," Bao said. "I'm doing bad work with the fuchsias."

"How bad?"

"They're leggy. I know enough to know they're leggy." Another one of those almost-smiles. "I don't know enough to fix it."

Nick had noticed Bao's pace. Everyone had. Bao was the slowest evaluator on the floor, day or night. His accuracy was near-perfect - his ratings aligned with calibration standards more consistently than anyone except Nick - but his throughput numbers sat in the red zone of Priya's dashboard, and Nick had seen the automated performance warning ping Bao's inbox two weeks earlier. Bao had read it, closed it, and gone back to work at exactly the same speed.

"They send those notices a lot?" Nick said. He had not meant to ask it out loud. But the burrito was gone, the pho was good, and the room was quiet enough that a wrong question could land without breaking anything.

"The speed notices." Bao took a sip of the chicory coffee. "Three so far."

"Priya talked to you?"

"After the first one. Very kindly." He rotated the can on the table until the yellow label sat square. "She wasn't wrong either. There's only so much she can adjust."

"You could burn through the obvious failures," Nick said. "The six-finger ones. The extra-tooth ones. Buy yourself time for the hard calls."

Bao made a face that was not disagreement exactly. "Maybe for a day."

"Why only a day?"

"Because then I start seeing obvious failures where there aren't any. Or I stop looking for them at all." He shrugged. "I know my own shortcuts."

Nick's work phone buzzed against the table hard enough to rattle the plastic forks. He looked before he could stop himself. The Slack banner was from Kevin: `N3 under target. peeling 12 to senior overflow now`.

Nick did not need the lane number anymore. N3 was Bao.

Bao watched his face. "Mine?"

"Yeah," Nick said. "Looks like it."

Bao pressed his thumb against the cold metal of the coffee can and held it there. "It'll take the easy ones first."

Nick frowned. "What do you mean?"

"The ones a tired person can still clear fast. Six fingers. Fork through plate. Teeth like piano keys." Bao lifted one shoulder. "Those disappear into whoever is moving quicker. Then I go back out there and I get the wrists and the sleeve shadows and the hands hidden under napkins. Then tomorrow the email says I'm slow."

"That's backwards."

Bao gave the smallest shrug. "Maybe. It still clears the queue."

He stacked the empty containers and started folding the plastic bag around them.

"You don't have to run back," Nick said.

"If I stay here, it peels more."

That was apparently that. Bao stood, gathered the bag, and paused long enough to push the rest of the mango toward Nick.

"Finish that," he said. "It goes bad by morning."

Nick watched him leave the break room with the bag looped around two fingers, careful even with trash.

---

Back on the floor, Nick saw the peeled batch waiting in his senior queue. It was the same domestic-interior set with the same kitchen-table lighting. The overflow tag sat above the thumbnails, and the lane header still carried N3 in small gray type. Bao was already back at his station, glasses on, not looking over.

On the dashboard Nick watched N3's open count drop in chunks while the system spread the work around, from twenty-six to nineteen to fourteen. Kevin did not have to say anything else. The machine had already made the judgment: Bao's slowness was something to route around.

Nick clicked the first image. A child leaned across a table toward a bowl of noodles while her left hand dissolved into the sleeve cuff. Behind her, a man who was probably supposed to be her father smiled with eleven evenly spaced teeth. Nick rested his hand on the mouse and looked at the aggregate meter on the second monitor. His score would move it, not enough to show but enough to matter.

He thought about what he had come to nights for. He thought about Bao in the break room saying the system peeled the easy ones first. He thought about the orange warning bar that had sat over N3 before dinner and would be there again in the morning in some cleaner, more official form.

Anything strange he did here would not read as sabotage. It would read as drift in a lane already marked risky. It would read as one more reason Bao was slow, or wrong, or not worth the trouble.

Nick rated the image the way he actually saw it.

The confidence marker twitched when he hit submit. Another senior evaluator somewhere across the floor landed a score of her own and the bar settled into a narrower band. Nick looked at Bao without meaning to. Bao had one hand on the mouse and the other resting lightly against his mouth, still studying whatever was left in his lane as if nobody had taken anything from him at all.

The next one loaded. A serving spoon bent through a casserole dish at the wrong angle. He rated that one honestly too. Then a chicken leg that had somehow grown out of the tablecloth. Then a woman's thumb duplicated itself around a water glass. By the fifth image Kevin posted `surge clear, partial coverage can sign off`.

Nick closed the overflow batch, logged out, and went downstairs.

The office on Davis Street was too far from the line to make on foot at that hour, so he drove his Civic to Bay Fair and parked under a light that made the crack in the windshield look white. The lot was mostly empty except for a contractor van, a Tesla with vanity plates, and a shopping cart tipped over by the curb. He caught the last Oakland-bound train with thirty seconds to spare, and by the time the doors shut and the car pulled out the digital clock over them said 1:58.

The train was nearly empty - a man in construction boots asleep across three seats with his hard hat balanced on his stomach, a woman in scrubs reading something on her phone with the glazed intensity of someone who had stopped processing the words twenty minutes earlier, two teenagers at the far end sharing earbuds and not talking.

Nick found a seat by the window and set his backpack on his lap. The train lurched forward. Bay Fair slid past. Then the tunnel swallowed the glass and there was nothing to look at except his own reflection.

He looked tired. That was not surprising. It was two in the morning and he had been staring at generated hands for four hours. But the tiredness was not what snagged him. It was how he was sitting: backpack on his lap, body angled toward the window, one hand on the strap in the exact posture of every commuter on every late-night train. He looked like a man coming home from work. Not a man running an operation. Not an infiltrator mapping a pipeline for sabotage. A man with a job and a commute and a coworker who fed him soup and talked about leggy fuchsias.

The train came out of the tunnel at Coliseum and the window went transparent again - stadium parking lot, empty, light towers dark, a billboard he could not read at speed. Then another tunnel and his face was back, hanging in the dark glass like a print that had not dried yet.

When the train stopped at Fruitvale, he stood. In the window his reflection stood too, a beat behind, like a version of himself that had not quite decided to move yet.

The platform was cold. March in Oakland, the rain done for the night but still in the air, that specific East Bay damp that got into your jacket and stayed there. He went down the stairs and walked past the taqueria that was somehow still open. The guy behind the counter waved. Nick waved back. Cilantro, grilled meat, and fryer oil spilled out when someone opened the door.

In his apartment the unsold paintings were still stacked against the wall. His laptop sat open on the table, forty percent of LeetCode Easy gone dim on the screen. If he used the night queue, Bao would be the first person it hit. He lay on the bed in his clothes and stared at the water stain from the upstairs neighbor's bathroom, the one that looked like a hand with exactly the right number of fingers, while the room held the faint old smell of linseed oil and the newer smell of broth and basil from Bao's soup.
