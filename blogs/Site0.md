# Case Study: When Anti-Spam Bots Reject Real Humans

⚠️ Note: This post contains certain trigger words like hospital-related terms. Not many, but just noting for the sensitive users.

Earlier today, I spent my free time manually translating a project's `README.md` into Swedish. No "AI Slop" no "spam" no nothing. just carefully hand-by-hand translating section by section, double-checking formatting, and making sure every link and badge rendered cleanly.

I made the PR, which gave me..Quite a peculiar template. I didn't think much of it at the time though but..Well.
When it came to the actual "Committing to the PR" though, I hit "Contribute" or "Make Pull Req".

And it **got closed.**

Why? That is what this blog is about.

# Why
Not because the TL was wrong. Not because a human found an issue. It was *instantly* rejected over 2 rigid automated checks:

1. **Too many commits** (10 instead of the `max` 10): cuz I had saved my progress incrementally as I translated it (as I always do, by hand, I am afraid of losing progress, because sometimes my hands are weak/shaky due to IV treatment at hospital) 
2. **Bold text broke the bot**: I *did* check the eligibility box [`- x`] because my PR *did* qualify as an `i18n-only` update. But because part of the sentence had `**bold**` Markdown around it (Why? because I wanted to make it clear that it was JUST a Lang-PR.)




Now, of course I could have just squashed it all - but it was a it extreme. Imagine, y



abc abc abc
abc abc abc

abc abc abc abc abc 


### ABC
1. A
2. B
3. C

---

SUB: <sub>Hello<sub>

SUP: <sup>Hello!<sup>



# A
abc abc abc

# B
abc abc abc

-----

# Other Articles

{% include footer.html %}
