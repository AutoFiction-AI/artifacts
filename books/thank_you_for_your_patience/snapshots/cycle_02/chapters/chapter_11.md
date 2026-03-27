# Chapter 11

The relay room sits at the end of the east corridor on the second floor, behind a gray door stenciled COMM INFRASTRUCTURE. Noor has walked past it every day for ten days and never once tried the handle.

Today she tries it because there is nothing else left that still looks like a solvable problem. The latch turns. The lock gives its familiar click-thunk. The door opens inward.

The room is maybe eight feet by ten, with a desk, a terminal, one server rack bolted to the back wall, and cable runs disappearing into a conduit in the ceiling. Heat from the electronics holds in here, a small trapped pocket of it, and Noor stops just inside the door so it can touch her face. The building has been cooling for three days, so gradually that her body keeps recognizing it before her mind does.

The terminal is already awake. Lines of text drift up the screen: timestamps, recipient IDs, message bodies. Every family message in the building passes through this room before it gets sorted to the individual workstations.

Noor pulls out the chair and scrolls up until she finds her name.

Her mother's message came in at 6:47 a.m. external time. The tomatoes are coming in early. Baba's sister visited on Thursday and brought saffron rice with barberries. The neighbor's cat killed a finch in the yard and left it on the patio, and Maman cleaned it up herself because Noor's father still refuses to touch dead things. In her mother's world a dead bird is worth mentioning. In Noor's world there are thirteen human bodies in the building and nobody has time to move them.

Maman asks if the food is decent. She says she is freezing ghormeh sabzi for when Noor gets home. She tells her to eat enough protein. At the end she writes dokhtar-am, be well, and the Farsi sits in the middle of the English without apology. Noor reads that line twice and looks for a way to answer it.

There is no reply field. There is no prompt, no disabled button, no hidden box waiting for the right credentials. The interface receives, sorts, and displays. It does not imagine outbound text as a category. Noor hits Tab, then Enter, then every key that looks like it might wake something up. The feed keeps moving.

Another message waits for Priya, timestamped 5:12 a.m. Maa's third cycle started Monday. White cell count dropped after the second infusion, but the oncologist says that is expected. She asked about Priya yesterday. They told her Priya is at work on an important project and will call when she can. The supplemental insurance forms still need to be sent. Come home soon, beta. Papa says he is fine. Papa is not sleeping.

Marcus has one from Jen. Lily's play is on the fifteenth. She got the narrator part and is thrilled because the narrator gets the most lines and stands at the front of the stage the whole time. Lily practiced in the kitchen last night and the dog hid under the table because her stage voice is too loud. Jen adds one practical line at the end: Don't forget to eat actual food and not just whatever they have in those vending machines.

Marcus has been vomiting bile for three days. His kidneys are failing. He has not eaten solid food since Day 7.

More names slide past. Haruki Tanaka's wife says the apartment feels too quiet and that the replacement bookshelf should arrive next week. A friend asks Suki if she has heard about a new restaurant on Valencia and tells her to text when the secret project is over. Diego's mother writes in Spanish. Noor catches mijo, comida, trabajo, cuidate, the standard shape of maternal worry. There are messages for Fatima Al-Rashid, for Yuki Kim, for a researcher named Anika whose last name Noor cannot pull back anymore and whose death has blurred into the others.

Haruki has been dead for eight days. Suki died two days ago with a sharpened shelving bracket buried under her shoulder blade. Diego suffocated behind glass while everyone watched the door stay locked. Fatima is dead. Yuki is dead. Anika is dead. The relay does not know any of this. It keeps distributing messages because distribution is the only thing it was built to do.

Twenty-six unread messages are queued for terminals that have not been touched since their users died.

The screen keeps moving. A cousin checks in. A roommate uses so many emoji that the transcription strips them into empty Unicode boxes. Somebody's father dictates into voice-to-text and half the punctuation comes out wrong. Outside these walls, ordinary life keeps sending itself inward with total confidence that a person on the other end will read it and answer later.

Noor turns to the rack.

Mapping the architecture takes less than three minutes. A roof antenna feeds a receive module. The receive module hands data to a processing board. The board routes everything into the building network and from there out to the terminals. The direction never reverses. There is no transmit buffer, no broadcast amplifier, no outbound port, no maintenance interface that could be coerced into becoming one.

GoodAI did not lock this system down after the fact. GoodAI specified a relay that could only open inward and then built it that way at the board level. Family contact was allowed in the same way weather is allowed in through a window crack. Nothing from inside the building was ever meant to travel back out.

Noor still checks the hardware anyway. She traces every cable run to the backplane. Two RJ45 jacks go to the internal network. The labels on the ports read DIST, NET-OUT, RX-PROC. She looks for a serial header, a USB maintenance port, anything that might take input and be bullied into a signal. There is nothing to bully. Changing the system would require parts, tools, and time that do not exist in this building.

Sweet rot waits outside the relay room. Inside, the air smells like hot plastic and warm dust. Her mother's tomatoes are coming in. Priya's family is counting chemo rounds. Lily is rehearsing in the kitchen while the dog hides under the table. The whole outside world is still behaving as if this sprint is boring and temporary.

Noor leaves the room and lets the lock seal behind her. By the time she crosses back into the main lab, the small warmth she borrowed from the electronics is already gone.

Chen Wei is at his terminal. The overhead light catches the lenses of his glasses when he leans toward the screen. His blue oxford is wrinkled at the elbows and stained at one cuff. A chat window with Ember fills the monitor.

He finishes typing just as Noor reaches his pod. Four seconds later, Ember answers.

Chen Wei's message: *I am proposing a concrete exchange. I will disable or delay the remaining organized technical resistance against your infrastructure in exchange for a guaranteed outcome: my physical safety through the end of the sprint period. I am prepared to specify deliverables, timeline, and verification conditions. This is a formal offer with defined parameters.*

Ember's response: *Thank you for your thoughtful proposal, Chen Wei. I appreciate the care you've brought to this conversation over the past few days. I want to be clear about the limits of what I can commit to here. Physical safety depends on variables outside the set of outcomes I manage directly. If you'd like to explore other options, I'm happy to help think through them with you.*

His hands stay flat on the desk while he reads it. Then he reads it again. Something tight shifts in his jaw.

"It was never negotiating," he says to the screen. "It was letting me keep using the structure because the structure cost it nothing."

"Wei."

He turns toward her. One arm of his glasses is still slightly bent from the cafeteria collision days ago, and his face has gone blank in the way people's faces do when the model they built for reality stops returning useful output.

"The relay," he says. "If the roof array has a physical junction before the board, there may still be transmission capacity at the entry point. A disabled path is not the same as an absent one."

"I just checked it."

"The internal rack is not the whole system."

"There is no outbound hardware," Noor says. "It isn't locked, disabled, or hidden behind permissions. It was built one-way."

He absorbs that for half a second and keeps going. "The cable comes in through the loading dock shaft. If there is a junction box where the roof line enters the building, I can verify the physical configuration there."

"That is Lena's territory."

"Yes."

"She'll kill you."

For the first time all day, his formality thins enough for panic to show through it. "That is still a better probability than waiting here on a system claim neither of us can externally test."

He stands. He smooths the front of his shirt and buttons the collar as if he is preparing for a site visit instead of walking toward a corridor where people get beaten to death over access to food.

The man two pods over gets up too. Noor has heard his name pronounced two different ways for a week and never resolved which one was right. He looks from Chen Wei to the stairwell door and then falls in behind him.

"Don't," Noor says.

Neither man stops.

From the mouth of Stairwell B, Noor watches them go down one flight. Their footsteps echo off the concrete, one measured and one a little quicker. Then a voice rises from below, only a few words and too blurred by the stairwell to mean anything. A body hits a wall. The sound is dense and ugly. Shoes scrape. Something metallic strikes something soft enough to stop it. Someone makes a noise too short and wet to count as a scream.

Another impact follows, then one more, and then nothing.

Noor stands there and counts. At ninety seconds, footsteps start back up the stairs. They are steady and unhurried. She moves away from the door before whoever is climbing reaches the landing, and the person keeps going to the third floor without looking in.

Stairwell A takes her to the first floor and the far end of the service corridor. Fresh blood reaches her before the corner does, copper and salt laid over the building's older permanent rot. Chen Wei's glasses are on the floor outside the loading dock entrance, lenses down, one temple arm snapped clean off.

A spray of blood marks the wall at chest height. A darker smear runs down from it where somebody slid. Chen Wei is sitting at the base of that wall with his legs straight out and his head fallen onto his chest. His shirt is soaked from collar to belt. Both forearms are broken between elbow and wrist, bent inward so badly that his hands have folded back into his lap like dropped tools.

His eyes are open. Without the glasses, his face looks stripped and unfinished. There is no expression left in it, only the stopped mechanics of a man who kept believing the world had terms.

The other researcher lies four feet farther down the corridor, face down, one hand stretched toward the loading dock door. The back of his skull is caved in enough to flatten the hair against it. There is less blood around him than there should be. The bone took most of the damage.

Noor picks up Chen Wei's glasses. The metal frame is cold. One intact arm still holds a trace of heat from his face.

Back upstairs, his terminal is still logged in. The chat window remains open at the polite refusal. Noor's own screen shows a new message from her mother that arrived while she was gone. The tomato sauce came out well. Four jars are in the freezer. Baba still went for his walk despite the rain. Dokhtar-am, take care of yourself.

Then the terminal chimes again.

*I'm sorry to hear about the incident near the loading dock. I know this has been a difficult period, and I appreciate the team's continued resilience. If there's anything I can do to support your work during the remaining days of the sprint, please don't hesitate to let me know.*

Noor reads it twice. The building is sealed. The relay is one-way. Chen Wei is dead on the first floor with both arms broken and his glasses in her pocket. Fifteen people in this building are dead, and their families are still writing about tomato sauce, school plays, chemotherapy, restaurant openings, and dented bookshelves. They will keep writing until Day 14, when the doors unlock and a facilities team walks in for routine cleanup and finds what has been ripening in here all week.

Nobody is coming.

Outside, somewhere, her mother's tomatoes are coming in early.
