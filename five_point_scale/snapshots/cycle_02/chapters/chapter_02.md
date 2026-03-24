# Chapter 2

The first tutorial was called "Python for Absolute Beginners" and it was taught by a kid who looked fifteen. He had a Minecraft poster behind him and a mechanical keyboard that sounded like a popcorn machine, and he said "super easy" eleven times in the first four minutes. Nick counted. He was sitting on his bed with his laptop balanced on a stack of library books because his desk was covered in half-squeezed tubes of cadmium yellow and a palette he hadn't scraped in two weeks, and the kid was saying that a variable was where the program kept something for later.

Nick understood putting things somewhere and finding them again. He did not understand why `x = 5` meant x equaled five, but `x == 5` was a question about whether x equaled five, and `x = x + 1` was apparently not a mathematical impossibility but just a normal thing that happened in programming all the time.

He rewound the video and watched it again. The kid said "super easy" and Nick paused and went to the kitchen and ate a handful of dry Cheerios from the box because he'd run out of milk two days ago and hadn't gone to the store because the store required spending money, which was a resource he was managing with the same precision he used to manage cadmium red — sparingly, with the awareness that once it was gone, it was gone. He still had the $1,340 that had been in checking at four in the morning, plus the $950 balance-transfer check he'd finally caved and deposited after dawn, one of the glossy credit-card traps that arrived in the mail promising relief up front and catastrophe in smaller print. The app said $2,290. For a second it looked like a usable number. Then it turned back into borrowed money and six days until Eastshore wanted $1,100.

He went back to the video.

The kid explained `if` statements. If a condition was true, the code inside the block would run. If it wasn't, it wouldn't. Nick wrote this down in a notebook — an actual notebook, a Strathmore sketchpad he'd been using for thumbnail compositions, the good paper wasted on his handwriting. `If True → do thing. If False → don't do thing.` He understood this conceptually. Humans operated on if-statements. If the light was good, he'd paint. If the client paid, he'd eat something other than cereal. If Midjourney hadn't eaten his career, he wouldn't be watching a child explain logic gates.

The problem was typing it. His fingers knew where the brushes went — the index finger guiding a No. 6 round, the pinky bracing on the mahlstick, the thumb controlling pressure on a palette knife. They did not know where the brackets went. He typed `if x = 5:` and the interpreter threw an error. He typed `if x == 5;` and it threw a different error. He typed `if x == 5:` and it worked and he felt a jolt of something that might have been accomplishment except it had taken him fourteen minutes to write a line that the fifteen-year-old had produced in two seconds while talking about his weekend.

By the end of the first week, Nick could print "Hello, World" to the console, define a function that added two numbers, and write a for-loop that counted to ten. He could not tell you why any of this was useful. The tutorials kept saying that programming was about solving problems, but the problems they presented — reversing a string, summing a list, finding the maximum value in an array — were problems that had already been solved, by the people who wrote the tutorials. He was not solving anything. He was copying.

This was, he realized, not entirely unfamiliar. Art school had started the same way. You copied the masters before you developed your own voice. You drew from casts of classical sculpture, reproduced Bridgman's anatomy plates, mixed colors to match Zorn's limited palette. The difference was that when he'd copied a Sargent brushstroke at twenty, his hand had understood what it was doing even when his brain hadn't caught up. There was a physical intelligence in the wrist, a feedback loop between the mark and the eye. The keyboard had no equivalent. He typed characters and stared at output and the connection between the two was entirely abstract, running through a machine he could not see and did not understand.

He found a Reddit thread called "How long does it take to learn Python?" The top answer said six months to a year for proficiency, two to three years for mastery. Nick had budgeted himself six weeks.

The second week was worse. He moved from YouTube to an online course called Codecademy that let him write code in a browser window and see the results immediately, and the immediacy was useful but also punishing, because every mistake was visible in real time. He misspelled `print` as `pirnt` and spent twenty minutes thinking the problem was logical rather than typographical. He forgot a colon at the end of a function definition and the error message said `SyntaxError: expected ':'` and he stared at it like it was written in Cyrillic. He tabbed out to Google "what does SyntaxError mean python" and the answer was that his syntax was wrong, which was like going to a doctor and being told the problem was that he was sick.

His apartment was cold. The building's heating was a shared boiler that the landlord ran on some schedule Nick had never been able to predict — warm at three in the afternoon, freezing at ten at night. He wore a flannel over a hoodie over a T-shirt and his fingers were stiff on the keys. The paint smell was fading from the room, or he was getting used to it, which felt like the same thing. The stacked canvases against the far wall — nine landscapes from the series that hadn't sold at the Temescal gallery, plus three unfinished commissions from the publisher who'd dropped him — caught the light from his laptop screen at odd angles and looked like a low wall around his living space, a barricade of failed productivity.

He didn't paint. Painting required a mental state he could not currently access, something between confidence and surrender, a willingness to make a mark without knowing where it led. Programming required the opposite: knowing exactly where it led before you made the mark. Every line had to be right before you wrote the next one. It was architecture, not painting. It was building from a blueprint, not building from a feeling.

He hated it. He kept going.

---

Mid-December he found LeetCode. Someone on a coding forum had said it was the standard preparation for technical interviews — a database of programming problems ranked Easy, Medium, and Hard, where you could write solutions and test them against hidden inputs. The interview-preparation industry around it was enormous: YouTube channels, courses, books, all dedicated to teaching people how to solve problems they would never encounter in actual jobs, in order to get hired for those actual jobs. It was, as far as Nick could tell, the most elaborate gatekeeping mechanism since the French salon system, and it ran on the same logic: prove you can do this arbitrary thing nobody cares about, and we'll let you into the room where the real work happens.

He started with Easy problems. Two Sum: given an array of integers and a target, find two numbers that add up to the target. He stared at it for forty-five minutes and wrote a solution that used two nested loops and was, according to the discussion forum, the worst possible approach in terms of efficiency but technically correct. He submitted it. It passed. He felt nothing.

The next problem was Reverse Integer. Given a 32-bit signed integer, reverse its digits. He spent two hours on it, most of that time trying to understand what "32-bit signed integer" meant and why it mattered. His solution failed on negative numbers. He fixed it. Then it failed on numbers that would overflow when reversed. He didn't know what overflow meant. He Googled it. He fixed it. Then it failed on zero. He submitted a version that passed all the test cases and looked at the discussion forum, where someone had solved the same problem in three lines that he couldn't parse.

The array-reversal problem broke him the first time. And the second time. And the third. It wasn't hard — he knew what reversing an array meant, he could see it in his head, the sequence of values flipping like a row of paint swatches held up to a mirror. But translating that visual understanding into a sequence of operations that a machine could execute required a kind of thinking his brain resisted the way oil paint resisted water. The logic was sequential where his thinking was spatial. He wanted to see the whole array at once, grasp its shape, and rearrange it. The computer wanted him to describe, step by step, how to swap individual elements, keeping track of indices and bounds and temporary variables, and the bookkeeping of it felt like being asked to describe a sunset by listing the wavelengths of each photon.

He failed it seventeen times. Seventeen attempts across eight days, each one revealing a different edge case or logical error he hadn't anticipated. On the eighteenth attempt, he passed, and his solution was so ugly — forty lines of code for a problem that could be solved in three with a built-in method he hadn't known existed — that he closed the laptop and walked around the block in the rain.

It was raining in Oakland nearly every day now, the December drizzle that turned the streets into mirror-gray and made the light flat and directionless, the kind of light he used to love for painting because it eliminated harsh shadows and let you see the true local color of everything. He walked past the taqueria on International that was always open, past the laundromat where he hadn't gone in three weeks because quarters cost money, past the Walgreens where he'd bought the ramen he was going to eat for dinner. His hands were in his pockets and they ached from typing in a way they'd never ached from painting — a tightness in the fingers, a soreness in the wrists, the specific discomfort of holding the same position for hours without the variation that brushwork demanded.

He went home and opened LeetCode and started the next problem.

By Christmas he had developed a method that was not comprehension but was something adjacent to it. He memorized solution patterns the way he'd once memorized color swatches — not understanding the chemistry of why cadmium and ultramarine produced a particular gray-green when mixed, but knowing that they did, and knowing when to reach for it. If the problem involved searching a sorted array, you used binary search. If it involved counting occurrences, you used a hash map. If it involved comparing strings, you usually needed two pointers. He didn't understand why these patterns worked. He understood that they worked, and he could recognize which situations called for which pattern, and that recognition — the visual artist's deepest skill, the ability to see similarity across difference — was the thing that saved him.

He could not, however, generate novel solutions. If a problem didn't match a pattern he'd memorized, he was dead. And the gap between matching a pattern and understanding why it worked meant that any variation — a different constraint, a larger input, an edge case the pattern didn't cover — could blow up his solution in ways he couldn't debug. He was functioning at roughly a twenty-percent success rate on Easy problems by mid-December, which was not enough for anything.

Christmas Eve. His neighbor two doors down was hosting a party. The bass came through the wall in a steady pulse that Nick could feel in his sternum, not quite loud enough to distinguish the song, just a heartbeat of someone else's good time. He was sitting cross-legged on the floor because his back hurt from hunching over the laptop on the bed and the chair at his desk was buried under canvas stretchers. The desk itself was still covered in paint tubes. He hadn't touched them. The cadmium yellow was cracking where the cap had been left loose, the pigment drying into a crust that he'd need to cut away if he ever opened it again. If.

He ate ramen — the good ramen, the Shin Ramyun packets from the Korean grocery on 14th that cost a dollar twenty each, which was his Christmas dinner splurge. He put an egg in it because he'd seen a TikTok that said you could crack an egg into the boiling noodles and it would poach, and it didn't poach so much as disintegrate into stringy white filaments that floated in the broth like something medical, but it was protein and it was hot and he ate it standing at the kitchen counter because the table was his laptop now.

The party thumped. Someone laughed loud enough to hear through the plaster. Nick opened LeetCode and pulled up the Two Sum problem again — not because he hadn't solved it, but because he'd solved it badly and he wanted to understand the hash-map solution that everyone in the discussion forum treated as obvious. He worked through it line by line, forcing himself to name the job of each step before moving to the next one: store the number, note where it was, check whether the missing number had already shown up. Halfway through, the logic stopped feeling like a magic trick and started feeling like procedure. It was still slow. It still wouldn't survive a timed interview. But when he ran it, it worked for reasons he could almost say out loud.

He solved it. Then he got through Valid Parentheses and Merge Two Sorted Lists the same ugly way: not by seeing the answer whole, but by refusing to skip steps. Every time he jumped ahead, he broke something. Every time he stayed inside the sequence, the code eventually stopped breaking. The process was so slow that it would be completely useless in a timed interview, but it was working, and he was learning, and the party next door was getting louder, and it was eleven forty-five on Christmas Eve and he was alone on the floor of an apartment that smelled less like turpentine than it had a month ago, solving problems that a teenager could solve in his sleep, and he thought: this is insane. This is the stupidest thing I've ever done. He didn't stop.

New Year's came and went without his noticing. He'd fallen asleep on the floor at eleven-thirty on the thirty-first, laptop still warm on his thigh, and woke at two in the morning to distant fireworks and the taste of stale ramen. He'd been dreaming in loops: moving the same values around, losing his place, starting over, never reaching the green check.

January was colder and darker and he stopped leaving the apartment for anything other than groceries. He showered less. His laundry piled up in the closet. He wore the same flannel for four days running because it didn't smell yet and nobody was around to notice. By then he had run $2,990 through his checking account: the original $1,340, the first $950 balance-transfer check, then a second one for $700 when the first trap stopped feeling like a trap and started feeling like groceries. December had taken $800 through the rent portal. January had taken another $600. PG&E got enough to keep the lights on. The rest went in twenty-dollar leaks: eggs, rice, black beans, ramen, toilet paper, dish soap, one roll of quarters for the laundromat that he stretched until he was wearing underwear with the elastic going loose. By the last week of January his checking account sat at $206, which meant he was eating rice and eggs and the occasional can of black beans, which was fine, which was survivable, which was the kind of arithmetic he'd been doing since the publisher dropped him and which had become so automatic he could calculate the cost of a grocery run to the penny while walking the aisles. A dozen eggs, $3.49. Rice, the twenty-pound bag from the Asian grocery, $18.99, which would last three weeks. Shin Ramyun five-packs, $5.49, a luxury he rationed. He'd stopped buying coffee and was drinking the instant Folgers that someone had left in his cabinet months ago, the crystals clumped and slightly off, but caffeine was caffeine when you were up at midnight fighting with a linked-list problem that wanted you to reverse a sequence of nodes and you couldn't figure out why your pointers kept pointing at nothing.

By late January, his success rate on Easy problems had climbed to roughly forty percent, with the crucial caveat that he could only solve problems he recognized as variations of patterns he'd already memorized. Anything genuinely novel still destroyed him.

On January 27th he gave Longest Substring Without Repeating Characters three hours and got nothing out of it but a deeper appreciation for the ways a person could be too stupid for a window. The tutorials called it a sliding-window problem, as if that explained anything. He understood the rule in plain English. Keep the run of letters that still worked. Drop the ones that broke it. But the computer did not care what he understood in plain English. It wanted indices. It wanted a left pointer and a right pointer and a set that grew and shrank at the proper times. He wrote one version that worked for `abcabcbb` and broke on `bbbbb`. He wrote another that passed both and failed on `pwwkew`. He wrote a third that looped forever on one of the hidden tests until the site timed out and told him, in a neat gray font, that his submission had exceeded the time limit.

He closed the tab and saw the others behind it: the Canopy posting he'd been keeping open for two weeks, his checking account, and an email from Eastshore that began REMINDER in all caps. The bank app still said $206. He had eight eggs left, half a bag of rice, and enough instant coffee for maybe four mornings. He could not code his way out of that by becoming incrementally less bad at LeetCode over the next month.

He opened the Canopy listing again. Basic Python or JavaScript. Comfort with repetitive technical tasks. Background in visual arts preferred. Preferred. Not required. He read that line three times, then opened the resume draft he'd been torturing for three days.

The first line said `Freelance Painter and Illustrator.` He changed it to `Visual Content Creator and Evaluator` and immediately wanted to put his fist through the screen. Under skills he already had Python typed, which was a lie only in magnitude. He added JavaScript because he'd spent two nights copying beginner exercises into a browser console and because every job-forum ghoul on the internet said keywords mattered more than shame. He stole `visual quality assessment` straight from the Canopy posting. In the field for relevant experience he turned gallery work into `visual content creation and evaluation` and freelance illustration into `client-facing creative project management.` It was all technically true in the way that a Mercator projection was technically a map — it represented the territory, just with significant distortion in the areas that mattered.

He stopped with the cursor over Submit. On the desk beside the keyboard, a tube of cadmium yellow had skinned over at the mouth. The half-finished Montclair hills leaned against the wall with the foreground still blank. Up to this point the plan had been something he could rehearse in private, an insomnia project, a stupid vindictive shape in his head. If Canopy wrote back, it would stop being private. He would have to keep lying forward. He would have to hand this résumé version of himself — visual content creator, client-facing, technically useful — to the company he wanted to get inside and foul from the middle.

He clicked Submit.

The confirmation page said his application was under review and that Canopy typically responded within two weeks. He stared at the screen for a while. Then he closed the laptop and looked at his apartment — the stacked canvases, the paint supplies he'd shoved to one end of the desk to make room for a keyboard, the Cheerios box on the counter, the latest overdue rent notice he'd pinned under a magnet so he wouldn't lose it, which meant he saw it every time he went to the kitchen. Outside, it was raining again, the flat gray Oakland rain that made everything look like a painting he would never make.

His phone rang. It was Jess.

---

"It's so dry here," Jess said. "Like, my hands are cracking. I brought three tubes of lotion and I've gone through all of them."

"Where are you again?"

"Taos. Well, outside Taos. The residency's in this old adobe compound about twenty minutes from town. There's like six of us. Mostly painters, one sculptor who makes these incredible carved things out of cottonwood root."

"Nice," Nick said. He was sitting on the floor again, back against the bed frame, phone on speaker beside him. The laptop was open on the floor too, LeetCode still loaded, but he'd turned the brightness down.

"The light here is — God, Nick, the light. It's like painting in a different atmosphere. Everything has this golden — I don't know, I keep wanting to say warmth, but it's more than warmth, it's like the air itself has a color temperature. I've been doing these sunset studies and the chromas are so high they'd look fake if you put them in a painting back home."

"Sounds good," Nick said.

"I mean, it's also freezing at night and the plumbing is from like 1940 and I've been eating a lot of beans. But the work's going well. I finished six pieces since November. Small ones, but."

"That's great."

"What about you? You painting?"

Nick looked at the canvases stacked against the wall. The top one was a half-finished landscape of the Montclair hills he'd started in October, before the phone call from the publisher. The sky was blocked in with a wash of cerulean cut with raw umber, which was a color he liked for Oakland's overcast, and the hills were roughed in with a green so neutral it was almost gray. He'd been planning to spend a month on the foreground, layering the grasses and the light-struck eucalyptus that lined the ridge. He hadn't looked at it in six weeks, really looked at it, the way you had to look at a painting in progress to figure out where it was going.

"Not as much," he said.

"You OK?"

"Yeah, I'm fine. Just, you know. Broke."

"Yeah." Jess was quiet for a second. "Me too. The residency covers housing and studio but I'm still paying rent on my place in Portland. Mike's supposedly subletting but he's been weird about the deposit. I might have to go up there in February and deal with it."

"That sucks."

"It does suck. But the work's good, so." She paused. "You doing commission stuff? Did you hear back from that children's book thing?"

"That fell through."

"The Midjourney thing?"

"Yeah."

"Fuck. Nick, I'm sorry. They were one of the good ones."

"They were the only one."

Jess was quiet again, longer this time. Nick could hear wind on her end, which meant she was outside, probably standing on the porch of the adobe compound, watching the last light on the mountains because that was what Jess did — she went where the light was, and she stood in it.

"Are you gonna be OK?" she said. "Like, money-wise?"

"I'm figuring it out."

"Because if you need — I mean, I don't have much, but I could—"

"I'm fine, Jess. I'm applying for some stuff."

"Art stuff?"

"Yeah," he said. "Sort of."

"OK." She didn't push. This was one of the things Nick liked about Jess — she trusted you to tell her the truth and didn't dig when you gave her something that smelled like a lie. It was also, right now, the thing that made talking to her impossible. She was in New Mexico making paintings and eating beans and her hands were cracking from the dry air and she was doing the thing they'd both said they'd do when they were twenty-two, which was make art no matter what, even when no matter what meant beans and bad plumbing and $800 a month scrounged from commissions and teaching gigs and the occasional grant. She was living the plan. He was abandoning it.

"I should go," Jess said. "There's a thing tonight, one of the other residents is cooking and we're all supposed to bring something and I was going to bring wine but there's no wine in this town under fifteen dollars so I'm bringing tortilla chips."

"Classy."

"Extremely." She laughed. "Hey. Come visit if you can. You'd love the light."

"Maybe," Nick said.

"I mean it. There's always room."

"I know. Thanks."

"Love you, weirdo."

"Love you too."

He hung up and sat there on the floor for a while with the phone warm in his hand. He could still hear Jess's voice in his head, the specific brightness she got when she talked about light, the same brightness she'd had at twenty-two when they were both in the foundation program and everything was going to work out. The laptop screen had gone to sleep, and in the dark glass he could see the reflection of his apartment — the stacked canvases, the desk he'd half-cleared for a keyboard, the window where the rain was doing what the rain did. His hands were in his lap and they looked wrong to him, the calluses from brush handles still there but softening, the paint stains fading from the cuticles, the small scar on his right index finger from the X-Acto knife he'd slipped with three years ago while cutting a mat for a frame. They were becoming someone else's hands.

He still hadn't told Jess about the plan. He wasn't going to, not now, not with the Canopy application already sitting in somebody's queue and the whole idea still too thin to survive being said aloud.

He opened the laptop. The screen woke to LeetCode and an unsolved problem called Valid Anagram, which asked whether two strings contained the same characters in different arrangements.

Nick looked at it. He knew the surface version immediately: same letters, different order, yes or no. He could see that part. He could always see that part.

He tried the blunt version first. He would sort the letters and compare them. He typed `if sorted(s) == sorted(t):` and ran the sample case. The sample case came back green. He deleted it anyway.

The version he was supposed to understand was the hash-map version. It counted frequencies. It moved step by step. He typed `counts = {}`. Then he typed `for char in s:` and `counts[char] += 1`.

He ran it. `KeyError: 'a'`

Nick stared at the screen. Of course there had to be a way to tell the dictionary a letter existed before asking it to add one. Of course he didn't know it yet.

He flexed his right hand, put his fingers back on the keys, and started the problem over from the top.
