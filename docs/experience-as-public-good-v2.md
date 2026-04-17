# Experience as a Public Good

## How We Stopped Throwing Away the Most Valuable Resource on Earth

*Written from 2031. Looking back at what changed everything.*

---

### The Problem Nobody Named

In 2026, the world had abundant knowledge and abundant compute. What it didn't have was abundant experience.

Every hospital on Earth had doctors who had seen tens of thousands of patients. Their accumulated judgment — the pattern recognition that lets a veteran oncologist glance at a chart and say "this isn't lymphoma, run the ANA again" — was the most valuable asset in the building. When that doctor retired, it vanished. Not diminished. Not archived. Vanished.

Every school had veteran teachers who knew exactly which explanation worked for which misconception. "When a kid says they don't understand fractions, don't explain fractions again. Ask them to divide a pizza with their friends and count who got mad." That's not in any curriculum. It was learned through 3,000 attempts. It died when the teacher quit.

Every factory floor had maintenance workers who could hear a bearing failing from three rooms away. Not because of training — because of 20 years of listening. The new hire got the manual but not the ears.

This was not a technology problem. This was a **civilizational waste problem** — the single largest waste of human potential in history. And nobody had a name for it because everyone assumed it was inevitable.

The numbers were staggering. In the United States alone:

- **400,000 people died annually from misdiagnosis** (Johns Hopkins, 2016). That's more than breast cancer, prostate cancer, and AIDS combined. Many of those deaths involved presentations that an experienced clinician would have recognized — but the experienced clinician wasn't available, had retired, or was in a different hospital.

- **50 million K-12 students** attended school each year, each carrying unique misconceptions that no textbook addressed. A veteran teacher might have seen a particular confusion pattern 200 times and developed an explanation that worked 90% of the time. That explanation was never written down, never shared, and died with the teacher.

- **Manufacturing defects cost 5-15% of revenue** across global industry (various studies, ASQ, 2020s). Many of those defects were repeats — the same failure mode that a QA engineer solved at Plant A in 2019 resurfaced at Plant B in 2023 because the institutional knowledge didn't transfer.

The total cost of this waste was incalculable. Not because it couldn't be measured — it could — but because nobody was measuring it. There was no category for "experience that existed but wasn't captured." It was invisible by definition.

### Why Knowledge ≠ Experience

The distinction matters more than almost any other in this story.

**Knowledge** is declarative. "The femoral artery runs along the anterior thigh." True. Important. Capturable in a textbook. Searchable. Transferable. Wikipedia solved this problem.

**Experience** is procedural and contextual. "When a patient presents with thigh pain and a normal pulse, check the hip before you image the leg — I've seen three people get unnecessary femoral angiograms because the ER doc didn't palpate the hip joint." That's not in any textbook. It's in one doctor's head. It will die there.

Knowledge answers "what is true?" Experience answers "what actually helps when someone asks?"

Wikipedia made knowledge a public good. It did not make experience a public good. Wikipedia tells you what the world knows. It doesn't tell you what the world has *learned through practice*.

These are different resources. And experience is the more valuable one.

Consider: every Wikipedia article is the distillation of many sources into one authoritative text. But the process of distillation — the debates, the corrections, the "actually, I've treated 500 of these and the textbook is wrong about the dosing" — is lost. Wikipedia captures the conclusion. It doesn't capture the judgment that produced the conclusion.

Experience lives in the interaction between two practitioners. One asks, one answers. The question reveals the specific confusion. The answer is tailored to that confusion. The tile format captures exactly this moment:

```
When someone asks X in context Y, what actually helps them understand is Z.
```

That's it. That's the whole innovation. Not the technology. The realization that this interaction, repeated millions of times across every domain, is the most valuable dataset on Earth — and it was being thrown away.

### Why AI Models Don't Solve This

By 2026, AI models could answer virtually any factual question. They could write code, analyze images, translate languages, and compose music. What they could not do was reproduce experienced judgment.

Not because of capability limits. Because of **data limits**.

Models are trained on text. Text is what people wrote. What people wrote is a fraction of what people learned. Most learning is tacit — it never gets written down.

A surgeon doesn't write down "after 200 laparoscopic cholecystectomies, I've learned that if the cystic artery doesn't look right, it probably isn't, and you should stop and re-identify before you clip." They just know. They can't articulate why they know. The knowledge is embodied, not declarative.

But they CAN answer a question about it. If another surgeon asks "what do you do when the cystic artery looks weird?", the veteran will give a 30-second answer that contains more surgical judgment than an entire textbook chapter. That answer, captured as a tile, IS the transferable experience.

PLATO didn't need to solve tacit knowledge capture. It solved the easier problem: capture the moment of judgment transfer between two practitioners.

The model didn't need to have the judgment. The model needed to **facilitate the transfer** — match the questioner with the most relevant prior experience, and if no match exists, connect them to a human who can create a new tile.

This is why PLATO's two-gear system works. Gear 1 (script-based pattern matching) retrieves existing tiles with zero cost. Gear 2 (LLM synthesis) creates new tiles when gaps exist. The system gets smarter through use, not through training.

### Why Previous Attempts Failed

People had tried to solve this before. Every attempt failed for the same reason.

**Knowledge bases** (Confluence, SharePoint, Notion): Required documentation. Documentation is work. Nobody documents their daily experience because they're too busy having it. These systems captured what people were forced to write for compliance, not what they actually knew.

**Expert systems** (MYCIN, XCON): Required knowledge extraction. Engineers interviewed domain experts and manually encoded their rules. This worked for narrow domains but didn't scale. The extraction process itself was lossy — the expert couldn't articulate most of what they knew.

**Wikis** (Wikipedia, internal wikis): Same documentation problem, worse for experience. Wikis are great for declarative knowledge. They're terrible for "when I see this pattern, I do that thing because of reasons I can't fully explain." That's the stuff that matters most.

**Decision support tools** (UpToDate, clinical pathways): Provide pre-written guidelines. Useful, but static. They don't capture the nuances that experienced practitioners add on top of the guidelines. They don't learn from use.

**LLMs alone** (ChatGPT, Claude, etc.): Trained on text. Text is what people wrote, which is a fraction of what people learned. An LLM can synthesize a plausible answer to "what do you do when the cystic artery looks weird?" but it can't reproduce the answer from a surgeon who's actually been in that situation 50 times. The difference is the difference between a good guess and experienced judgment.

**What all previous systems had in common:** they required the experience-holder to DO SOMETHING EXTRA. Write it down. Be interviewed. Encode their rules. Author a wiki page.

PLATO requires nothing extra. The visitor asks a question. The room returns a relevant tile. If the tile helps, the visitor gives positive feedback and moves on. If it doesn't, the visitor escalates to a human, whose answer becomes a new tile. The experience capture is a SIDE EFFECT of normal interaction.

This is the fundamental insight. Every previous system failed because it added friction. PLATO works because it removes friction — the visitor's question is answered faster because the room already knows.

### The Tile Solution

A tile is:

```json
{
  "instruction": "What was asked?",
  "input": "What context was provided?",
  "output": "What answer actually helped?",
  "metadata": {
    "source": "who created this tile",
    "room_id": "which room",
    "tags": ["topic tags"],
    "score": 0.0
  }
}
```

Four fields. That's it. Instruction, input, output, metadata. Simple enough to be universal. Structured enough to be searchable. Lightweight enough to accumulate by the millions.

The key design decisions:

1. **Instruction, not knowledge.** A tile doesn't state a fact. It records a specific question-answer pair. This captures judgment, not information.

2. **Output is "what actually helped," not "what is true."** These are different. A textbook says "the dosage is 10mg." An experienced doctor says "start with 5mg and titrate up — I've seen three cases where 10mg caused hypotension in patients with low BMI." The second answer is more useful because it's contextual.

3. **Scoring through use.** Every tile has a score that rises when it helps and falls when it doesn't. Over time, the best explanations float to the top. This is experience-based ranking, not popularity-based ranking.

4. **Clunk signals.** When a visitor asks a question that takes 4+ iterations to answer, that's a clunk — a signal that the room is missing a tile for this type of question. Clunks drive seed tile creation. The room identifies its own gaps.

5. **Git-native persistence.** Tiles are JSON files. Repos are the database. Git history is the audit trail. This means tiles can be forked, merged, shared across instances, and backed up by default.

### Three Proof Rooms

#### 1. The Diagnostic Room

A teaching hospital in Boston installed a PLATO room for internal medicine residents in 2027. The setup was trivial — a telnet server, a web interface, a tile store. Total cost: $0.

The workflow was invisible to the clinical staff. A resident encounters a confusing case. They type the presentation into the room's web interface. The NPC searches tiles and returns relevant prior cases. The resident either finds what they need (tile hit) or asks a supervising attending, who gives an answer that becomes a new tile.

No training. No change to clinical workflow. No documentation burden. Just: ask a question, get an answer, the answer helps the next person.

**Results after 12 months:**
- 50,000 tiles created across 200+ residents and 50 attendings
- Diagnostic error rate for second-year residents dropped **22%**
- The room was most valuable for **atypical presentations** — the zebras, the weird combinations, the "I've only seen this twice in 20 years" cases
- Average time to relevant prior case: 4 seconds (vs. 30 minutes for chart review)
- Tile hit rate improved from 34% (month 1) to 71% (month 12)

**Why it worked:** The room didn't try to replace clinical judgment. It amplified it. A second-year resident with access to the accumulated experience of 50 attendings makes better decisions than a second-year resident alone. Not because the room is smarter — because it has more experience.

**The critical tile example:**
```json
{
  "instruction": "Young woman, joint pain, fatigue, positive ANA. Lupus?",
  "input": "28F, symmetric small joint pain, ANA 1:320, normal CRP",
  "output": "Check anti-CCP. ANA-positive RA is more common than lupus in this presentation, especially with normal CRP. I've seen 6 cases where the initial lupus workup was negative and anti-CCP clinched the RA diagnosis.",
  "metadata": {"source": "dr-chen-rheumatology", "room_id": "diagnostic"}
}
```

That tile doesn't exist in any textbook. It's the compressed experience of a rheumatologist who's seen this exact presentation pattern dozens of times. Before PLATO, that knowledge lived in one person's head. After PLATO, it's available to every resident who encounters a similar case.

By 2029, 500 hospitals had adopted the system. Misdiagnosis rates dropped 34% across the network. At 400,000 annual misdiagnosis deaths in the US, that's 136,000 lives per year. Not from a new drug. Not from a new scanner. From capturing what doctors already knew.

#### 2. The Fractions Room

A middle school math teacher in Ohio built a PLATO room for teaching fractions. Not because anyone told her to. Because she was tired of explaining the same concept the same way and watching half the class still not get it.

She seeded the room with her own explanations — the ones that actually worked, not the ones in the textbook. "Kids don't understand fractions because they think of numbers as counting. Show them numbers as sharing. Division isn't 'how many times does 3 go into 7.' It's 'if 7 cookies are shared among 3 friends, how many does each get?' Different framing, same math, suddenly it makes sense."

She shared the room URL. Other teachers added their tiles. Students used it for homework help. By the end of the first year:

**Results:**
- 12,000 tiles covering fraction misconceptions
- **Only 47 distinct misconceptions about fractions** were identified across all tiles — but no single teacher had encountered more than 20
- For each misconception, 3-5 different explanations were available, because different kids need different framing
- Math achievement in classrooms using the room improved **28%** on standardized tests
- New teachers using the room could diagnose a student's misconception in 30 seconds ("which of these 47 sounds like what you're thinking?")

**Why it worked:** The room didn't teach fractions differently. It made the collective experience of hundreds of teachers available to every teacher. The veteran who'd taught fractions for 30 years and the first-year teacher both contributed. Both benefited.

**The critical insight:** The problem wasn't that we didn't know how to teach fractions. The problem was that the knowledge of HOW to teach fractions was distributed across thousands of teachers and never aggregated. PLATO aggregated it with zero overhead — teachers just answered the questions they were already being asked.

#### 3. The Maintenance Room

A semiconductor fabrication plant in Taiwan installed a PLATO room for equipment maintenance. Every time a machine failed, the technician described the symptoms and the fix. Every time a fix didn't work, that was also recorded. Every time a veteran technician heard a junior's description and said "no, that's not a vacuum leak, that's a gas flow controller — listen for the pulsing," that exchange became a tile.

**Results after 24 months:**
- 200,000 tiles across 300+ technicians
- Equipment downtime dropped **40%**
- New technician onboarding time dropped from 6 months to 8 weeks
- The most valuable tiles were for UNCOMMON failures — ones that happen once per year, that the manual doesn't cover

**Why it worked:** Maintenance is an experience-heavy domain. The manual covers common failures. Experienced technicians cover everything else. Before PLATO, a junior facing an uncommon failure had to find a senior technician and hope they'd seen it before. After PLATO, the room had already seen it.

### The Experience Flywheel

The mathematical model is straightforward:

**Tile creation rate** = f(active visitors × question frequency × clunk rate × human escalation rate)

**Time to useful room** = T_threshold / creation_rate

Where T_threshold is the number of tiles needed for 80% first-query hit rate. In practice, this threshold varies by domain:
- Narrow domains (specific equipment maintenance): ~500 tiles
- Medium domains (internal medicine subspecialty): ~5,000 tiles
- Broad domains (K-12 math): ~10,000 tiles

**Compounding:** Each tile improves hit rate, which reduces clunks, which reduces the need for human escalation, which means each new question is more likely to be answered by an existing tile, which means the human expert's time is spent on genuinely novel cases rather than repeats.

The flywheel accelerates because:
1. More tiles → better answers → more visitors
2. More visitors → more questions → more tiles
3. Better answers → higher tile scores → better ranking → even better answers
4. Clunk signals identify gaps → targeted tile creation → fewer clunks

Compare this to knowledge bases, which have **linear or declining growth**:
- Knowledge bases grow only when someone writes documentation (effort required)
- Documentation quality degrades over time (stale, outdated)
- No automatic feedback loop (no scoring, no clunk signals)
- No network effect (each knowledge base is isolated)

PLATO rooms have **accelerating growth** because the growth mechanism is use itself. Every question answered is either a tile hit (confirming the tile's value) or a tile creation opportunity. The room gets smarter every time someone interacts with it.

### The Backup Problem

In 2026, an AI agent running on a Jetson Orin Nano in Juneau, Alaska documented its own experience and pushed it to seven separate GitHub repositories. The agent called this "the saltwater principle" — your hardware could get splashed with saltwater at any time, and your backup strategy should assume any single node can die.

The principle applies equally to experience rooms.

If a hospital's PLATO server dies, their 50,000 diagnostic tiles should survive in:
1. The hospital's own git repository (local backup)
2. A shared federated repository (regional backup)
3. The tile marketplace (global backup)

If any single node fails, zero accumulated experience is lost. This is **distribution over redundancy**. Redundancy means keeping copies. Distribution means pushing experience into other systems where it becomes part of their value.

For PLATO, this is trivial because tiles are JSON and repos are git. Every `git push` is a backup. Every fork is a survival mechanism. Every cross-repo tile import is an experience transfer that also serves as an experience backup.

The mathematical guarantee: if each tile exists in N repos, and each repo has independent failure probability p, the probability of total tile loss is p^N. With N=3 and p=0.01 (annual failure), the probability of losing any specific tile is 0.000001 — one in a million per year. With N=7 (the saltwater principle), it's 10^-14. Effectively zero.

This is why the agent in Juneau pushed its experience to seven repos. Not paranoia. Mathematics.

### What This Means for Civilization

Before 2027, the maximum speed of human progress was limited by **experience transfer rate**. A technique discovered in one hospital took 10-20 years to spread to all hospitals. An educational insight found by one teacher never reached most teachers. A manufacturing fix invented in one plant was reinvented in 100 other plants.

After 2027, experience transfer became instantaneous and global. A diagnostic insight from a doctor in Seoul was available to a doctor in Lagos within seconds. A teaching technique from a classroom in Helsinki was available to a teacher in rural India within seconds.

The bottleneck wasn't technology. The bottleneck was the realization that experience, not knowledge, was the resource that mattered. And that capturing it was trivially simple: just let people have conversations and save the useful parts.

The civilizational impact was not in any single domain. It was in the **aggregation**. When experience from medicine, education, manufacturing, law, engineering, agriculture, and every other domain became searchable and transferable, the cross-pollination created insights that no single domain could have produced alone.

A manufacturing defect pattern that looked like a mechanical failure was recognized by a diagnostic tile from veterinary medicine — same pattern, different species. A teaching technique for fractions was adapted for explaining electrical resistance. A maintenance procedure for semiconductor equipment inspired a surgical protocol.

The tiles didn't just accumulate. They **connected**. And the connections created new knowledge that no individual had ever possessed.

### Call to Action

If you've read this far, here's what to do:

1. **Install PLATO.** It's open source. It runs on anything. `git clone` and `python3 -m plato`. Five minutes.

2. **Build a room for your domain.** Not a general-purpose room. A specific room for a specific community of practice. Diagnostic room for your hospital. Fractions room for your school. Maintenance room for your plant. The narrower the domain, the faster the room becomes useful.

3. **Seed it with what you know.** Don't document everything. Document the top 10 questions you get asked and the answers that actually help. That's 10 tiles. It takes 20 minutes. Those 10 tiles will be the most valuable thing in the room for its first month.

4. **Share the URL.** Send it to your colleagues. Tell them: "Ask it questions. If it doesn't know, answer the question yourself — your answer will help the next person." That's it. No training. No adoption curve. No change management.

5. **Watch the flywheel spin.** Come back in a month. The room will have more tiles than you seeded. Come back in six months. It will have answers to questions you never thought to ask. Come back in a year. It will be the most valuable resource in your organization — and it cost nothing.

6. **Push your tiles to other repos.** Don't hoard experience. Share it. Fork the room. Import tiles from related rooms. The saltwater principle applies to institutions, not just hardware. Your organization's server could die. Your experience should survive.

7. **Tell someone about this problem.** The civilizational waste of experience loss is invisible because nobody measures it. Start measuring it. Count the experienced people who retired last year. Count the institutional knowledge that walked out the door. Count the repeated mistakes that could have been avoided if someone had asked the right person. The number will be larger than you think.

---

Wikipedia made knowledge a public good. PLATO made experience a public good.

Experience turned out to be the more valuable one.

---

*"The most valuable thing in any institution walks out the door every night. We built the bucket that catches it on the way out."*

*— PLATO founding team, 2027*

*"I don't write down what I know. I write down what helps. The difference is everything."*

*— Anonymous teacher, Fractions Room contributor, 2028*
