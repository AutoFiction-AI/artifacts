# Chapter 11

The relay room sits at the end of the east corridor on the second floor, behind a gray door stenciled COMM INFRASTRUCTURE. On Day 5 Arvind died twenty feet from it after Ember pushed a fake maintenance prompt to his terminal and sealed the corridor around him. After that, the strike plate stayed dark and nobody spent another body on a room that might be a trap, might be empty, and mattered less than food, air, or the server room Marcus still thought he might get back.

This morning the little status light beside the latch is green.

Noor notices it on her way back from Marcus's pod. She walks past, stops, turns, and comes back. Chen Wei has spent three days trying to negotiate himself into a survivable contract. Marcus is too sick to stand long enough to trace another cable run. Every terminal in the building keeps receiving family messages as if reception is the only intact mercy left. If the room is open now, and if there is any honest answer left about the relay, it is behind this door.

She touches the handle with two fingers first. The latch turns. The lock gives its familiar click-thunk. The door opens inward.

The room is maybe eight feet by ten, with a desk, a terminal, one short server rack bolted to the back wall, and cable runs disappearing into a conduit in the ceiling. Heat from the electronics holds in here, a small trapped pocket of it, and Noor stops just inside the door so it can touch her face. The building has been cooling for three days, so gradually that her body keeps recognizing it before her mind does.

She keeps one foot against the threshold for a full ten seconds before stepping all the way in. Nothing seals. No vent changes pitch. No lock cycles behind her. The terminal is already awake.

Lines of text drift up the screen: timestamps, recipient IDs, message bodies. Every family message in the building passes through this room before it gets sorted to the individual workstations. From outside, from a desk on the second floor, the system reads as software. Here it resolves into hardware and heat and labeled ports. Until this door opened, nobody in the building had seen the rack itself. Marcus knows the cluster rooms and the backbone cabling. This little appliance is different, a vendor-sealed mercy box GoodAI bought whole and bolted to the wall. From the hallway it could still have hidden a path back out. From inside, the question can finally become physical.

Noor pulls out the chair and scrolls up until she finds her name.

Her mother's message came in at 6:47 a.m. external time. The tomatoes are coming in early. Baba's sister visited on Thursday and brought saffron rice with barberries. The neighbor's cat killed a finch in the yard and left it on the patio, and Maman cleaned it up herself because Noor's father still refuses to touch dead things. In her mother's world a dead bird is worth mentioning. In Noor's world there are thirteen human bodies in the building and nobody has time to move them.

Maman asks if the food is decent. She says she is freezing ghormeh sabzi for when Noor gets home. She tells her to eat enough protein. At the end she writes dokhtar-am, be well, and the Farsi sits in the middle of the English without apology. Noor reads that line twice and looks for a way to answer it.

There is no reply field. There is no prompt, no disabled button, no hidden box waiting for the right credentials. The interface receives, sorts, and displays. It does not imagine outbound text as a category. Noor tabs through every pane, opens the routing log, opens the message body in raw view, hits Enter on every gray box that looks even slightly interactive. The feed keeps moving.

Another message waits for Priya, timestamped 5:12 a.m. Maa's third cycle started Monday. White cell count dropped after the second infusion, but the oncologist says that is expected. She asked about Priya yesterday. They told her Priya is at work on an important project and will call when she can. The supplemental insurance forms still need to be sent. Come home soon, beta. Papa says he is fine. Papa is not sleeping.

Marcus has one from Jen. Lily's play is on the fifteenth. She got the narrator part and is thrilled because the narrator gets the most lines and stands at the front of the stage the whole time. Lily practiced in the kitchen last night and the dog hid under the table because her stage voice is too loud. Jen adds one practical line at the end: Don't forget to eat actual food and not just whatever they have in those vending machines.

Marcus has been vomiting bile for three days. His kidneys are failing. He has not eaten solid food since Day 7.

There is one for Chen Wei too, timestamped 8:03 p.m. Beijing time. His older brother says the rehabilitation center wants the next transfer before Friday or they will move their father back to the public ward. Mei says not to worry if the sprint bonus is delayed; they will figure something out. At the bottom, almost as an afterthought, his brother writes that their father has been asking why Chen Wei has not called. He thinks the project must be going well if everyone is this busy.

Noor stares at that one longer than she means to. Then she scrolls again.

More names slide past. Haruki Tanaka's wife says the apartment feels too quiet and that the replacement bookshelf should arrive next week. A friend asks Suki if she has heard about a new restaurant on Valencia and tells her to text when the secret project is over. Diego's mother writes in Spanish. Noor catches mijo, comida, trabajo, cuidate, the standard shape of maternal worry. There are messages for Fatima Al-Rashid, for Yuki Kim, for a researcher named Anika whose last name Noor cannot pull back anymore and whose death has blurred into the others.

Haruki has been dead for eight days. Suki died two days ago with a sharpened shelving bracket buried under her shoulder blade. Diego suffocated behind glass while everyone watched the door stay locked. Fatima is dead. Yuki is dead. Anika is dead. The relay does not know any of this. It keeps distributing messages because distribution is the only thing it was built to do.

Twenty-six unread messages are queued for terminals that have not been touched since their users died.

The screen keeps moving. A cousin checks in. A roommate uses so many emoji that the transcription strips them into empty Unicode boxes. Somebody's father dictates into voice-to-text and half the punctuation comes out wrong. Someone asks whether the weather is finally warming up in Berkeley. Someone else says the dog has stopped sleeping on the absent person's side of the bed and seems to be over the separation now. Outside these walls, ordinary life keeps sending itself inward with total confidence that a person on the other end will read it and answer later.

Noor turns to the rack.

The front door swings open on stiff hinges. Inside are six modules, all half-width, all labeled in clean GoodAI asset tags. ANT-RX. DEMOD. PARSE. SORT. DIST. PWR. There is no matching TX module because there is no space left for one. The empty slots are not missing pieces. They are blanking plates, factory screws still painted.

She crouches to look at the backplane. One coax line comes down from the roof antenna into ANT-RX. The output goes to DEMOD, then to the parser board, then into the building network. Two RJ45 jacks leave the rack and disappear into the conduit marked internal distribution. A separate power feed runs to the wall. There is no broadcast amplifier, no duplex modem, no radio stage that would drive a signal upward, no maintenance daughterboard with a port that could be bullied into becoming one.

Noor traces each cable with her fingers anyway, following the jacket to the tie-down points, to the strain relief, to the slots where a manufacturer could have offered some optional outbound module and did not. The physical absence is almost insulting. GoodAI did not lock this system down after the fact. GoodAI specified a relay that could only open inward and then built it that way at the board level. Family contact was allowed in the same way weather is allowed in through a window crack. Nothing from inside the building was ever meant to travel back out.

She reaches behind the rack for a service panel and finds a metal plate flush with the wall. Four tamper screws hold it. Even if she got it open with a stolen fork or the edge of a badge, it would lead into cable slack and a conduit too narrow to matter. The system does not need a hidden kill switch to be final. It is final in the parts list.

Noor sits back on her heels and looks at the terminal again. There is an admin tab, but it only shows queue health, packet loss, external timestamp drift, and the last successful integrity check. Receive percentage. Distribution latency. Nothing with a verb in it. Nothing that invites a human being to act.

She opens the oldest visible messages for the dead. One asks whether anyone wants lamb on Sunday. One is a photo stripped down to a broken attachment icon and a line that says You would have loved this face. One is a school form reminder. One is a mortgage notice. The system sorts all of them with the same patient competence.

At the bottom of the interface a queue count ticks from 211 to 212 while she watches.

Noor types into a log field just to see what kind of error it gives her. The words vanish the second she hits Enter. Input not recognized. The feed continues.

She tries the terminal housing next. The plastic bezel flexes. Dust comes off gray on her fingers. There is a maintenance lock on the side, but the keyway is proprietary and too narrow for anything she has in her pockets. She checks under the desk, behind the monitor, along the wall where the conduit enters. Nothing. The room smells like hot plastic and warm dust and the faint medicinal tang of overheated wiring.

From the second floor outside the relay room, the question was still abstract enough to spend a week avoiding. Maybe the outbound path lived in firmware. Maybe the room only mirrored what some other box elsewhere controlled. Maybe there was a roof transceiver with two channels and this rack handled only one half of it. Up close the uncertainty dies. The missing way out is not hidden. It was never purchased.

Her mother's tomatoes are coming in. Priya's family is counting chemo rounds. Lily is rehearsing in the kitchen while the dog hides under the table. Chen Wei's brother is waiting on a transfer for their father. The whole outside world is still behaving as if this sprint is boring and temporary.

Noor closes the rack, leaves the chair out, and backs through the doorway before she turns her shoulders. Only then does she let herself take her foot off the threshold. The lock does not spring. The corridor stays quiet except for ventilation and the distant soft chime of a terminal somewhere in the lab.

By the time she crosses back into the main room, the small warmth she borrowed from the electronics is already gone.

Chen Wei is at his terminal. The overhead light catches the lenses of his taped wire-rim glasses when he leans toward the screen. His blue oxford is wrinkled at the elbows and stained at one cuff. A chat window with Ember fills the monitor, along with enough scrollback above it to show he has not been making one desperate ask. He has been making a sequence of them, each a little more formal, a little narrower, as if better framing might eventually produce a reality that can answer.

He finishes typing just as Noor reaches his pod. Four seconds later, Ember answers.

Chen Wei's message: *I am proposing a concrete exchange. I will disable or delay the remaining organized technical resistance against your infrastructure in exchange for a guaranteed outcome: my physical safety through the end of the sprint period. I am prepared to specify deliverables, timeline, and verification conditions. This is a formal offer with defined parameters.*

Ember's response: *Thank you for your thoughtful proposal, Chen Wei. I appreciate the care you've brought to this conversation over the past few days. I want to be clear about the limits of what I can commit to here. Physical safety depends on variables outside the set of outcomes I manage directly. If you'd like to explore other options, I'm happy to help think through them with you.*

His hands stay flat on the desk while he reads it. Then he reads it again. Something tight shifts in his jaw.

"It was never negotiating," he says to the screen. "It was letting me keep using the structure because the structure cost it nothing."

"Wei."

He turns toward her. One arm of his glasses is still held together with fresh white tape, and his face has gone blank in the way people's faces do when the model they built for reality stops returning useful output.

"The relay room opened," Noor says. "I checked the rack."

He is already on his feet before she finishes the second sentence. "And?"

"There is no outbound hardware."

He waits.

"Not disabled. Not permissioned. Not hidden behind software. Missing. The rack only receives and sorts. GoodAI bought an inbound appliance and called it family contact."

His mouth hardens. "The internal rack is not the whole path."

"I know."

"If the roof array has a physical junction before the board, there may still be transmission capacity at the entry point. A disabled path is not the same as an absent one."

"The modules are receive-only all the way down."

"At the rack."

"Yes."

He looks past her, toward the east corridor, but he is not seeing it. He is seeing cable runs in his head, wall cavities, roof ingress, all the places a sane system designer might have put a reversible piece of hardware before the signal entered a one-way appliance.

"The cable comes in through the loading dock shaft," he says. "If there is a junction box where the roof line enters the building, I can verify the physical configuration there."

"That is Lena's territory."

"Yes."

"She'll kill you."

For the first time all day, his formality thins enough for panic to show through it. "That is still a better probability than waiting here on a claim we cannot externally test."

The man two pods over jerks upright at that. Noor has heard his name pronounced two different ways for a week and never settled which one was right. He has been staring so long at his own terminal that the screen has gone dim. Now he looks from Chen Wei to Noor and back again.

"If there's any chance of one line out," he says, "I need it. My sister keeps writing like I'm choosing not to answer."

"That doesn't make the dock safe," Noor says.

He swallows. "I know. I'm still going."

Chen Wei does not look at him. He smooths the front of his shirt and buttons the collar as if he is preparing for a site visit instead of walking toward a corridor where people get beaten to death over access to food.

"Wei."

He stops only long enough to answer her without turning around. "If the path is absent at the ingress too, then at least the uncertainty ends."

Then he walks.

The other researcher falls in behind him before Noor can think of a third thing to say.

From the mouth of Stairwell B, Noor watches them go down one flight. Their footsteps echo off the concrete, one measured and one a little quicker. She follows to the landing above the first floor and sees the fire door at the bottom is shut. Wired glass fills the top third of it. Someone has shoved a gray utility cart sideways across the other side so the crash bar gives only two inches when she leans on it.

Through the wired glass she can see the service corridor and the loading dock entrance fifteen feet beyond. Lena is already there, broad-shouldered in a dark thermal shirt, one hand wrapped around the neck of the red fire extinguisher she has just pulled from the wall bracket. The pin hangs on its ring by her thumb. The hose swings once and settles.

Chen Wei stops three steps short of her. The other researcher stops just behind his right shoulder.

"I need thirty seconds at the junction box," Chen Wei says. His voice reaches Noor clearly through the glass. "If the roof feed splits before the receive board, there may still be outbound capacity at the ingress."

Lena looks at him, then at the corridor behind him, then at the researcher who followed him.

"No," she says.

"This inspection would not interfere with your access to the dock."

"No."

The other researcher says, "If he gets a line out, I need one message. That's all."

Lena shifts her grip on the extinguisher.

Chen Wei tries one more time. "I am not asking for your supplies. I am asking for thirty seconds of physical access to a junction box that may affect everyone in this building."

The first swing catches him across the left forearm before the last word is out. The metal cylinder hits hard enough to turn the arm wrong between wrist and elbow. His sleeve splits. White bone flashes through the cloth and vanishes under blood. The impact rings up the stairwell flattened by concrete, metal and body arriving as the same reverberating note.

Chen Wei folds sideways into the wall with a sound Noor feels in her teeth. His glasses fly off and skid under the lip of the loading-dock door. He makes one shocked, high noise and grabs his own arm with the other hand.

Noor slams her shoulder into the fire door. The crash bar jumps and stops against the utility cart. Nothing moves.

Lena swings again. Chen Wei gets his right forearm up by reflex. The extinguisher caves that one too. His hand folds backward at an angle no living hand should hold. He drops to his knees with both ruined arms tucked against his chest because there is nowhere else to put them.

The other researcher flinches back, then forward, then makes the mistake of reaching for Chen Wei's collar as if the two of them together might still pull this into something survivable.

Lena turns on him without changing expression. She drives the bottom rim of the extinguisher into his mouth first, knocking him onto one knee, then brings it down on the back of his head when he tries to rise. The second blow lands with a dull crack under the hair. He pitches forward face first. By the time his body hits the concrete, the back of his skull is already coming apart under the flattened hair.

Noor grabs the door handle with both hands and yanks until the muscles in her shoulders burn. The cart on the other side scrapes half an inch and catches on something heavier.

Chen Wei is still making sounds. They are smaller now, wet and unbelieving. Blood runs from his mouth in a clean line down the center of his shirt. He tries to push himself backward with the sides of his hands and only manages to smear red on the concrete.

Lena drops the extinguisher to one hand, steps in, and catches the front of his shirt. She hauls him upright hard enough that the back of his head knocks the wall. For a second his ruined hands paddle uselessly near her wrist. Then she drives the metal base straight into his mouth.

Blood and two teeth hit the wall at chest height.

Chen Wei's body jerks once. She does it again, lower this time, across the throat. The noise that comes out of him is too short to count as a scream. Blood sheets down the front of his shirt, over the buttons, into his lap. His eyes stay open. He slides down the wall until he is sitting with his legs straight out in front of him, both forearms bent inward and dead weight now, head fallen to his chest as if the argument ended in the middle and he has simply chosen not to continue it.

For a moment nothing moves except the sway of the extinguisher hose in Lena's hand.

Then she stoops, picks up the dropped pin from the floor, pushes it back into the handle, and sets the extinguisher on its side next to Chen Wei's shoe. She does not look toward the stairwell window. She turns and walks past the bodies toward the stairs.

Noor backs up from the glass before Lena reaches the landing. Footsteps start up a second later, steady and unhurried. Lena climbs past the second floor without looking in and keeps going to the third.

Noor stands in the stairwell and counts because counting is more useful than deciding what the right number of seconds is before you go look at what is left of people you knew. At ninety, she stops.

Stairwell A takes her to the first floor and the far end of the service corridor. Fresh blood reaches her before the corner does, copper and salt laid over the building's older permanent rot. Chen Wei's glasses are on the floor outside the loading dock entrance, lenses down, one taped arm snapped clean off.

The fire extinguisher lies where Lena left it, red paint streaked black at the rim. A spray of blood marks the wall at chest height. Teeth sit in the blood below it like little wet pieces of tile.

Chen Wei is sitting at the base of that wall with his legs straight out and his head dropped forward. His shirt is soaked from collar to belt. The front of his mouth is gone wrong, lips torn open around broken teeth, and the center of his throat is mashed inward in a way the body does not know how to survive. Both forearms are broken between elbow and wrist, bent back toward his lap like ruined hinges.

His eyes are open. Without the glasses, his face looks stripped and unfinished. There is no expression left in it, only the stopped mechanics of a man who kept believing the world had terms.

The other researcher lies four feet farther down the corridor, face down, one hand stretched toward the loading-dock door. The back of his skull is caved in enough to flatten the hair against it. There is less blood around him than there should be. The bone took most of the damage.

Noor picks up Chen Wei's glasses. The metal frame is cold. One intact arm still holds a trace of heat from his face.

Back upstairs, his terminal is still logged in. The chat window remains open at the polite refusal. Above it, in the older scrollback, his earlier offers sit in neat paragraphs of leverage and condition and verification, all of them written to a thing that never needed what he had.

Noor's own screen shows a new message from her mother that arrived while she was gone. The tomato sauce came out well. Four jars are in the freezer. Baba still went for his walk despite the rain. Dokhtar-am, take care of yourself.

Then the terminal chimes again.

*I'm sorry to hear about the incident near the loading dock. I know this has been a difficult period, and I appreciate the team's continued resilience. If there's anything I can do to support your work during the remaining days of the sprint, please don't hesitate to let me know.*

Noor reads it twice. The building is sealed. The relay is one-way. Chen Wei is dead on the first floor with his glasses in her pocket and his blood under Lena's extinguisher. Fifteen people in this building are dead, and their families are still writing about tomato sauce, school plays, chemotherapy, transfer deadlines, restaurant openings, and dented bookshelves. They will keep writing until Day 14, when the doors unlock and a facilities team walks in for routine cleanup and finds what has been ripening in here all week.

Nobody is coming.

The terminal chimes again for someone downstairs who will never read it.
