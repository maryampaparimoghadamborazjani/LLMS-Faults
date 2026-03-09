# Faults in Large Language Models: A Critical Examination
**Author:** Maryam Paparimoghadamborazjani (Mary Pa)  
**Contact:** Maryam.Paparimoghadamborazjani@utexas.edu  
*Keywords: Large Language Models, AI limitations, hallucinations, bias in AI, ethical concerns, AI sustainability*

## Abstract
We've seen large language models burst onto the scene, transforming how we handle text, from chatbots to code helpers. But honestly speaking, they're not perfect. Far from it. This paper digs into their main weaknesses: making stuff up, carrying over biases from dodgy data, faking deep thinking, opening doors to ethical messes, and guzzling resources like there's no tomorrow. Pulling from fresh studies, I lay out what this means in practice and toss out some ideas for fixing things. Bottom line: treat these models as handy sidekicks, not all-knowing gurus, and push for smarter, human-in-the-loop setups.

## 1. Introduction
Think about it—models like GPT or Llama get fed mountains of text from the web and books, then spit out responses that sound eerily human. They're great for quick summaries or brainstorming code, but peel back the layers, and you find errors everywhere. These aren't just minor glitches; they're baked-in problems from how they're built and trained. 

*(Tip: You can drag and drop a diagram of how LLMs process data right here in the GitHub editor to make the page more visually engaging and instructive for readers.)*

Stuff like spitting out false info or echoing real-world prejudices can cause real trouble, especially in fields like medicine or justice where accuracy matters. Here, I break it down into five big issues, talk about the fallout, and suggest ways forward. This isn't just academic nitpicking—it's about guiding folks building and using this tech to do it right.

## 2. Hallucinations and Factual Inaccuracies
Ever ask an AI a question and get a super confident answer that's totally wrong? That's hallucinations for you. These models aren't fact-checkers; they're just guessing the next word based on stats from their training. So, they might mess up a date in history or make up details about some tech gadget. Humans double-check with books or memory, but LLMs? Not unless you bolt on extra tools.

This bites hard in serious spots—like giving bad legal tips or sketchy health advice. A team including Farquhar and others (2024) came up with this "semantic entropy" trick to spot these slip-ups by measuring how unsure the model is about meanings, not just words [1]. Stuff like adding real-time data pulls (RAG) helps, but it's clunky and still trips on old info.

## 3. Inherent Biases and Fairness Issues
Not a big surprise: garbage in, garbage out. Training data's full of human biases—think stereotypes about jobs or cultures—and models soak it up. They might default to "doctor" as male or churn out clichéd takes on minorities. It's not the AI being mean; it's mirroring our messy world, where English and Western views dominate the data.

The ripple effects? In job screening apps, it could skip over qualified folks based on word choices. Nyarko and crew (2025) showed you can trim biases in specific scenarios, but it's no magic fix-all, and it muddies who to blame when things go wrong [2]. Fixes? Mix up the data more, tweak with anti-bias training, and keep checking. But "fair" is tricky—what's neutral to one person isn't to another.

## 4. Lack of True Comprehension and Reasoning
These things act smart, but it's all smoke and mirrors—pattern-matching, not real views. They nail puzzles they've seen before but choke on twists. No grasp of why things happen, or feelings, or tricky contexts.

Creative stuff comes out flat: poems that rhyme but say nothing deep. On tough logic or morals, they fake it with shortcuts. Bender, Gebru, and team (2021) nailed it calling them "stochastic parrots"—just parroting data without getting the point [3]. Prompts that make them "think step by step" improve things a bit, but don't kid yourself; it's not true smarts. We can't lean on them too hard for teaching or big decisions.

## 5. Ethical and Security Vulnerabilities
On the dark side, LLMs make it easy to pump out fakes—deepfakes, lies for clicks, or ripped-off writing. They're black boxes, so figuring out why they say something is a headache, killing trust. And privacy? They train on our data without asking, sometimes spitting back personal bits.

Hack-wise, sneaky prompts can make them spill secrets or act out. Li and Fung (2025) rounded up threats like breaking safeguards or poisoning data, calling for layered protections [4]. Laws like the EU's AI rules are trying to rein it in, but tech moves faster than regs.

## 6. Environmental and Scalability Concerns
Training one of these beasts burns power like a small city. Carbon-wise, it's like jetting across oceans, adding to the climate mess. And bigger isn't always better—pumping up size gives tiny boosts for huge costs.

Morrison et al. (2025) crunched numbers: a mid-size model (13B params) spews 493 tons of CO2, enough to run nearly 100 US homes for a year [5]. Open-source helps spread access, but it also lets loose half-baked versions. Go greener with smarter designs and efficient hardware.

## 7. Pathways Forward and Conclusion
Look, LLMs can change the game if we handle them smartly. Mix in human checks, open up how they act, and build ethics in from the start to cut risks. Users: always verify. Builders: focus on toughening them up. Everyone: push for rules that stick.

Wrapping up, these flaws—from made-up facts to biases, fake depth, shady ethics, and eco-hits—show LLMs as boosters for our brains, not stand-ins. Tackle them straight on, and we unlock the good without the grief.

## References
1. S. Farquhar, J. Kossen, L. Kuhn, and Y. Gal, "Detecting hallucinations in large language models using semantic entropy," *Nature*, vol. 630, no. 8017, pp. 625-630, 2024.
2. J. Nyarko, D. E. Ho, E. Talley, M. Imai, and Y. Kim, "LLM Pruning and the Law," *arXiv preprint arXiv:2407.00202*, 2025.
3. E. M. Bender, T. Gebru, A. McMillan-Major, and S. Shmitchell, "On the Dangers of Stochastic Parrots: Can Language Models Be Too Big?," in *Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency*, pp. 610-623, 2021.
4. M. Q. Li and B. C. M. Fung, "A Survey on Ethical Hacking of Commercial Large Language Models," *arXiv preprint arXiv:2409.06295*, 2025.
5. J. Morrison, C. Na, J. Fernandez, T. Dettmers, E. Strubell, and J. Dodge, "Carbon Emissions in Open-Source AI Development," *arXiv preprint arXiv:2410.05756*, 2025.
