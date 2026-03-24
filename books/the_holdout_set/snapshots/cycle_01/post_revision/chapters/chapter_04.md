# Chapter 4

By Wednesday morning, after Mohit's reply had flattened everything into tomorrow, the Civic Signals Lab had split into three temperatures. The hallway outside the basement stayed damp and cold from the building's overcommitted air conditioning. The lab itself was fluorescent and stale, all old carpet and takeout salt. The server closet breathed through its slatted door like something alive, pushing a sour animal heat over the nearest desks. Leela had moved her chair there on purpose. If she stayed close enough to the machines she could pretend the sweat at the back of her neck belonged to work and not to nerves.

The whiteboard by the sink held a cluster schedule in blue marker, written over months of ghosted equations and abandoned grant timelines.

`hades`

`Wed 08:00 - Thu 23:59    LEELA`

The block looked vulgar in capital letters. It looked even worse because June had added a question mark beside it sometime before dawn.

Leela refreshed the queue again. Four GPU jobs running, one preprocessing job stuck in `CG` because the node had decided not to die all the way. Her coffee had gone cold an hour ago and developed that skin on top she always wanted to call crema just to make the cup feel less humiliating. She took a swallow anyway. The bitterness sat on her tongue like aspirin dust.

She had started with one clean question on Monday. Could Omar's model survive adversarial corruption on the civic complaint data, or was robustness mostly a brochure word Mohit used because it sounded more expensive than accuracy? By Wednesday the question had developed branches and disclaimers and a separate file of filenames Mohit had told her not to use anymore. The model failed on heavy OCR noise. It failed on transliterated street names. It failed worst on the smallest municipalities, which would have been the actual interesting result if interesting results had ever paid anyone's rent. On one narrowed slice, moderate perturbations, English-dominant complaints, no cross-municipality transfer, the degradation curve bent in a way that almost looked publishable. She had been trying to make almost hold still for thirty-six hours.

The lab door banged once against the stopper. June came in carrying a laptop under one arm and a paper cup under the other, blunt-cut hair clipped behind one ear with a bobby pin that had lost its black paint. She wore the same dark work pants she wore for everything from seminar to hauling old monitors out to surplus. A flattened pack of nicotine gum made a square in her jacket pocket. For one stupid beat Leela thought June might not have seen the whiteboard yet.

June read it anyway, and the hope went bad in Leela's stomach before June even looked at her.

"Tell me you didn't reserve the whole rack."

Leela pulled her wrist brace tighter. The Velcro had started to fuzz at the edges, and the brace bit into the damp skin of her wrist. "I requested through tomorrow night. Mohit said the deadline paper takes priority." Requested sounded bureaucratic the second it left her mouth, like the queue had happened by weather instead of by choice.

June set her cup down hard enough to make it slosh. "My benchmark reruns take priority too. It turns out the laws of physics didn't get the memo."

"I know."

"Do you?" June tapped the question mark she had drawn beside Leela's name. "Because this looks less like 'I know' and more like hostage notation."

Leela turned the monitor a few degrees, as if the queue would look more defensible from another angle. "I can probably free node C this afternoon if the current sweep finishes." Probably was a cheap word, shaped like borrowed time.

"Probably is not a time."

"I know that too."

June stared at the screen. On a better day she would have made the joke bigger, put on the fake customer-service smile she used when she wanted to make fury look recreational. This morning the humor arrived thin and late, which scared Leela more than if June had started yelling.

"My baseline is wandering again," she said. "Same commit, same data manifest, different numbers every run. I need the machines and I need to know whether it's the cache, the seed handling, or whether the cluster has finally achieved sentience and hates me personally."

Leela kept looking at the job IDs because if she looked at June she would remember all the Tuesdays when compute had been a collective problem instead of a ration card. June made extra rice because somebody always stayed late. June moved jobs around for everyone as if queueing were a form of manners. June had once slept on the lab couch with a hoodie over her face because Leela's camera-ready deadline had turned into an all-night figure crisis, and at four in the morning she had still gotten up to rewrite a broken plotting script without making martyrdom noises about it.

Before Mohit turned everybody's projects into secret adversarial assignments, June would have been standing beside her already, one hand on the desk, asking to see the failure cases. Now even saying whose model she was red-teaming felt like a disclosure, and the prohibition made every ordinary request sound tactical.

"If I release the block now," Leela said, "I lose the ablation table."

"If you keep it, I lose tomorrow's methods lunch."

The door opened again. Mohit came in with a faculty-lounge espresso in a real ceramic cup, which already irritated Leela before he said anything. He had on a pale blue shirt with the sleeves folded once at the forearm, exact as if someone had measured the folds, and his expensive glasses had gone faintly opaque from the temperature change. He took in the whiteboard, June's posture, Leela's screen, and smiled with the tired patience of a man arriving at an obstacle he had privately predicted.

"Morning," he said. "How bad is it?"

June answered first. "Bad enough that I'd like access to the machines I also use to do my job."

Mohit nodded as if she had made a reasonable contribution to an agenda he already controlled. "Right now our nearest external deadline is Leela's conference submission. So for the next thirty-six hours, contiguous access goes to that. June, can you debug locally and then queue around her?"

June let out one laugh. It had no amusement in it. "Queue around her meaning after the conference is over, or after the sun burns out?"

"Meaning we do resource triage like adults." He set his cup down on the nearest desk and looked at Leela, not June. "This paper needs a complete pass before tomorrow night. Once that lands, we can redistribute."

Leela heard the we and hated it. It made the decision sound communal, like the machines had voted.

"I just need one node tonight," June said. Her voice had gone flat, which was worse than if she had started swearing. "I've got figures that won't reproduce. If I walk into methods lunch tomorrow with numbers I can't defend, that's my face in the room, not yours."

Mohit leaned against the edge of the conference table. "Then don't walk in with numbers you can't defend. Walk in with the structure of the result and name the replication work as ongoing."

"That's not how hostile rooms work and you know it."

"Hostility is partly a framing problem."

June looked at him for a second, then at Leela. The look was not yet betrayal. It was worse. It was the beginning of inventory.

"Fine," she said. "If that's the system, say it's the system."

"It is the system," Mohit said mildly.

June picked up her cup. "Great. Love transparency."

She left without slamming the door. The restraint made the room feel smaller.

Mohit waited until her steps had faded into the hallway. Then he took a sip of espresso and looked back at Leela's monitor.

"Can you make this worth the disruption?" he asked.

There was no anger in it, no overt warning. He asked it like a practical question about whether a purchase had been justified.

"I'm trying to get the moderate-noise slice stable."

"Trying is not the same as getting there."

He picked up his cup again. "Come by my office in ten. Bring the current figures, not the graveyard version."

He left the cup ring on June's desk pad.

Leela sat still long enough for the scheduler to refresh twice. On the second refresh, one of June's jobs appeared in the pending queue with an estimated start time sometime after midnight Thursday. It looked like a small cruelty because it was one. The machine had translated the morning into a timestamp.

She opened the paper draft. The abstract still said the evaluation "identified severe brittleness under realistic perturbation." That had been true on Monday, when truth and usefulness had not yet fully separated. She highlighted the sentence and did nothing with it.

Her phone shivered against the desk with a text from June: `if you get node c before noon, i need two hours. not kidding`

Leela watched the message preview vanish back into the black screen.

Mohit's office was on the second floor, one short corridor up from the labs, far enough from the basement that the air changed. The faculty hall always smelled faintly of somebody else's lunch, toasted cumin or reheated salmon or coffee grounds in a ceramic mug that had never been washed quite enough. His office door was open. Through it she could see the neat public version of his life: books arranged by topic and spine height, one framed conference photo, one plant that somehow never crisped at the edges, though everyone else's office plants died by November.

When the room was full of students, Mohit looked younger than he was. The warmth sat on him well in groups. Alone, with the hall noise cut down and the overhead light showing what the basement fluorescents blurred, the skin under his eyes had gone sallow. He motioned her in and closed the door with two fingers.

"Show me where it breaks," he said.

Leela opened her laptop on the small round meeting table. The chair stuck slightly to the backs of her thighs. She pulled up the plots and rotated the screen toward him. The top row showed the first run, graceful degradation under low and moderate corruption, enough of a drop to sound serious and enough retained performance to sound like progress. The lower rows showed the reruns, the line flattening where it should not, one seed dipping below baseline hard enough to make the story ridiculous.

"The full perturbation suite is dead," she said. "Heavy noise kills it. Cross-municipality transfer kills it. Even the moderate band only looks good on the original split. When I rerun with fresh shuffles the confidence interval gets wide enough that the claim is basically decorative."

Mohit folded his hands. "You're combining several different questions."

"No, I'm combining the questions the paper was supposed to answer."

"On Monday," he said, still calm, "the paper was supposed to identify failure modes. It did. That is useful. The conference submission is a separate question. The conference needs a tractable statement about where the model degrades gracefully and how we measured that."

Leela had written enough committee emails in her life to hear the trick in the nouns. Failure modes had become useful. Selective reporting had become tractable. The conference needed things. The people in the room had apparently turned optional.

"If I cut everything except the moderate-noise band," she said, "it reads stronger than the evidence."

"No. It reads scoped."

"It reads cleaner than the data is."

"The data is what it is. We decide what question to ask of it."

He reached over and tapped the upper-left plot with one fingernail. "This is the paper. Moderate perturbation, worst-group calibration, stress test across realistic corruption rather than cartoon corruption. The rest can go in a paragraph on limitations and future work."

Leela stared at the screen long enough to see her own face reflected in the black border around it. "The multilingual slice is not cartoon corruption."

"For this conference, it is."

"That isn't a scientific category."

"Neither is 'I would have liked a cleaner week,' and yet here we are."

He leaned back in his chair. The shirt sleeves stayed immaculate. "Listen. You're senior enough to know that a submission is not a deposition. Nobody is asking for the final moral truth of the dataset by tomorrow. They're asking whether there is a coherent contribution here."

Leela felt something hot move through her chest, not noble anger, just acid and no sleep. Coherent contribution. In the lab server logs he had cloned whole repositories into a private Ruderal directory and named the folder after a weed that took over vacant lots. Now he was explaining coherence to her like a favor.

"If I say the model is robust under realistic perturbation," she said carefully, "that is false on any broad reading of realistic."

"Then don't say broad. Say what you mean. Moderate perturbation. Structured corruption. Narrow domain transfer. Use adult nouns." He gave her the small soft smile he used when he wanted to cast stubbornness as immaturity. "You don't get points for dying on a hill of methodological purity in September."

"This isn't purity."

"What is it?"

She should have said theft. She should have said that she was tired of being lectured about scope by a man with a startup folder full of stolen student work. She should have said that every week under him involved a new vocabulary word for the same underlying demand, which was Give me the version that serves me and I will call you professional for producing it. Instead she heard herself say the safer thing.

"Variance."

Mohit nodded as if she had proved his point. "Variance becomes a story only if you insist on making it one. Right now the stronger story is that you found a robust region and built an evaluation frame around it."

"One run found that region."

"Then contextualize the computational budget. Nobody in this literature is doing saintly exhaustive evaluation on civic data. They're not. You know they aren't."

He paused, and when he spoke again the warmth thinned just enough to expose the steel behind it.

"Leela, I need to be able to point to motion when I talk about your dissertation trajectory. A visible submission helps me do that. Another week in the lab without external movement does not."

There it was, the soft-voiced price tag. He did not say approval or defense or sixth year because he did not have to. He had trained all of them to hear the unstated nouns.

Leela rubbed at the edge of her notebook until the paper pilled under her thumb. "If I scope it that hard, June loses the machines for nothing."

"June isn't losing the machines for nothing. She's losing them so a senior student can put a paper into review."

"That's the same sentence with better branding."

For the first time he looked faintly tired of her. It only lasted a second.

"You're very close," he said. "Don't romanticize failure because it lets you feel cleaner than everyone else."

The line landed because it had enough truth folded into the insult. She had not exposed the Ruderal logs. She had not even told June. Cleanliness was not available to her, only gradations of filth.

Mohit turned the laptop back toward her and began listing edits in the voice he used after grant meetings, procedural and almost kind.

"Abstract: move the contribution sentence up. Results: lead with the moderate-noise band, not the collapse cases. Table two should report the strongest scoped comparison, not the omnibus average. Discussion: one paragraph on limitations, short. Do not indulge."

He glanced toward her wrist brace. "And sleep a little before submission, if possible. Exhaustion makes people melodramatic about ordinary tradeoffs."

When she left his office June was in the hall by the vending machines, feeding a dollar into the slot for pretzels. She hit the selection button twice because the machine lagged in a way everyone knew and hated. The packet dropped with a thick plastic thunk.

"Well?" June asked.

Leela shifted her laptop higher against her hip. "He wants the moderate-noise slice in front."

June chewed a piece of nicotine gum before answering. "Of course he does."

"It's not insane. That band is the only place the degradation curve is directional."

"Directional is one of his words for 'please stop making me look at the part where the thing is on fire.'"

Leela looked at the pretzel packet in June's hand because June's face had gone too readable. "I still have to see if it holds."

"Does it?"

"Not cleanly."

June gave a short nod, the kind people gave after receiving lab test results they had already guessed. "Right."

The vending machine hummed. Somewhere below them the elevator shuddered its way up from the basement.

"I need node C tonight," June said. "Not in principle. Literally tonight. My baseline is moving around and I can't tell whether it's seed drift or whether that preprocessing cache from August got rebuilt wrong. I need to know before methods lunch tomorrow, and I've got the deck meeting for the October seminar at five. If you have ten minutes, I also need your eyes on the hash logs, because you're still the only person in this building who can read old Hades output without making it sound mystical."

Leela should have said yes to one of those requests. Even one would have preserved something.

"Let me get through the afternoon sweep," she said. "Then I'll look."

June's mouth twitched as if a joke had tried to form and died on the way out.

"Sure," she said. "After your sweep, after methods lunch, after my deck meeting, after capitalism. Text me a real time when you have one."

She took the pretzels and went down the stairs instead of waiting for the elevator.

Leela spent the rest of the afternoon turning plots into smaller plots, then into captions that made the plots sound more settled than they were. She moved to the shared graduate office on the sixth floor because the basement had become too hot to think in. The office had one long window facing the lake. In daylight it could pass for relief. By evening it turned into a mirror and gave everyone back their own bad skin.

She ran the moderate-noise slice on three fresh shuffles, then five. One run came back close to the first result, not identical but near enough to tempt her. The next two sagged. The fifth returned a number that made the whole story look as if it had been assembled by a defendant's cousin. She ate crackers from the department seminar leftovers and licked the salt off her thumb because there was nothing else in the office and she did not want to lose the queue position walking to the cafe.

At 6:12 p.m. June's name lit the phone with `status on node c`. Seven minutes later another banner shoved over it: `also if you have the old hash-check script send it. mine is pulling different cache keys for no reason`. At 7:03 the third message arrived before Leela had answered either of the first two: `not joking, lee. if the august cache got overwritten i need to know now`.

Leela opened the thread and watched the gray bubbles stack over the blank half reserved for her. Then she set the phone face down on a stack of printouts. A few seconds later it buzzed again hard enough to make the paper clip tray chatter against the desk.

She pulled up the old hash-check script anyway. It sat in her utilities directory with a filename she had given it at two in the morning two years earlier, `please_god_work.py`. She could have sent it in five seconds. Instead she started a sixth run.

At 8:41 p.m. Mohit dropped two comments into the draft in quick succession: `Lead with strongest result. The point is evaluative framing, not total collapse.` and `Let's not overplay instability. Workshop audience will read that as lack of contribution.` He was home by then, or at least somewhere with lamplight warm enough to make the track-change colors look expensive. The comments had that composed end-of-day tone people used when someone else was still in the office doing the part that turned output into copy.

Leela typed back before she could stop herself.

`The strongest result is not replicating across fresh shuffles.`

The reply came four minutes later: `Then report the observed result on the scoped slice and name broader replication as future work. This is normal.` Normal had become another one of his laundering words. She stared at it until the blue message bubble blurred.

At 9:17 June called. The phone vibrated itself half an inch across the desk. Leela watched it move and did not pick up. When the ringing stopped, voicemail transcription threw up a mangled preview that was clear enough anyway: `Lee, pick up if you're there. I just need the stupid script. Call me back.` She swiped the banner away without listening to the audio.

She went down to the basement because the office had become too quiet. In the lab, the server closet heat wrapped around her like damp fabric. The fluorescents had entered their late-night phase, a faint intermittent buzz that made even clean objects look greasy. Somebody had thrown out the noodle tray but left the sauce streak on the table. Leela sat cross-legged in her chair, shoes off, one foot tucked under the opposite thigh until it went numb. She reran the sweep with the same parameters and a new seed. Negative again.

She opened the table in the paper and moved the strongest single run into the main column.

The run existed: timestamp, seed, output folder, a number the cluster had actually produced. The PDF could not contain every failed shuffle, every queue hour, every unanswered message from June glowing on her phone, and still remain the kind of document Mohit meant when he said submission. People scoped papers all the time. People decided which failures belonged in the room. If she wrote the full story there would be no paper, only a small respectable obituary for three days of compute and one more item on the list of reasons Mohit could present her as the senior student who did not finish things.

She changed the sentence one clause at a time. `In one initial evaluation, the model exhibited resilience under moderate corruption.` Then she cut `In one initial evaluation,` and watched the claim stand up straighter on the page. The shorter version bought her what the longer one did not: something Mohit could defend, something a committee might count as motion. She kept typing.

At 11:06 June appeared in the doorway.

She had changed into an old gray sweatshirt, the one with a food-service logo half peeled off the chest from too many washes. A nicotine gum wrapper was stuck to the cuff. Her laptop charger hung out of one pocket like an IV line.

"I called," she said.

"I saw."

"And?"

Leela turned back to the screen, hating herself for making that choice in such a visible way. "I'm in the middle of something."

"Obviously."

June came in and set her own laptop on the neighboring desk. The screen showed a spreadsheet of benchmark runs, green and yellow cells, comments in the margins, one column circled in red trackpad ink.

"Look," she said. She was not joking now. "This row was stable last week. Seventy-one point four, seventy-one point two, seventy-one point five. Now it is sixty-eight point nine, seventy-two point one, sixty-nine point two. Same branch. Same seed setting, as far as I can tell. If the cache is corrupt or the scheduler is reusing stale artifacts, I need to know before methods lunch tomorrow or I walk in there and get skinned alive in public."

Leela leaned over because reflex was older than strategy. The familiar code, the familiar naming conventions, June's comments in the margin written like she talked, `this one is bullshit`, `why is god like this`, `check manifest?` The problem might have been a cache mismatch. It might have been the August rebuild. It might have been nothing more dramatic than nondeterminism surfacing in a benchmark June had been too busy to babysit. Ten minutes with the logs would at least narrow it.

"I can look after this run finishes," Leela said.

June looked at the monitor on Leela's desk. "What run? The one that still doesn't hold, or the one after that?"

Leela straightened. "I don't have time for this."

"You mean you don't have time for me."

"I've got a deadline tomorrow."

"So do I, just with less branding."

The words should have escalated. Instead June's voice dropped lower.

"Did he tell you to take the pretty slice and call the rest future work?"

Leela did not answer fast enough.

"Jesus Christ," June said. Not loud. Almost tired. "He did."

"It's more complicated than that."

"No, it isn't. He found a cleaner noun for cherry-picking and now everybody gets to act civilized about it."

Leela felt the old instinct to explain, to produce enough clauses that the moral shape of the thing disappeared inside method. "The moderate band is real. The signal is there on the original split, and one rerun is close, and if I can stabilize the preprocessing"

"If you can wait long enough for the number you want."

Leela looked back at June's spreadsheet because June's face had turned too bare. "I said I'll help after this run."

June stood there another second. Then she shut her laptop.

"Don't do me the favor later," she said. "Either help now or don't."

She picked up the machine by one corner and left. The charger cable dragged behind her for a second like a tail, then snapped free of the chair leg.

Leela sat with both hands flat on the desk until the skin of her palms stuck to the laminate. The run finished. The result was still bad.

At 11:48 Mohit texted `Need draft by 8 so I can do a final pass before portal close.` Then he followed with `Do not flood the paper with caveats. Caveats are not integrity if they obscure the contribution.` Leela laughed once, a dry private sound that made nothing better. She forwarded herself the PDF figures, revised the discussion section, and cut the paragraph on the multilingual failures from six sentences to two. By 1:30 in the morning the paper had become recognizably professional. For a few seconds the trimmed paragraphs and clean table borders let her breathe. It looked like something a serious lab might submit.

She went home at 2:07, not because the work was done but because her right hand had started dropping characters while she typed. In the studio the cheap blinds leaked orange parking-lot light through the slats. She did not bother undressing all the way, only kicked off her jeans and lay down in a T-shirt and underwear on top of the sheet with her phone beside her head. The radiator knocked once and then did nothing useful. She slept for fifty-three minutes and dreamed in progress bars.

When she woke the lock screen held four unread texts from June, timestamps marching from 12:14 to 1:08 as if the night had been orderly: `forget node c. i found cpu time`, `still need the hash script`, `are you actually not answering me`, and finally, at 1:08 a.m., `never mind`.

Never mind was the angriest thing June had sent all week.

Leela showered because she could smell the server closet on her skin. The hot water ran out while she still had shampoo in her hair. She rinsed under a final burst of cold, swore once into the tile, and got dressed in yesterday's black jeans and a sweater that had gone shiny at the cuffs. On the walk back to Keating the early air was almost kind, lake wind and wet leaves and the false September suggestion that a person could restart anything.

The feeling lasted until she opened the draft.

Mohit had already left comments on the PDF she'd sent at 3:11 a.m.: `Title stronger if we foreground robustness rather than brittleness.`, `Table 2: remove variance column. It distracts from main comparison and is underpowered anyway.`, and `Abstract: "demonstrates" is fine here.`

There were no question marks anywhere. He edited like a man touching up a slide deck before a sponsor visit.

Leela put the paper side by side with the raw results. The variance column did distract. It distracted by making the result honest. She deleted it.

At 9:26 June sent a screenshot from the scheduler. Her jobs had finally started on slow shared nodes, estimated completion after 4 p.m. Beneath it she wrote `october seminar deck meeting at 5. if these numbers still drift i'm fucked`

Leela typed `I can look at the cache after submission` and then erased it because the sentence was already an insult.

At 10:02 Mohit called.

"How close are we?"

He sounded as if he were walking somewhere carpeted.

"Close enough to submit," Leela said. "Not close enough to believe."

"Belief is not the threshold."

"It should be."

"For a dissertation, perhaps. For a conference, the threshold is whether the contribution is intelligible and true within the stated scope."

"One run is not scope."

"Then stop saying one run. You did multiple evaluations. One of them supports the framed claim. The paper is about that frame."

Leela leaned against the office window. The glass held the previous night's grease from someone's forehead. Below, the lake looked metallic and uninterested.

"If someone asks for the broader failures in review"

"Then you answer the question in review. That is what review is for."

"And if June asks me why I held the cluster for a result I don't trust?"

There was a brief silence. When he spoke again his voice had gone quieter.

"June's frustrations with infrastructure aren't the governing issue here. Your submission is. Don't confuse side turbulence with your actual priorities."

Side turbulence. She pictured June in the basement at midnight with her sweatshirt cuff sticky from old gum wrappers, watching nondeterministic benchmark numbers wobble across a spreadsheet because the machines were busy generating another version of Leela's alibi.

"Send me the final PDF at noon," Mohit said. "Don't miss the window because you're feeling conflicted. Conflict is cheap. Deadlines are not."

He hung up before she could answer.

At noon she sent him the PDF. At 12:17 he returned it with two edits in the abstract and a single-line note: `Good. Submit this version.`

June did not text again until 2:04, when two messages landed almost on top of each other: `cache hashes don't match august` and, thirty seconds later, `was going to ask if you knew why but apparently i know why`.

Leela read both messages twice. The second one was unfair in the narrow technical sense. She had not caused the cache mismatch. Maybe a half-forgotten rebuild had caused it, or a storage sync glitch, or June's own deadline-cut corner from August. But unfairness was not the point. June had asked for time, for script help, for two hours on a node, for the courtesy of an answer. Leela had spent all of that currency already.

At 3:30 the conference portal opened for final upload. The system had the neutral bureaucratic look all portals shared, soft blue buttons, too much white space, a font that assumed the act underway was clean. She uploaded the anonymized PDF, then the supplemental appendix, then deleted the appendix and replaced it with a shorter one that omitted the worst collapse plots. The portal asked whether the paper included limitations. Yes. It asked whether computational resources might have constrained the breadth of evaluation. Yes. It asked whether all authors had reviewed the final submission. Yes, because Mohit had done more than review it.

At 4:11 June called again. Leela watched the screen light up with her name and a photo from last winter, both of them in June's kitchen with paper crowns from Christmas crackers somebody's cousin had mailed. June was making a face because the crown had torn in the middle. Leela let the phone ring out.

This time June did not leave even the formality of a voicemail.

Leela reopened Table 2. She could still restore the variance column. She could still change `demonstrates robust performance under moderate corruption` back to `shows promising performance in an initial moderate-corruption evaluation.` She could still make the paper small and embarrassing and probably accurate enough that Mohit would stop calling it a paper at all.

Instead she changed one more sentence in the discussion from `the model may retain utility under constrained perturbation settings` to `the model retains utility under constrained perturbation settings.`

The revision took less than two seconds. The firmer verb settled the paragraph into the shape Mohit wanted, blunt enough for a skim, stable enough to pass as confidence. One more line he could point to when he talked about trajectory.

At 4:43 Mohit sent one final text: `Submitted?` Leela typed `Uploading now.` He replied immediately: `Good. Keep the jobs live through tonight in case we need an extra sensitivity figure for rebuttal prep.`

She looked over to the scheduler window still open on the second monitor. Her reservations ran until midnight. June's latest job had crashed on node D with an out-of-memory error and requeued itself behind hers.

Leela could have canceled her block. Submission was enough for the deadline. The paper existed now. Whatever else she did to it after 5 p.m. would be greed or fear or habit, some mix so ordinary it barely needed a name. She rested her cursor over `scancel` and thought of June saying Either help now or don't.

Then June's name surfaced once more on the lock screen: `are you going to answer me at all`

The question sat on the screen while the portal generated its progress wheel. A thin blue circle filling itself with borrowed confidence.

Leela clicked `Submit`.

The confirmation page loaded with indecent speed. `Thank you for your submission.` A paper ID. A receipt. No siren, no lock on the door, no warning that the thing she had just done would remain true after she closed the browser.

She did not answer June.

On the scheduler, the jobs kept running. Her name held the machines in a clean rectangular block all the way to midnight. Below it, June's requeued job waited in yellow.

Leela turned the phone face down and left it vibrating against the desk until it stopped, as if delay were still a smaller thing than choice.
