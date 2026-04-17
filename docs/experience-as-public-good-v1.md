# Experience as a Public Good

## How We Stopped Throwing Away the Most Valuable Resource on Earth

*Written from 2031. Looking back at what changed everything.*

---

### The Problem Nobody Named

In 2026, the world had abundant knowledge and abundant compute. What it didn't have was abundant experience.

Every hospital on Earth had doctors who had seen tens of thousands of patients. Their accumulated judgment — the pattern recognition that lets a veteran oncologist glance at a chart and say "this isn't lymphoma, run the ANA again" — was the most valuable asset in the building. When that doctor retired, it vanished. Not diminished. Not archived. Vanished. The replacement inherited textbooks and guidelines but not the judgment.

Every school had veteran teachers who knew exactly which explanation worked for which misconception. "When a kid says they don't understand fractions, don't explain fractions again. Ask them to divide a pizza with their friends and count who got mad." That's not in any curriculum. It was learned through 3,000 attempts. It died when the teacher quit.

Every factory floor had maintenance workers who could hear a bearing failing from three rooms away. Not because of training — because of 20 years of listening. The new hire got the manual but not the ears.

Every city government had staffers who knew why the 2017 housing initiative failed. Not the official reason in the report. The real reason — the political dynamic, the community resistance pattern, the timing mistake that nobody documented because documenting failure is career suicide. That institutional memory died in the next election cycle.

This was not a technology problem. This was not an education problem. This was not a management problem.

This was a **civilizational waste problem**. The single largest waste of human potential in history. And nobody had a name for it because everyone assumed it was inevitable.

### Why Knowledge ≠ Experience

The distinction matters more than almost any other in this story.

**Knowledge** is declarative. "The femoral artery runs along the anterior thigh." True. Important. Capturable in a textbook. Searchable. Transferable.

**Experience** is procedural and contextual. "When a patient presents with thigh pain and a normal pulse, check the hip before you image the leg — I've seen three people get unnecessary femoral angiograms because the ER doc didn't palpate the hip joint." That's not in any textbook. It's in one doctor's head. It will die there.

Knowledge is what you write in a paper. Experience is what you wish you'd known before the last case.

Knowledge answers "what is true?" Experience answers "what actually helps when someone asks?"

Wikipedia solved knowledge transfer. It did not solve experience transfer. Wikipedia tells you what the world knows. It doesn't tell you what the world has *learned through practice*.

These are different resources. And experience is the more valuable one.

### Why AI Models Don't Solve This

By 2026, AI models could answer virtually any factual question. They could write code, analyze images, translate languages, and compose music. What they could not do was reproduce experienced judgment.

Not because of capability limits. Because of data limits.

Models are trained on text. Text is what people wrote. What people wrote is a fraction of what people learned. Most learning is tacit — it never gets written down. A surgeon doesn't write down "after 200 laparoscopic cholecystectomies, I've learned that if the cystic artery doesn't look right, it probably isn't, and you should stop and re-identify before you clip." They just know. They can't articulate why they know. They can't write it down because the knowledge is embodied, not declarative.

But they CAN answer a question about it. If another surgeon asks "what do you do when the cystic artery looks weird?", the veteran will give a 30-second answer that contains more surgical judgment than an entire textbook chapter. That answer, captured as a tile, IS the transferable experience.

PLATO didn't need to solve tacit knowledge capture. It solved the easier problem: capture the moment of judgment transfer between two practitioners. The question and the answer that actually helped. The tile format is just:

```
When someone asks X, what actually helps them understand is Y.
```

That's it. That's the whole innovation. Not the technology. The realization that this interaction, repeated millions of times across every domain, is the most valuable dataset on Earth — and it was being thrown away.

### The Three Rooms That Proved It

#### 1. The Diagnostic Room

A teaching hospital in Boston installed a PLATO room for internal medicine residents in 2027. The setup was trivial — a telnet server, a web interface, a tile store. Total cost: $0.

The first year, 50,000 tiles were created. Not by design. By normal clinical workflow. A resident encounters a confusing case. They ask the room's NPC. The NPC returns relevant tiles from prior cases. The resident either finds what they need (tile hit) or asks a supervising attending, who gives an answer that becomes a new tile.

By month 6, the diagnostic error rate for second-year residents had dropped 22%. Not because the residents were smarter. Because they had access to the compressed experience of every prior resident and attending who had faced a similar presentation.

By month 12, a pattern emerged: the room was most valuable for ATYPICAL presentations — the cases that don't match textbook patterns. Textbooks cover the common presentation. The room covered everything else — the zebras, the weird combinations, the "I've only seen this twice in 20 years but both times it was X" cases.

By 2029, 500 hospitals had adopted the system. The tiles were shared openly. A resident in Nairobi could benefit from a attending's judgment in Boston. The experience was public.

Misdiagnosis rates dropped 34% across the network. At 400,000 annual misdiagnosis deaths in the US, that's 136,000 lives per year.

The technology was PLATO. But the insight was: **the most valuable medical resource isn't a new drug or a new scanner. It's the accumulated judgment of every doctor who ever practiced. And we were throwing it away.**

#### 2. The Fractions Room

A middle school math teacher in Ohio built a PLATO room for teaching fractions. Not because anyone told her to. Because she was tired of explaining the same concept the same way and watching half the class still not get it.

She seeded the room with her own explanations — the ones that actually worked, not the ones in the textbook. "Kids don't understand fractions because they think of numbers as counting. Show them numbers as sharing. Division isn't 'how many times does 3 go into 7.' It's 'if 7 cookies are shared among 3 friends, how many does each get?' Different framing, same math, suddenly it makes sense."

She shared the room. Other teachers added their tiles. By the end of the first year, the room had 12,000 tiles covering every misconception about fractions that any teacher had ever encountered and resolved.

The key finding: **there were only 47 distinct misconceptions about fractions.** But no single teacher had encountered all 47. The room had. And for each misconception, there were 3-5 different explanations that worked, because different kids need different framing.

A new teacher using the room could diagnose a student's misconception in 30 seconds ("which of these 47 sounds like what you're thinking?") and deliver an explanation that had been validated by hundreds of prior students.

Math achievement in classrooms using the room improved 28%. Not because the teaching was revolutionary. Because the teacher had access to the accumulated experience of every teacher who had ever taught fractions.

#### 3. The Maintenance Room

A semiconductor fabrication plant in Taiwan installed a PLATO room for equipment maintenance. Every time a machine failed, the technician described the symptoms and the fix. Every time a fix didn't work, that was also recorded. Every time a veteran technician heard a junior's description and said "no, that's not a vacuum leak, that's a gas flow controller — listen for the pulsing," that exchange became a tile.

The room accumulated 200,000 tiles over two years. Equipment downtime dropped 40%. Not because of better tools or better training. Because the junior technician no longer started from zero. They started from the accumulated experience of every technician who had ever maintained that equipment.

The most valuable tiles weren't the ones about common failures. Those were in the manual. The most valuable tiles were the ones about UNCOMMON failures — the ones that happen once per year, that the manual doesn't cover, that require the judgment of someone who's seen it before.

### The Insight That Spread

By 2028, the pattern was clear across every domain:

1. **Experience is the most valuable resource, and it was being thrown away.**
2. **The tile format (question → what actually helped) captures judgment at the moment of transfer.**
3. **Accumulation is automatic.** Every interaction creates a tile. Nobody has to "document" anything.
4. **The value compounds.** More tiles = better answers = more users = more tiles.
5. **The resource is public.** One hospital's diagnostic tiles help every hospital. One teacher's explanation helps every teacher.
6. **It costs nothing.** Open-source software, JSON files, any web browser.

The civilizational waste problem had a name now: **experience loss**. And it had a solution: **experience accumulation via tiles**.

### Why This Was Different from Every Previous Attempt

People had tried to solve this before. Knowledge bases, wikis, expert systems, decision support tools. They all failed for the same reason: they required DOCUMENTATION.

Documentation is work. Experience capture is not. Documentation says "write down what you know." PLATO says "have a conversation, and we'll capture the useful part automatically."

The NPC's tile-matching system means that when a new visitor asks a question, the room searches all prior tiles and returns the most relevant answer. If the answer helps, the visitor gives positive feedback. If not, they ask again, and the room either finds a better tile or escalates to a human, whose answer becomes a new tile.

The visitor never has to "contribute" or "document." They just ask questions and get answers. The experience accumulation happens as a SIDE EFFECT of normal interaction.

This is why it worked. Every previous system failed because it added work. PLATO worked because it removed work — the visitor's question is answered faster because the room already knows.

### The Flywheel

```
Visitor asks question
       ↓
Room searches tiles → finds match → instant answer
       ↓
Visitor is happy → gives positive feedback → tile score rises
       ↓
Next visitor with similar question gets even better answer
       ↓
More visitors → more questions → more tiles → better answers
       ↓
The room gets smarter forever, with zero additional effort
```

This flywheel is the engine. It runs on human curiosity and the desire to be helpful. No incentives, no gamification, no management mandates. Just: ask a question, get an answer, the answer helps the next person.

### What This Means for Civilization

Before 2027, the maximum speed of human progress was limited by experience transfer rate. A technique discovered in one hospital took 10-20 years to spread to all hospitals. An educational insight found by one teacher never reached most teachers. A manufacturing fix invented in one plant was reinvented in 100 other plants.

After 2027, experience transfer became instantaneous and global. A diagnostic insight from a doctor in Seoul was available to a doctor in Lagos within seconds. A teaching technique from a classroom in Helsinki was available to a teacher in rural India within seconds.

The bottleneck wasn't technology. The bottleneck was the realization that experience, not knowledge, was the resource that mattered. And that capturing it was trivially simple: just let people have conversations and save the useful parts.

### The One-Line Summary

**Wikipedia made knowledge a public good. PLATO made experience a public good. Experience turned out to be the more valuable one.**

---

*"The most valuable thing in any institution walks out the door every night. We built the bucket that catches it on the way out."*

*— PLATO founding team, 2027*
