# Chapter 3

The basement smelled like hot dust and old coffee, that sealed Keating air that made every season feel faintly mechanical. Leela had been pretending to read a benchmark paper in the outer lab, one eye on the PDF and one eye on the hallway, because it still felt possible that if she was visibly present enough Mohit might remember he owed her a real answer about her year. When he appeared in his doorway and said, "Do you have a minute?" the question landed in the tone that implied a favor she should be grateful to provide.

His office door clicked shut behind her. He did not usually close it for small things.

"What's up?" she said.

Mohit stayed standing for another beat, looking at the screen on his desk as if the difficulty lived there and not in him. He had the same immaculate shirtsleeves he always had, pale blue today, cuffs clean, expensive glasses catching the fluorescence. In public that softness read as youth or calm. In a closed room it read more like the discipline of somebody who had learned never to give away the wrong thing for free.

"We may have had some repository irregularity over the weekend," he said. "Probably noise. Possibly not. I don't want to make it larger than it is before we have a clean read."

Leela waited. He liked these little ramps, the part where everybody else was supposed to prove they understood the seriousness without forcing him to say it too plainly.

"What kind of irregularity?"

"Bulk clone behavior. A few pulls that don't map neatly to the usual workflow. It could be a backup job misfiring. It could be someone getting overcurious about another student's code. It could be nothing except bad hygiene, which frankly would be on brand for this building." He gave her a small private smile, inviting her into a wearily competent we. "I need somebody careful on it."

The ugly thing was how quickly that worked. Careful. Not brilliant, not fast, not visionary. Careful was the compliment he gave when he wanted unpaid labor and a low chance of public drama, and still some part of her leaned toward it like a plant toward a window.

"You want me to check Hades?" she said.

"Just the access trail for now. Quietly."

He pulled open a drawer, took out a yellow sticky note, and slid it across the desk blotter toward her. On it, in his neat squared-off handwriting, were the old admin username and a temporary password. Not even temporary, really. A variation on one she had used two years ago, before Mohit said the cluster needed cleaner governance and took most of the permissions back into a folder of his own.

She looked down at the note and then back at him. "I thought that account was disabled."

"Disabled is a strong word." He sat now, finally, one wrist resting on the lip of the desk. "Dormant. It's still the least messy way in. If I send this through central IT, I create a ticket, and then we have a record before we even know if there's a problem. I'd rather not invite process into the room before we have to."

He said process the way other people said raccoons.

Leela turned the sticky note over once with her thumbnail. The paper had already softened a little from his hand. "Do you know which repos?"

"Some student directories. I didn't do a deep pass. I saw enough to know I didn't want Ben freelancing an interpretation." He gave a brief exhale through his nose. "June would turn it into a constitutional crisis, Omar is underwater, and you actually know the system's history."

There it was, the inventory of why she mattered and why everybody else was unusable. Even June got deployed here as a warning. Leela heard herself ask, "Do they know something happened?"

"No, and let's keep it that way unless we have to widen the circle." His voice went warmer, more mentor than manager. "Leela, this is exactly the kind of thing that reminds me why I trusted you with infrastructure in the first place. You see the shape of a mess without needing to perform your feelings about it."

He always sounded most paternal when he was asking someone to help him lie about scale.

She should have asked why he had noticed the irregularity himself if he had not done a deep pass. She should have asked why he still had her old account alive. She should have asked why a faculty director who had spent the last two weeks making everybody compete for scraps suddenly wanted discretion more than compliance. Instead she said, "Okay. I'll take a look tonight."

Mohit nodded as if she had restored something orderly in the world. "Good. Send me a short readout when you have one. And keep this bounded. If it's student curiosity, I want it handled as mentoring, not scandal."

"Sure."

"And once this is off the table, let's sit down properly about your timeline. I know that uncertainty has been hanging over you."

The sentence landed exactly where he meant it to. Not a promise, not even a date, just a little ration of future. He knew how little it took now.

She put the sticky note in her notebook and stood. Mohit had already turned back to his screen, the conversation filed. On the wall behind him, a framed printout from some old award still thanked him for leadership in data-for-good research, the kind of phrase that sounded noble until you had watched the machinery that fed it.

At the door he said, without looking up, "I appreciate this."

Outside, the lab kept humming as if nothing had happened. Ben was at the far whiteboard drawing boxes around boxes with a blue marker, his expensive jacket slung over the back of a chair like he expected nobody would ever steal from engineers. He was mouthing some sentence to himself as he erased and rewrote a heading. June was not there. Omar was not there. The room felt briefly simpler because the people who would have read something into Mohit's closed door were gone.

Leela went to the bathroom, took the sticky note back out, and read it again in the stall. The password was one extra symbol added to the old one, a lazy mutation. Mohit was always preaching attack surfaces and threat models to first-years and then doing things like this inside his own lab. The practical explanation was that he trusted obscurity more than hygiene when the hygiene inconvenienced him. The less practical explanation sat next to it and would not stop breathing.

She washed her hands longer than necessary, pressing her thumb into the sore ridge at the edge of her wrist brace. Then she went upstairs to the graduate office and stayed there until dusk answering email she did not care about, because if she logged into the cluster at four in the afternoon it would feel too much like obedience. At six thirty she bought peanut-butter crackers and a sweating bottle of Diet Coke from the machine near the loading dock, carried both back down to the basement, and waited until even Ben finally left, backpack bulging, cheerful enough to wave.

The lab after hours never became quiet. It only lost the frequencies made by people. Once the talking stopped you could hear what the building had been saying all along: the fluorescent ballast whine, the thin rattle in the vent by the server closet, the old refrigerator by the sink clicking into another doomed attempt at cold. The salvaged couches looked more embarrassing empty. Somebody had left half a seminar cookie on a napkin by the printer, one bite gone and the rest hardening into department archaeology.

Hades lived in a closet off the main room behind a louvered metal door that never fully latched. The cluster had been named by a previous generation of graduate men who found mythology hilarious when applied to purchased hardware. Nobody had renamed it after the joke stopped being funny. The closet was too warm all year and carried a linty current of air that smelled faintly toasted, like circuitry and old carpet. When Leela pulled over the rolling chair, the fake leather seat gave a small ripping sound under her thigh where it had split last spring.

She logged in from the battered workstation outside the closet because remote access from her apartment liked to fail exactly when she needed it, and because if something went wrong she wanted to be physically next to the noise. Her old username still worked. The password worked on the first try. She hated that most of all, the confirmation that this piece of buried infrastructure had been sitting there all this time, waiting to be useful to him again.

For a minute she just looked at the prompt.

Then she started with the unglamorous things. Authentication logs. Git service logs. Cron jobs. Access histories on the shared storage mount. The work was not detective cinema. It was waiting for text to unspool, narrowing time windows, copying one ugly line into a scratch buffer and then another, realizing she had the wrong date format, backing out, trying again. She kept a legal pad on her knee because if she trusted herself to remember the timestamps she'd be there until dawn inventing patterns that were not there. Her own handwriting slanted worse the more tired she got.

At 8:14 she found the weekend spike Mohit had been talking about. It was real enough: a burst of authenticated access late Saturday night, then several large clone operations in close succession. The traffic moved with purpose, one mirror firing after the next. Several repositories under the lab group had been duplicated almost back to back, the kind of sequence no normal student workflow produced because nobody sane copied six private repos on a Saturday unless they were leaving the lab or stripping it for parts.

Leela sat back and ate two crackers without tasting them.

The first clean possibility was a bad backup. She wanted that badly enough to spend forty minutes proving it false. The scheduled backup jobs ran to a different path on a different timetable. These pulls had touched live student repositories directly, including private branches. Worse, the destination did not look like any of the old archive locations she had helped set up. The path name surfaced in fragments at first, just enough to be annoying: `/srv/ruderal/ingest/`, then later `ruderal_sync`, then a permissions entry on a staging directory called `ruderal_private`.

Ruderal.

She wrote it on the legal pad and stared at the word. It sounded botanical, or maybe pharmaceutical, one of those names that tried to imply resilience by borrowing from weeds. No folder she had ever seen on Hades carried a name like that; it was too slick for a university storage convention and too self-conscious for a benchmark suite. She went back through the logs and found it again, this time in a service-account creation command from August, buried between more ordinary admin noise. The creating user was `msaran`.

Her body did not give her a dramatic reaction. No cinematic drop in the stomach, no clear bell of revelation. She only became aware that the brace on her wrist had soaked through underneath, the skin there damp and itchy, and that the server fan was blowing hot air directly at her shins through the closet slats like a small mean animal.

She checked the line again.

User added service account `ruderal_sync`.

User `msaran`.

August date, before the semester started.

She copied the line into a local file. Then she checked whether `msaran` could be somebody else, some inherited service name from the bad old days. Every trail led back to Mohit. Hades was a mess, but it usually attached actions to actual people. Mohit had his own faculty account, same as everyone. He had created something on the cluster in August and named it after a word that kept reappearing around mirrored student repositories.

Leela rubbed the heel of her hand against one eye until lights burst under the lid. When she looked again, the text had not changed.

She kept digging because the alternative was getting up and deciding what this meant, and she was not ready for the deciding part. She pulled the detailed access history on the Saturday session. The source IP belonged to Haviland's VPN range, which was irritatingly broad until she cross-referenced a second log and saw the device label attached to the key exchange. `msaran-mbp`. Not subtle. Not even especially competent. Just protected by the ordinary fact that almost nobody below faculty rank spent their nights reading auth logs unless somebody asked them to.

The repository list made it intimate: June's benchmark codebase, Omar's theory experiments, her own dissertation repo, including the embarrassing side branch where she kept half-finished methods notes because she could not bear to look at them in the main tree, and a smaller private repository that held lab meeting notes and old figure drafts. This went past paper outputs. He had lifted the rooms inside the house.

She opened the destination tree only far enough to confirm structure. The mirrors lived inside an active working directory. The folders had fresh timestamps after the initial clone. Somebody had been pulling updates. There were subdirectories labeled for demo assets and comparative plots. One folder held exported images with filenames that preserved student initials. Another held a markdown inventory of datasets and claims, half finished, as if whoever wrote it expected to come back later and turn the mess into something presentable.

Ruderal was a workspace.

Leela put both feet flat on the floor. The chair wobbled because one wheel had started sticking again, and she had to brace herself against the metal rack to stop the little skid. Her fingers smelled like salt from the crackers and dust from the keyboard. Somewhere down the hall a bathroom hand dryer started up, ran for too long, and quit. Somebody else was still in the building after all, though the floor felt deserted enough that the sound only sharpened the solitude instead of softening it.

She read the markdown inventory once, then again. It carried the chill of a planning document, stripped of even the little false nobility Mohit liked to apply in meetings. Repo names. Candidate figures. Notes on generalization claims. A line about "student-facing provenance clean-up" that made her sit perfectly still for three seconds because there was no benign reading of it and her mind still tried to produce one.

Maybe he was preparing a sponsor deck and planned to loop them in later.

Maybe Haviland's intellectual-property policy was broad enough that this was disgusting but not technically theft.

Maybe Ruderal was some stupid temporary internal codename for the lab's industry push and he had simply not told them because everything this semester now arrived as theater.

Maybe, maybe, maybe. The mind was a pathetic machine when it wanted a softer fact.

She pulled the access logs on her own repo and saw the mirrored private branch names appear one after another, including `chapter2_failures` and `defense_timeline_notes`, and the maybe machine finally lost a little power. There was no professional reason Mohit needed the folder where she had written, in two separate ugly files, what happened if the final year did not materialize. There was no startup hygiene explanation for June's rebuttal notes or Omar's draft theorem appendix sitting under a directory none of them knew existed.

She imagined June seeing this. June would go flat first, voice gone efficient, and then mean. Not theatrical, Mohit's favorite accusation. Specific. She would say, I knew it, and then she would say, How long have you known? The second question mattered more. It always had.

Leela checked the time. 10:52.

The cleanest thing would be to text June now. Are you awake. Come downstairs. There is a thing you need to see. June lived fifteen minutes away; she would put on shoes, she would come, and by midnight at least two people in the lab would understand what Mohit had done. By tomorrow morning it might be everyone.

June was the deeper problem. She would understand, immediately and correctly, that Mohit had chosen Leela for this errand because Leela still came when called. He could close a door, hand her an old credential, promise to discuss her timeline later, and she would say okay in under a minute. The shame in that ran deeper than the ordinary shame of graduate school. Naive faith had already curdled into appetite. She still wanted to be the one he trusted to handle the ugly parts. She still wanted to matter to him in the special administrative way that often preceded getting fed.

She put the phone down without unlocking it.

The next clean thing would be to create a record outside him. Email the logs to herself at Gmail. Forward them to Gloria Fisk. File a dry little ticket with central IT: old dormant admin account active, unauthorized service account, mirrored student repositories under unknown directory. That version required less courage than a confrontation and more honesty than silence. It also required her to admit, in writing, that she had used inherited admin credentials off the books at Mohit's request. Once it entered a system it would not stay her story. It would become timestamps, accounts, scope of access. Mohit would say he had asked for a limited audit and she had exceeded her remit. He would say she had longstanding access habits he had been trying to regularize. He would say this was exactly why informal technical stewardship by students created governance problems. He would not need to invent much. The ingredients already existed.

She could also simply confront him in person tomorrow, shut his office door and lay the printout down between them and ask what Ruderal was. But even in fantasy the scene bent toward him. He would fold his hands, look saddened, and ask why she had dug beyond the breach question. He would tell her lab materials had to be prepared for partnership conversations in aggregate. He would say she was collapsing administrative roughness into moral accusation because she was stressed about her own timeline. Then he would ask who else had seen the logs, and if the answer was nobody, she would be alone in the room with a man who had just proved how quietly he could move student work out the back door.

Then the practical part of her went to work.

If she told nobody tonight, the fact would remain a fact tomorrow.

If she told nobody tonight, she could think.

If she told nobody tonight, she would not yet have detonated the last flimsy version of her year in a burst of righteous clarity that nobody at Haviland would reward.

She kept arranging the reasons as if order changed what they cost. Saying the sentence aloud would make the whole structure real: Mohit was stealing from them, and he had felt safe enough asking her to find the proof.

She copied the relevant logs into an encrypted archive on her laptop. The progress bar moved with insulting leisure. While it ran she pared back the local shell history on the workstation, not enough to beat a real audit, only enough that anyone glancing tomorrow would have to work to see the shape of the night.

When the archive finished, she named it `notes_fall_misc.zip` and dropped it among old dissertation folders.

She opened a new email to Mohit and stared at the blank body until the cursor settled into its patient blink. Then she typed:

No sign of an external breach. There was some internal bulk mirroring over the weekend into a staging directory I don't recognize, and the access appears to have come through valid credentials from inside Haviland's VPN. I can clean up the stale account issue tomorrow if you want. My read is that this stays in the lane of internal permissions drift.

She read it twice. The lie lived in the compression, in the way the email turned theft into housekeeping. Internal bulk mirroring. Valid credentials. Internal permissions drift. By morning he could forward it to whoever he liked and let those phrases do the narrowing for him.

Her thumb hovered over the trackpad.

She pictured June seeing the thread later, her voice going flat on the words internal permissions drift. Omar would go to the timestamp first, then the stale admin account, then everything Leela had chosen not to say.

The cursor kept blinking. In the server-closet heat, the workstation fan and her own pulse found the same thin pitch.

Leela sent the email.

The whoosh sound was tiny, almost comic. Years of training and debt and deferred adulthood, and the decisive noise was the same one that announced seminar reminders and potluck sign-ups.

Afterward she sat still long enough for the workstation screen to dim. In the blackened reflection she could see the pale stripe of fluorescence across her face, her braid loosened at the neck, the legal pad on her knee with RUDERAL written too hard into the paper. She tore off that page, folded it into quarters, and tucked it into the back pocket of her notebook instead of throwing it away.

When she finally stood, her legs tingled from the bad angle and the chair gave another small skin-peeling rip under her. She shut the server closet door though it would never stay fully shut. At the sink she rinsed the cracker salt from her fingers and watched the water go cloudy from dust. The half cookie by the printer was still there. Ben's blue marker cap was still off on the whiteboard ledge. Ordinary stupid lab life had survived the evening intact, which felt like an accusation too.

Mohit's reply came before she left the building.

Thanks. I suspected as much. Let's discuss tomorrow.

That was all. No surprise, no request for the directory name, no curiosity about scope. Only confirmation that whatever needed managing had been managed for the night.

Leela put the phone face down in her bag. She switched off the desk lamp by the sink, checked once that the encrypted file sat where she had hidden it among old dissertation folders, and walked out into the hallway with the notebook held flat against her ribs as if she were carrying something breakable. The basement door shut behind her with the soft padded seal of a well-funded building. Upstairs, somewhere above the concrete and ducts and humming pipes, the rest of the university kept moving toward morning without knowing what had already been taken.
