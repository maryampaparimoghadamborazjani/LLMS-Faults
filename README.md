Faults in Large Language Models: A Critical Examination
Author: Maryam Paparimoghadamborazjani 

Contact: Maryam.Paparimoghadamborazjani@utexas.edu

Keywords: Large Language Models, AI limitations, hallucinations, bias in AI, ethical concerns, AI sustainability

Abstract
Large Language Models (LLMs) have significantly transformed natural language processing applications, from conversational agents to code generation. However, these systems exhibit substantial limitations. This paper examines their primary vulnerabilities: hallucinations, the propagation of biases from training data, the illusion of reasoning, ethical and security risks, and substantial environmental costs. Drawing on recent research, this review outlines the practical implications of these flaws and proposes mitigation strategies, advocating for a human-in-the-loop approach and treating LLMs as assistive tools rather than infallible systems.

1. Introduction
Foundational models such as GPT and LLaMA are trained on massive textual datasets, enabling them to generate highly coherent, human-like text. While effective for summarization and code generation, their underlying architectures harbor structural flaws. These are not merely superficial errors but inherent issues stemming from their training methodologies. The generation of false information or the echoing of societal prejudices can have severe consequences, particularly in high-stakes domains such as healthcare and criminal justice. This paper categorizes these challenges into five primary areas, discusses their real-world impact, and suggests pathways for more responsible development and deployment.

2. Hallucinations and Factual Inaccuracies
A well-documented limitation of LLMs is their tendency to "hallucinate"—generating highly confident but factually incorrect outputs. Because these models function essentially as probabilistic next-word predictors rather than fact-checking databases, they frequently fabricate dates, technical details, or historical events. Unlike human cognition, LLMs cannot verify their own claims without external integrations. This poses significant risks in critical fields like law and medicine. Recent research, such as the work by Farquhar et al. (2024), introduces "semantic entropy" to detect these errors by measuring the model's uncertainty at the level of meaning rather than specific phrasing [1]. While techniques like Retrieval-Augmented Generation (RAG) provide external grounding, they can be cumbersome and still struggle with outdated or conflicting information.

3. Inherent Biases and Fairness Issues
The outputs of LLMs are fundamentally constrained by their training data. Because these datasets often reflect historical human biases, stereotypes, and a predominantly Western, English-centric worldview, the models inevitably internalize and reproduce these prejudices. This can result in outputs that default to gendered assumptions about professions or perpetuate cultural clichés. In applications such as automated resume screening, these biases can lead to systemic discrimination against qualified candidates. While studies like Nyarko et al. (2024) demonstrate that targeted pruning and fine-tuning can mitigate bias in specific scenarios, there is no universal solution, complicating accountability [2]. Effective mitigation requires a combination of diversified training data, algorithmic fairness interventions, and continuous auditing.

4. Lack of True Comprehension and Reasoning
Despite their fluency, LLMs do not possess genuine comprehension or reasoning capabilities; their performance relies on sophisticated pattern matching. They can excel at familiar logical puzzles but frequently fail when presented with novel variations, demonstrating a lack of underlying causal understanding. Bender et al. (2021) famously characterized these models as "stochastic parrots," emphasizing that they synthesize language without grasping its meaning [3]. While prompting strategies like "Chain-of-Thought" (asking the model to evaluate step-by-step) can improve apparent logical flow, they do not simulate true cognition. Consequently, LLMs cannot be entirely relied upon for autonomous decision-making in complex moral or logical scenarios.

5. Ethical and Security Vulnerabilities
The proliferation of LLMs introduces significant ethical and security concerns, including the facilitated creation of deepfakes, misinformation, and plagiarized content. The "black box" nature of these models makes explainability difficult, undermining user trust. Furthermore, models trained on unvetted public data may inadvertently memorize and expose sensitive personal information. From a security perspective, LLMs are vulnerable to adversarial attacks, such as prompt injection and data poisoning, which can bypass safety guardrails. Li and Fung (2024) emphasize the need for robust, multi-layered defensive frameworks to counter these threats [4]. While legislative efforts like the EU AI Act aim to regulate deployment, technological advancements frequently outpace regulatory frameworks.

6. Environmental and Scalability Concerns
The computational resources required to train and deploy state-of-the-art LLMs have a profound environmental impact. Training large-scale models consumes massive amounts of electricity, resulting in carbon footprints comparable to commercial aviation. Furthermore, the trend toward increasingly larger parameter counts often yields diminishing returns in performance relative to the exponential increase in energy cost. Morrison et al. (2024) highlight that even mid-sized open-source models (e.g., 13B parameters) can emit 493 tons of CO₂, enough to power nearly 100 US homes for a year [5]. While open-source initiatives democratize access, they also multiply the number of models being trained. Addressing these concerns requires a shift toward more parameter-efficient architectures and sustainable hardware infrastructure.

7. Pathways Forward and Conclusion
To harness the capabilities of LLMs safely, the AI community must prioritize transparency, human-in-the-loop verification, and ethics-by-design principles. Users must adopt a critical approach to AI-generated content, while developers must focus on robustness and interpretability. In conclusion, the identified vulnerabilities—ranging from hallucinations and bias to environmental degradation—underscore that LLMs are powerful assistive tools, not autonomous authorities. By addressing these limitations directly, the field can maximize the utility of these models while mitigating their inherent risks.

References
S. Farquhar, J. Kossen, L. Kuhn, and Y. Gal, "Detecting hallucinations in large language models using semantic entropy," Nature, vol. 630, no. 8017, pp. 625-630, 2024.

J. Nyarko, D. E. Ho, E. Talley, M. Imai, and Y. Kim, "LLM Pruning and the Law," arXiv preprint arXiv:2407.00202, 2024.

E. M. Bender, T. Gebru, A. McMillan-Major, and S. Shmitchell, "On the Dangers of Stochastic Parrots: Can Language Models Be Too Big?," in Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency, pp. 610-623, 2021.

M. Q. Li and B. C. M. Fung, "A Survey on Ethical Hacking of Commercial Large Language Models," arXiv preprint arXiv:2409.06295, 2024.

J. Morrison, C. Na, J. Fernandez, T. Dettmers, E. Strubell, and J. Dodge, "Carbon Emissions in Open-Source AI Development," arXiv preprint arXiv:2410.05756, 2024.
