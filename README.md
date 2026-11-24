# book-talk

**A Claude skill that helps you have a proper conversation with your child about a book, one good question at a time.**

Most book chat with children ends at "What happened?" Asking a good *why* question at the right moment, and then the right follow-up, is hard to do on the spot. **book-talk** gets the book ready, plans the questions and coaches you through the conversation turn by turn. You ask the questions and your child does the thinking, while Claude keeps the conversation on track.

It grew out of several weeks of real book talks with a 9-year-old reader in Year 5, and it keeps what worked and drops what didn't.

---

## What it does

1. **Gets the book ready.** It builds a short brief: the characters, the key moments with chapter numbers, the author's notable choices, and questions with more than one good answer. For public-domain books it works from the full text, and for anything else it checks the facts with you first, because it **never makes up plot details**.
2. **Plans the talk along a fixed path.** Every talk asks the four questions from Adler and Van Doren's *How to Read a Book*, in order, and climbs a reading ladder one rung at a time: first the whole book, then the detail, then judging it, then comparing books. The next rung, not whatever went wrong last time, is the talk's focus. It plans two or three "bridge" questions that start from what your child already does well and lead up to that rung.
3. **Coaches you live.** Each turn gives you one question to read aloud, two hints ready in case your child gets stuck, and a note on what a good answer sounds like.
4. **Sums it up.** Afterwards you get a short summary: the step your child took towards the focus, where to pick up next time, what they needed help with, their own reading tips, words they didn't know, and two questions to ask again in a month.

## Two modes

| Mode | When | Length |
|---|---|---|
| **After the book** | Your child has just finished a book | 25–35 minutes, 8–10 questions (shorter for 7–8-year-olds) |
| **During reading** | Partway through a book, or a long or hard book | 5–10 minutes per chapter, 3–4 questions, with no spoilers |

## The four questions and the reading ladder

Every talk asks the four questions a good reader asks of any book, in this order (from *How to Read a Book*):

1. **What is the book about as a whole?**
2. **What does it say in detail, and how?**
3. **Is it true? Is it good?** Understand first, judge second.
4. **What of it?**

The ladder turns them into skills your child climbs one rung at a time:

| Floor | Rungs |
|---|---|
| 1 · The whole book | what kind of story · the whole book in three sentences · the big parts · the central problem |
| 2 · In detail | why characters act and change · cause and effect · the main idea with evidence from start and end · a line the book works hard on |
| 3 · Judging | what the book wanted you to feel · likes and dislikes, with the place in the book · would a real person do that? · standing your ground |
| 4 · Across books | two books on the same subject: how they differ |

Most of each talk goes to the next rung on your child's floor. A rung is secure when your child does it unaided in two of three talks; then the support comes off and the next rung opens. The summary after each talk shows where your child is on the ladder.

### The question bank: nine types

| # | Type | For example |
|---|---|---|
| 1 | First response and anything unclear | "Was there a part that puzzled you?" |
| 2 | Sum it up | "Tell me the story as if I were three years younger than you." |
| 3 | Characters: why and how they change | "How did Marilla change? Where does it start?" |
| 4 | One word | "What do you think *ruminated* means here? How did you work it out?" |
| 5 | One moment: picture it, then look at a word | "What do you see? Why that word and not a plainer one?" |
| 6 | The author's choices | "Why doesn't the author just tell us straight away?" |
| 7 | A stance question | "Was she right?" Then: "I'm going to argue the other side now…" |
| 8 | Connections: self, other books, the world | "…and where in the book did you see that?" |
| 9 | Close | "How did you work that out earlier?" |

## A coaching turn looks like this

```
Say:       Montgomery lets us know Marilla loves Anne long before Anne knows.
           How does she let us know?
If stuck:  1) Think of a time Marilla is cross with Anne. What does she do afterwards?
           2) Is there a moment where we hear what Marilla is thinking, but Anne doesn't?
Listen for: small actions or private thoughts that show love she won't say
```

You read the question out, then type in what your child said. Claude suggests the next move: a follow-up on their own words, a step towards the focus, the next hint, or the next question.

## The principles behind it

- **It's there to help, not to test.** Each talk climbs one rung. When your child says something good, Claude helps you take it one step further before moving on.
- **Don't spoil the first read.** Nothing to do while reading; after finishing, three sticky notes (where it turns, a favourite line, a puzzling bit) so the evidence is at hand.
- **One question at a time**, and follow what the child actually says, not the script.
- **Questions that need thinking, not memory.** Ask "Why does it matter that…?", not "What colour was…?"
- **A hint ladder, not lectures.** When Claude does give the answer, it shows the path: *clue + what we know → so…*
- **Clear the fog first.** If a child has lost the plot or a key word, tell them, then ask. You can't make inferences through fog.
- **Preview before you challenge.** "I'm going to argue the other side; your job is to stay standing if you still think so." Children hold their ground far better when they know it's coming.
- **"How did you work that out?"** Children's own answers to this become their reading tips.
- **Sharpen the word.** When a child says "it's more interesting" or "he was really angry", offer two or three nearby words and let them pick. That gives them words for exactly what they mean.
- **No jargon, no marks, no corrections.** It's meant to feel like a conversation, not a test.

## Install

**Claude Code**

```bash
git clone https://github.com/sonic1822/book-talk.git
cp -r book-talk/book-talk ~/.claude/skills/
```

**Claude.ai** (Pro, Max, Team or Enterprise, with code execution turned on)

1. Download `book-talk.zip` from Releases (the archive contains the `book-talk/` folder).
2. Go to **Settings → Capabilities** and upload it under Skills, then switch it on. Some accounts have this under **Features** instead.

Other tools that support Agent Skills can use the `book-talk/` folder as it is.

## Using it

Just ask:

- "Let's do a book talk. My son is 8 and has just finished *Charlotte's Web*."
- "My daughter's on chapter 6 of *The Secret Garden*. Can we do a during-reading check-in?"
- "Coach me in Chinese, please; the book is in English."

## The parent runs the talk

Claude's consumer terms require users to be 18 or over, so **the parent is the user and the child doesn't use the AI.** That's also the point: the conversation is between you and your child. Claude helps you prepare, and suggests what to say next.

## Privacy

Don't give Claude your child's full name, school or other identifying details. Keep the summaries on your own device. The skill doesn't store anything.

## Where it comes from

- Mortimer J. Adler and Charles Van Doren, *How to Read a Book* (revised edition, 1972): the four questions, the stages of reading a book (structure, interpretation, criticism) and comparing books. The rungs, the mastery rule and the sticky notes are this skill's adaptation for children.
- Aidan Chambers, *Tell Me: Children, Reading and Talk*: the "likes, dislikes, puzzles, patterns" opening
- Isabel Beck, Margaret McKeown et al., *Questioning the Author*: making the author visible
- Ellin Keene and Susan Zimmermann, *Mosaic of Thought*: text-to-self, text-to-text and text-to-world connections
- The reading skills tested at Key Stage 2 in England, used to check that the question types cover the ground
- Socratic tutoring skills such as Jellypod's `socratic-tutor` and `malkreide/socratic-method-skill`, both MIT-licensed, which inspired the hint ladder, although no text has been copied from them.

## Licence

Released under the MIT licence, with the full text in [LICENSE](LICENSE).
