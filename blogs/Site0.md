# Case Study: When Anti-Spam Bots Reject Real Humans

⚠️ Notes
- This post contains certain trigger words like hospital-related terms. Not many, but just noting for the sensitive users.
- You can see the [PR here](https://github.com/open-webui/open-webui/pull/34765)

Earlier today, I spent my free time manually translating a project's `README.md` into Swedish. No "AI Slop" no "spam" no nothing. just carefully hand-by-hand translating section by section, double-checking formatting, and making sure every link and badge rendered cleanly.

I made the PR, which gave me..Quite a peculiar template. I didn't think much of it at the time though but..Well.
When it came to the actual "Committing to the PR" though, I hit "Contribute" or "Make Pull Req".

And it **got closed.**

Why? That is what this blog is about.

# Why
Not because the TL was wrong. Not because a human found an issue. It was *instantly* rejected over 2 rigid automated checks:

1. **Too many commits** (10 instead of the `max` 5 or something): cuz I had saved my progress incrementally as I translated it (as I always do, by hand, I am afraid of losing progress, because sometimes my hands are weak/shaky due to IV treatment at hospital) 
2. **Bold text broke the bot**: I *did* check the eligibility box [`- x`] because my PR *did* qualify as an `i18n-only` update. But because part of the sentence had `**bold**` Markdown around it (Why? because I wanted to make it clear that it was JUST a Lang-PR.) Apparently? That was enough for breaking a the poor bots parser. And it accused me of leaving the box unchecked. And? **Closed the PR.**

I say one word: __Thank god it was just a small Readme, and not a huge Readme or something way huger.__

Now, of course I could have just squashed it all and re opened it but I was afraid it would close for another reason (It was never upfront that there was a bot like this - and, it was a huge wall of text anyway in their documentation, [try to read it!](https://docs.openwebui.com/contributing/#submit-code). For someone with sensitive eyes as myself(as per side effect of Remicade), it was even *painful to read*. I tried my best, though.)
So I tried to act in good faith but..Well. Apparently that wasn't enough.

---

## Visuals / Screenshots

<img width="332" height="544" alt="image" src="https://github.com/user-attachments/assets/19f3fca7-9708-42a8-b6ce-5750e79f2fbd" />

Note: this is not everything, and I zoomed out to show the sheer "dense-ness", there is no sections. No summary. It's just "read it all or go away" - or at least, that's the feeling I got.

## The irony of their "Accessibility reporting section"

<img width="762" height="106" alt="image" src="https://github.com/user-attachments/assets/a5117d97-3a5c-49fe-b628-2d97625df468" />

How on earth do I know a issue wont be closed just like my PR was?

---


# The real cost of doing this
I get why huge repos build stricter gatekeeper bots. But that's not the only way forward. Many other bots exists. This bot was so overzealous I got *stunned* and that's also why I had to write this blog, because..Honestly? I laughed when I saw the big picture It's all you can do to cope. I just feel bad for the many people who try to contribute to repos like these, just to get hit (maybe even months of work!) "CLOSED. please open a new pr fixing a tiny typo in your template-reply that nobody will read anyway when its merged". It's **NUTS**. to put it mildly.

**When a bot can't tell the difference between AI-spam("slop") and a human TL(made by hand) and immediately auto-closes instead of leaving a helpful note - it punishes (and selects to exclude) the exact people who actually care.**

This is what it does:
- It turns volunteering into a minefield. Suddenly you have to be perfect. 
- It creates accessibility barriers. Weak hands because of medication? Oh bad luck.
- It replaces humans welcome with cold rejection. A maintainer could have at least checked Merged it with one click on "Squash and merged" Instead no human ever even saw it. And I don't think they will. And I wont care if they don't. The bot solves the problems for them: No spam thanks, even if it costs rejecting actual humans.

## Connection To Evolutionary Biology
This is like natural selection. You are only welcome IFF(If And Only IF):
- Perfect in terms of no bad eyes/eyesight or shaky-hands(so you have to save each progress out of habit)
- You will happily without complaining<sup>(because otherwise it breaks the contributing_rules of "respectfulness" at their discretion)<sup> go trough "git-hoops" <sup>(which may or may not be worth it in the end!)<sup> like, perfect the PR template, perfect everything.



NOTE: each one of those if alone would not be a problem.
1. I could squash it if it meant I didn't need to worry to be slammed again with a "closed. because now it's this<..> that's missing"
2. I could fix the template PR if that's actually useful (and wont be closed because of another reason I wont be told)
3. If I actually keep doing this..I would end up with 10 Closed PRS. why? because each PR would get closed - and how do I know its worth it anyway?

# Reductio ad Absurdum
For people who know I am a fan of logical-fallacy-analysis:
Even running it trough Reductio ad Absurdum doesn't solve it: what if 11th PR stay open and the maintainer says "Actually I dont need this! Thanks anyway!" 🌷️ You can imagine how *flawed* this system is.
**Even the rare times it "works!"**


## Conclusion
Spam is a real problem. And the fact that AI cant be distinguished between real stuff is also a problem. And this happened to me actually, I took a daring approach to see how "bad/good" AI-Detection tools are. I am a cancer survivor, so I have a port-a-cath in a jar. I photod it. And I uploaded it. Guess what? **It was marked as `most likely AI`** which...to me I don't know what I thought at that time? imagine it for a second. AI Detection tools are so bad, one time I wrote a letter, and I told Gemini(`[!]`Which I actually personally like `[!]`) "was this letter written by an A.I?" and...Gemini said Yes.



## Key TakeAway
I still obviously use Gemini. Why? Because, AI's just like humans(like myself) can do wrong. It has happened I have also fallen into this "Judging by the cover". When something happens fast for example, of course I get the "wait-is this only blindly copied AI? Or did they actually write it by hand?" And this is why I'm so careful right now because, it gets harder and harder to see what's AI and what's not.


---
And of course, neither was AI—the photo was taken on my phone, and I typed the letter myself
Thank you for reading. ♥️ It means a lot. Please, I have one favor I'd like from you who read this:

You made it this far, spent your energy reading my ramblings, and so, please take care of yourself now and do something you *genuinely* enjoy. Thanks once more, Good night. 🌷️ <sub> janna <sub>

-----

# Other Articles

{% include footer.html %}
