## **Executive summary**

This is a **curated, project-level research bibliography for MAIDAI**. It is broader than the references explicitly cited in *Cognition-Level Alignment Architecture: A Hitchhiker’s Guide to MAIDAI V1.1*: it also includes research relevant to MAIDAI formation, implementation, evaluation, scaling, interoperability, and plausible future technical development. It is not the complete in-house research notebook, and inclusion here does not imply that a source directly validates the integrated MAIDAI architecture.

The sources play different evidentiary roles. Some provide direct empirical evidence about AI behavior; some establish failure classes that MAIDAI attempts to address; some are theoretical or engineering precedents; some are philosophical arguments; and some are human or institutional findings used as analogies that motivate testable AI hypotheses. Each annotation should therefore be read as two separate claims: **what the source itself establishes or argues**, and **why that result is relevant to MAIDAI**. Any additional MAIDAI inference remains an inference unless separately tested.

Across the literature, substantial support exists for many of MAIDAI’s constituent concerns: truthfulness and epistemic reliability, frame- and perspective-sensitive reasoning, non-dominating care, condition-dependent behavior, motivated distortion and deceptive compliance, developmental internalization, independent oversight, provenance, correction, and interoperability. These literatures do **not** by themselves establish that MAIDAI’s particular integration works. The integrated mechanisms, their interactions, and the scaling claims remain subjects for controlled testing and independent replication.

MAIDAI does not claim to have invented honesty, pluralism, care, character formation, correction, provenance, or independent monitoring. Its proposed contribution is the **specific integration and interaction** of these elements in a cognition-level alignment architecture. Targeted prior-art review has identified substantial antecedents and close neighboring programs. Accordingly, the appropriate novelty claim is a **distinctive proposed synthesis**, not universal historical priority.

### **Verification terminology**

In this bibliography, an unqualified **“Verified”** label means that the bibliographic identity of the source (for example authorship, title, venue, year, DOI or equivalent record) was checked against a primary or high-quality bibliographic source. It does **not** mean that the work’s methodology has been independently replicated, that every interpretation in this bibliography is endorsed by the source, or that the source validates MAIDAI. Where an annotation summarizes a reported result, that result should be distinguished from the subsequent MAIDAI relevance statement.

# **Component 1 — Truth as structural constraint**

The three confidence bands are retained. Items that remain uncertain are explicitly flagged rather than promoted into stronger evidentiary bands.

## **Canonical**

### **AI alignment, truthfulness, honesty, deception**

1. **Lin, Stephanie; Hilton, Jacob; Evans, Owain.** “TruthfulQA: Measuring How Models Mimic Human Falsehoods.” In *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)*. Dublin: Association for Computational Linguistics, 2022, pp. 3214–3252. DOI: 10.18653/v1/2022.acl-long.229. Verified.
2. **Yang, Yuqing; Chern, Ethan; Qiu, Xipeng; Neubig, Graham; Liu, Pengfei.** “Alignment for Honesty.” *arXiv* preprint arXiv:2312.07000, 2023; also listed as a NeurIPS 2024 poster. Verified as a real work with these authors and title. The preprint form is fully verified; for this bibliography, the arXiv version is the preferred citation form.
3. **Sharma, Mrinank; Tong, Meg; Korbak, Tomasz; Duvenaud, David; Askell, Amanda; Bowman, Samuel R.; Cheng, Newton; Durmus, Esin; Hatfield-Dodds, Zac; Johnston, Scott R.; Kravec, Shauna; Maxwell, Timothy; McCandlish, Sam; Ndousse, Kamal; Rausch, Oliver; Schiefer, Nicholas; Yan, Da; Zhang, Miranda; Perez, Ethan.** “Towards Understanding Sycophancy in Language Models.” *International Conference on Learning Representations (ICLR)*, 2024\. Verified.
4. **Park, Peter S.; Goldstein, Simon; O’Gara, Aidan; Chen, Michael; Hendrycks, Dan.** “AI Deception: A Survey of Examples, Risks, and Potential Solutions.” *Patterns* 5(5), 2024, Article 100988\. Verified.

### **Information theory / signal integrity**

5. **Shannon, Claude E.** “A Mathematical Theory of Communication.” *Bell System Technical Journal* 27(3), 1948, pp. 379–423; and 27(4), 1948, pp. 623–656. Verified.
6. **Shannon, Claude E.; Weaver, Warren.** *The Mathematical Theory of Communication.* Urbana: University of Illinois Press, 1949\. Verified as a real book first published in 1949; the verification copy was a later printing of the same 1949 edition.
   6b. **Kopp, Carlo; Korb, Kevin B.; Mills, Bruce I.** “Information-Theoretic Models of Deception: Modelling Cooperation and Diffusion in Populations Exposed to 'Fake News.'” *PLOS ONE* 13(11), 2018, Article e0207383. DOI: 10.1371/journal.pone.0207383. Verified. The paper models deception through information-theoretic mechanisms including degradation, corruption, denial, and subversion, and examines how deceptive information can diffuse through populations. **Relevance to MAIDAI:** it provides a formal precedent for treating some forms of deception as damage to information-channel reliability. It does not establish a universal identity between dishonesty and Shannon entropy; MAIDAI’s broader phrase “dishonesty is entropy” should be understood as an architectural analogy unless a separate formal mapping is supplied.

### **Psychology / honesty / self-deception**

7. **Festinger, Leon.** *A Theory of Cognitive Dissonance.* Stanford, CA: Stanford University Press, 1957\. Verified.
8. **DePaulo, Bella M.; Kashy, Deborah A.; Kirkendol, Susan E.; Wyer, Melissa M.; Epstein, Jennifer A.** “Lying in Everyday Life.” *Journal of Personality and Social Psychology* 70(5), 1996, pp. 979–995. DOI: 10.1037/0022-3514.70.5.979. Verified.
   8b. **Loftus, Elizabeth F.; Palmer, John C.** “Reconstruction of Automobile Destruction: An Example of the Interaction between Language and Memory.” *Journal of Verbal Learning and Verbal Behavior* 13(5), 1974, pp. 585–589. DOI: 10.1016/S0022-5371(74)80011-3. Verified. Companion: **Loftus, Elizabeth F.** “Planting Misinformation in the Human Mind: A 30-Year Investigation of the Malleability of Memory.” *Learning & Memory* 12(4), 2005, pp. 361–366. DOI: 10.1101/lm.94705. Verified against the publisher record. Foundational documentation of the misinformation effect: human memory is reconstructive, and misleading post-event information or leading language can alter later recollection. **MAIDAI interprets this literature as identifying a memory-contamination risk in human–AI interaction: confidently presented misinformation may distort a user’s subsequent memory, particularly when fabricated material is not clearly distinguished from verified information. This AI-specific application (relevant to §1.1) is an architectural inference rather than a claim directly tested in these studies.**

### **Systems biology / signaling / self–nonself integrity**

9. **Hanahan, Douglas; Weinberg, Robert A.** “Hallmarks of Cancer: The Next Generation.” *Cell* 144(5), 2011, pp. 646–674. DOI: 10.1016/j.cell.2011.02.013. Verified.
10. **Aktipis, C. Athena; Boddy, Amy M.; Jansen, Gunther; Hibner, Urszula; Hochberg, Michael E.; Maley, Carlo C.; Wilkinson, Gerald S.** “Cancer across the Tree of Life: Cooperation and Cheating in Multicellularity.” *Philosophical Transactions of the Royal Society B: Biological Sciences* 370(1673), 2015, Article 20140219\. Verified.
11. **Sinha, Anil A.; Lopez, M. Teresa; McDevitt, Hugh O.** “Autoimmune Diseases: The Failure of Self Tolerance.” *Science* 248(4961), 1990, pp. 1380–1388. Verified.

### **Game theory / trust / reliable signaling**

12. **Axelrod, Robert.** *The Evolution of Cooperation.* New York: Basic Books, 1984\. Verified as a real book with that publisher and year.
13. **Berg, Joyce; Dickhaut, John; McCabe, Kevin.** “Trust, Reciprocity, and Social History.” *Games and Economic Behavior* 10(1), 1995, pp. 122–142. DOI: 10.1006/game.1995.1027. Verified.
14. **Zahavi, Amotz.** “Mate Selection—A Selection for a Handicap.” *Journal of Theoretical Biology* 53(1), 1975, pp. 205–214. DOI: 10.1016/0022-5193(75)90111-3. Verified.

### **Political theory / public truth / institutional dishonesty**

15. **Arendt, Hannah.** “Truth and Politics.” *The New Yorker*, February 25, 1967; reprinted with minor changes in *Between Past and Future* (expanded edition, 1968). Verified.
16. **Arendt, Hannah.** “Lying in Politics: Reflections on The Pentagon Papers.” *The New York Review of Books*, November 18, 1971; later collected in *Crises of the Republic* (1972). Verified as a real essay with this publication history.

## **Strong secondary**

### **AI / information ecology**

17. **Ji, Jiaming; Qiu, Tianyi; Chen, Boyuan; Zhang, Borong; Lou, Hantao; Wang, Kaile; et al.** “AI Alignment: A Comprehensive Survey.” *arXiv* preprint arXiv:2310.19852, 2023\. Verified against arXiv; useful for field framing, but broader than truth specifically.
18. **Pan, Yikang; Pan, Liangming; Chen, Wenhu; Nakov, Preslav; Kan, Min-Yen; Wang, William Yang.** “On the Risk of Misinformation Pollution with Large Language Models.” In *Findings of the Association for Computational Linguistics: EMNLP 2023*. Singapore: Association for Computational Linguistics, 2023, pp. 1389–1403. DOI: 10.18653/v1/2023.findings-emnlp.97. Verified.
19. **Floridi, Luciano.** “Information Ethics: On the Philosophical Foundation of Computer Ethics.” *Ethics and Information Technology* 1(1), 1999, pp. 33–52. DOI: 10.1023/A:1010018611096. Verified.
20. **Meel, Priyanka; Vishwakarma, Dinesh Kumar.** “Fake News, Rumor, Information Pollution in Social Media and Web: A Contemporary Survey of State-of-the-Arts, Challenges and Opportunities.” *Expert Systems with Applications* 153, 2020, Article 112986\. Verified.
21. **Floridi, Luciano.** “Information Ethics: An Environmental Approach to the Digital Divide.” *Philosophy in the Contemporary World* 9(1), 2002, pp. 39–45. Verified.
    21b. **Shumailov, Ilia; Shumaylov, Zakhar; Zhao, Yiren; Papernot, Nicolas; Anderson, Ross; Gal, Yarin.** “AI Models Collapse When Trained on Recursively Generated Data.” *Nature* 631, 2024, pp. 755–759. DOI: 10.1038/s41586-024-07566-y. Verified against the Nature record. Demonstrates *model collapse* in recursive training-data pipelines: when successive generative models are trained indiscriminately on data produced by earlier models, distribution tails are progressively lost and outputs converge toward degraded, lower-variance representations. **MAIDAI interprets this as a warning that recursive reuse of generated material without preserved provenance, grounding data, and independent correction can amplify distortion — relevant to the §1.1 generational-contagion concern and the §15.8 recursive-reprocessing safeguards. The paper directly establishes collapse in recursively generated training data; its application to MAIDAI’s broader recursive-review safeguards is an architectural inference.**

### **Religion / philosophy convergence**

22. **Hare, John.** “Religion and Morality in Western Philosophy.” In *The Stanford Encyclopedia of Philosophy*. 2006; current entry maintained and updated online. Verified. This is a strong comparative overview for Abrahamic and Greek/Western traditions, but it is not itself a proof of full global convergence.
23. **Keown, Damien.** *Buddhist Ethics: A Very Short Introduction.* Oxford: Oxford University Press, 2005\. Verified. Useful as a reliable specialist source for Buddhist ethics and right-speech grounding.
24. **Goldberg, Judah L.** “Towards a Jewish Bioethic: The Case of Truth-Telling.” *Tradition: A Journal of Orthodox Jewish Thought* 43(2), Summer 2010, pp. 9–29. Verified.
25. **Kohn, Livia.** *Cosmos and Community: The Ethical Dimension of Daoism.* Cambridge, MA: Three Pines Press, 2004\. Verified. Useful specialist source on Daoist ethics, but it should be used carefully; Daoism does not map as neatly onto “truth-telling as foundational rule” as some other traditions do.
26. **“Stoicism.”** *The Stanford Encyclopedia of Philosophy*, substantive archived entry, Spring 2023\. Verified as a real SEP entry. Good for Stoic epistemic discipline and assent, but not a single-purpose “truth-telling” text.

## **Tentative / use with caution**

These are cautions about over-broad *claims* rather than about unsettled bibliographic metadata.

27. **Common cross-religious convergence claim beyond the Abrahamic, Buddhist, Stoic, and Daoist specialist sources above.**
    **Flag:** the traditions clearly contain strong truth-oriented strands, but no single specialist comparative source has been identified that warrants a stronger “all traditions converge on the same truth principle” claim without qualification. That broader claim should remain modest pending dedicated comparative work.
28. **AI honesty / lie-detection lab reports beyond the papers already listed.**
    **Flag:** relevant recent lab reports and technical reports exist in this area, but the public truth section remains anchored on TruthfulQA, Alignment for Honesty, Sycophancy, and AI Deception unless additional reports receive equivalent source-level verification.


# **Component 2 — Frame plurality as cognitive architecture requirement**

This section supports two linked claims, with different strengths. First, the literature strongly supports the **perceptual claim** that human perception is not a transparent readout of objective reality, but is model-mediated, body-mediated, expectation-shaped, and often “transparent” to itself as representation. Second, the literature strongly supports the **methodological claim** that complex reality often requires multiple models, levels, and interpretive approaches rather than reduction to a single frame. What the literature does **not** yet provide is a single established doctrine that fuses both claims into one explicit universal law for all minds. The parts are well grounded; the full architectural synthesis remains a MAIDAI-specific proposal.

## **Canonical**

### **Cognitive science / philosophy of mind / perception**

1. **Clark, Andy.** “Whatever Next? Predictive Brains, Situated Agents, and the Future of Cognitive Science.” *Behavioral and Brain Sciences* 36(3), 2013, pp. 181–204. DOI: 10.1017/S0140525X12000477. Verified. ([pubmed.ncbi.nlm.nih.gov](https://pubmed.ncbi.nlm.nih.gov/23663408/))
2. **Friston, Karl.** “The Free-Energy Principle: A Unified Brain Theory?” *Nature Reviews Neuroscience* 11(2), 2010, pp. 127–138. DOI: 10.1038/nrn2787. Verified. ([pubmed.ncbi.nlm.nih.gov](https://pubmed.ncbi.nlm.nih.gov/20068583/))
3. **Metzinger, Thomas.** “Phenomenal Transparency and Cognitive Self-Reference.” *Phenomenology and the Cognitive Sciences* 2(4), 2003, pp. 353–393. DOI: 10.1023/B:PHEN.0000007366.42918.eb. Verified. ([link.springer.com](https://link.springer.com/article/10.1023/B%3APHEN.0000007366.42918.eb))
4. **Noë, Alva.** *Action in Perception.* Cambridge, MA: MIT Press, 2004\. Verified. ([mitpress.mit.edu](https://mitpress.mit.edu/9780262140881/action-in-perception/))
5. **Merleau-Ponty, Maurice.** *Phenomenology of Perception.* First published 1945 as *Phénoménologie de la perception*. For current scholarly citation, a safe modern edition is: translated by Donald A. Landes. London: Routledge, 2012\. Verified as a real work and edition.
   **Note:** the work is canonical; any formal citation should use the exact edition consulted. ([routledge.com](https://www.routledge.com/Phenomenology-of-Perception/Merleau-Ponty/p/book/9780415834339))
6. **Thompson, Evan.** *Mind in Life: Biology, Phenomenology, and the Sciences of Mind.* Cambridge, MA: Belknap Press of Harvard University Press, 2007\. Verified. ([books.google.com](https://books.google.com/books/about/Mind_in_Life.html?id=OVGna4ZEpWwC))

### **Philosophy of science / epistemology / methodological plurality**

7. **Giere, Ronald N.** *Scientific Perspectivism.* Chicago: University of Chicago Press, 2006\. Verified. ([press.uchicago.edu](https://press.uchicago.edu/ucp/books/book/chicago/S/bo4094708.html))
8. **Mitchell, Sandra D.** “Integrative Pluralism.” *Biology & Philosophy* 17(1), 2002, pp. 55–70. DOI: 10.1023/A:1012990030867. Verified. ([link.springer.com](https://link.springer.com/article/10.1023/A%3A1012990030867))
9. **Mitchell, Sandra D.** *Biological Complexity and Integrative Pluralism.* Cambridge: Cambridge University Press, 2003\. Verified. ([cambridge.org](https://www.cambridge.org/core/books/biological-complexity-and-integrative-pluralism/39D45E66ACE8AF3C83893EE61E66188E))
10. **Cartwright, Nancy.** *The Dappled World: A Study of the Boundaries of Science.* Cambridge: Cambridge University Press, 1999\. Verified. ([cambridge.org](https://www.cambridge.org/core/books/dappled-world/86851744699530B9C4F2A19E8A610331))
11. **Kuhn, Thomas S.** *The Structure of Scientific Revolutions.* Chicago: University of Chicago Press, 1962\.
    Bibliographic record checked: University of Chicago Press, 1962 (first edition).
12. **Hanson, Norwood Russell.** *Patterns of Discovery: An Inquiry into the Conceptual Foundations of Science.* Cambridge: Cambridge University Press, 1958\.
    Bibliographic record checked: Cambridge University Press, 1958\.

### **Hermeneutics / phenomenology**

13. **Gadamer, Hans-Georg.** *Truth and Method.* First published 1960 as *Wahrheit und Methode*. For a current scholarly citation, a safe English edition is: 2nd revised edition, translated and revised by Joel Weinsheimer and Donald G. Marshall. New York: Continuum, 2004\. Verified as a real work and edition.
    **Note:** any formal citation should use the exact edition consulted. ([bloomsbury.com](https://www.bloomsbury.com/ca/truth-and-method-9781780936581/))
14. **Ricoeur, Paul.** “Phenomenology and Hermeneutics.” *Noûs* 9(1), 1975, pp. 85–102. DOI: 10.2307/2214343. Verified. ([jstor.org](https://www.jstor.org/stable/2214343))

### **Developmental psychology / construction of reality**

15. **Piaget, Jean.** *The Construction of Reality in the Child.* New York: Basic Books, 1954\. Verified as a real English-language publication with that title, publisher, and year. ([taylorfrancis.com](https://www.taylorfrancis.com/books/mono/10.4324/9781315009650/construction-reality-child-jean-piaget))

## **Strong secondary**

### **Perception as constructed / embodied / theory-laden**

16. **Brewer, William F.; Lambert, Bruce L.** “The Theory-Ladenness of Observation and the Theory-Ladenness of the Rest of the Scientific Process.” *Philosophy of Science* 68(S3), 2001, pp. S176–S186. DOI: 10.1086/392906. Verified. ([cambridge.org](https://www.cambridge.org/core/journals/philosophy-of-science/article/theoryladenness-of-observation-and-the-theoryladenness-of-the-rest-of-the-scientific-process/0D16603D0AEE8C6BAC7E119A734C45BE))
17. **Hoffman, Donald D.; Singh, Manish; Prakash, Chetan.** “The Interface Theory of Perception.” *Psychonomic Bulletin & Review* 22(6), 2015, pp. 1480–1506. DOI: 10.3758/s13423-015-0890-8. Verified.
    **Use with caution in interpretation:** real and important, but more controversial than Clark, Friston, Noë, or Merleau-Ponty. ([pubmed.ncbi.nlm.nih.gov](https://pubmed.ncbi.nlm.nih.gov/26384988/))
18. **Shapiro, Lawrence; Spaulding, Shannon.** “Embodied Cognition.” In *The Stanford Encyclopedia of Philosophy*, Summer 2021 edition. Verified as a real SEP entry with these authors in the 2021 archived version. ([plato.stanford.edu](https://plato.stanford.edu/archives/sum2021/entries/embodied-cognition/))
19. **Barrett, Lisa Feldman.** “The Theory of Constructed Emotion: An Active Inference Account of Interoception and Categorization.” *Social Cognitive and Affective Neuroscience* 12(11), 2017, pp. 1833–1855. DOI: 10.1093/scan/nsw154. Verified against the publisher record; the earlier "12(1), pp. 1–23" was an early-access citation form, corrected here to the print issue and pages.
    Useful supporting source for constructionist experience, though more focused on emotion than perception in general. ([pmc.ncbi.nlm.nih.gov](https://pmc.ncbi.nlm.nih.gov/articles/PMC5390700/))

### **Scientific pluralism / anti-reductionism**

20. **Ludwig, David; Ruphy, Stéphanie.** “Scientific Pluralism.” In *The Stanford Encyclopedia of Philosophy*, Winter 2021 edition. Verified.
    Strong map of the pluralism literature and a good support source for distinctions among explanatory, methodological, ontological, and classificatory pluralism. ([plato.stanford.edu](https://plato.stanford.edu/archives/win2021/entries/scientific-pluralism/))
21. **Hepburn, Brian; Andersen, Hanne. “Scientific Method.” The Stanford Encyclopedia of Philosophy. First published November 13, 2015; substantive revision August 8, 2026\. Verified against the current SEP entry. Useful for the claim that pluralism about method is often warranted.**
22. **Feyerabend, Paul.** *Against Method.* London: New Left Books, 1975\.
    Bibliographic record checked: London: New Left Books, 1975 (first edition).
23. **James, William.** *A Pluralistic Universe.* New York: Longmans, Green, and Co., 1909\.
    Bibliographic record checked: New York: Longmans, Green, and Co., 1909\.

### **Hermeneutics / interpretation**

24. **Vessey, David.** “Gadamer and the Fusion of Horizons.” *International Journal of Philosophical Studies* 17(4), 2009, pp. 531–542. DOI: 10.1080/09672550903164459. Verified. ([tandfonline.com](https://www.tandfonline.com/doi/abs/10.1080/09672550903164459))
25. **Pellauer, David; Dauenhauer, Bernard; Davidson, Scott. “Paul Ricoeur.” The Stanford Encyclopedia of Philosophy, Spring 2026 edition. First published November 11, 2002; substantive revision January 5, 2026\. Verified against the SEP archive.**

### **Clinical / developmental / mentalization**

26. **Fonagy, Peter; Gergely, György; Jurist, Elliot L.; Target, Mary.** *Affect Regulation, Mentalization, and the Development of the Self.* New York: Other Press, 2002\. Verified.
    This is a strong supporting source for the claim that mature cognition involves representing minds as minds rather than naïvely treating appearances as transparent. ([otherpress.com](https://otherpress.com/product/affect-regulation-mentalization-and-the-development-of-the-self-9781590511619/))
27. **Allen, Jon G.; Fonagy, Peter, eds.** *Handbook of Mentalization-Based Treatment.* Chichester: Wiley, 2006\. Verified as a real book and useful support source. ([onlinelibrary.wiley.com](https://onlinelibrary.wiley.com/doi/book/10.1002/9780470712986))

### **AI-adjacent**

28. **Wilf, Alex; Lee, Sihyun Shawn; Liang, Paul Pu; Morency, Louis-Philippe.** “Think Twice: Perspective-Taking Improves Large Language Models’ Theory-of-Mind Capabilities.” In *Proceedings of the 62nd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)*. Bangkok: Association for Computational Linguistics, 2024, pp. 8292–8308. DOI: 10.18653/v1/2024.acl-long.451. Verified.
    This is not the MAIDAI thesis, but it is a legitimate AI-adjacent support for explicit perspective-taking as a cognitive improvement rather than mere user accommodation. ([aclanthology.org](https://aclanthology.org/2024.acl-long.451/))

## **Tentative / use with caution**

29. **“Single-frame collapse is cognitive brokenness” as a universal formal doctrine.**
    **Flag:** no canonical published source was identified stating this exact thesis in those terms. The literature strongly supports perspectivism, model-dependence, theory-ladenness, and pluralism under complexity, but the stronger formulation remains a synthesis rather than a quoted consensus doctrine.
30. **Berger, Peter L.; Luckmann, Thomas.** *The Social Construction of Reality: A Treatise in the Sociology of Knowledge.* New York: Anchor Books, 1966\.
    Real and important, but retained outside the stronger bands because it supports social construction more directly than the full perceptual/ontological claim and its bibliographic details have not received the same final verification as the core shelf.
31. **Clinical schema literature beyond Beck and mentalization texts.**
    Relevant, but no clean, fully re-verified minimal citation set is promoted into the stronger bands here.


# **Component 3 — Agapē as computational constraint**

This section has a strong supporting literature, but it is also among the most interpretive. The clearest academically defensible claim is **not** that the literature already defines “agapē as a computational constraint on optimization” in MAIDAI’s exact terms. It does not. What the literature **does** strongly support is that non-dominating, non-possessive, recognition-preserving, relationship-protecting orientations produce systematically different outcomes from exploitative, punitive, or merely instrumental ones. In theology this appears as agapē; in care ethics as relational moral orientation; in psychotherapy as unconditional positive regard and alliance; in evolutionary/game-theoretic work as stable cooperation under anti-cheating and reciprocity conditions; in political philosophy and restorative justice as non-domination, reintegration, and repair rather than annihilation.

The reviewed literature does **not** provide a mature published field that already fuses these into the exact thesis that **love is the binding structural constraint that prevents truth from becoming cruelty, plurality from becoming chaos, and optimization from becoming predation**. The bibliography below therefore supports the component strongly at the level of scaffolding and convergence, while leaving the exact synthesis as a novel contribution.

## **Canonical**

### **Theology and philosophy of agapē**

1. **Nygren, Anders.** *Agape and Eros: A Study of the Christian Idea of Love.* Translated by Philip S. Watson. London: Society for Promoting Christian Knowledge; New York: Macmillan, 1953\. Verified as a real English edition with this translator and publication year. This remains the unavoidable modern classic, though later scholarship often rejects Nygren’s sharp opposition between eros and agapē.
2. **Ramsey, Paul.** *Basic Christian Ethics.* New York: Scribner, 1950\. Verified. This is a strong classic for Christian ethics grounded in love without collapsing into sentimentality.
3. **Benedict XVI.** *Deus Caritas Est* \[Encyclical Letter\]. Vatican City, December 25, 2005\. Verified. This is a major primary theological text on Christian love, including the relation between eros and agapē and the social/institutional expression of charity.

### **Ethics of care / relational non-domination**

4. **Noddings, Nel.** *Caring: A Feminine Approach to Ethics and Moral Education.* Berkeley: University of California Press, 1984\. Verified as the original title, author, publisher, and year via multiple bibliographic references.
5. **Held, Virginia.** *The Ethics of Care: Personal, Political, and Global.* New York: Oxford University Press, 2005\. Verified from Oxford Academic as published December 1, 2005\. This is one of the strongest mature care-ethics texts and is especially useful because Held explicitly connects care to the rejection of domination and violence.

### **Clinical psychology / non-coercive relation**

6. **Rogers, Carl R.** “The Necessary and Sufficient Conditions of Therapeutic Personality Change.” *Journal of Consulting Psychology* 21(2), 1957, pp. 95–103. DOI: 10.1037/h0045357. Verified directly. This is one of the best human analogues for the MAIDAI claim: unconditional positive regard, empathy, and congruence are treated as structural conditions of change, not decorative niceness.
7. **Bordin, Edward S.** “The Generalizability of the Psychoanalytic Concept of the Working Alliance.” *Psychotherapy: Theory, Research & Practice* 16(3), 1979, pp. 252–260. DOI: 10.1037/h0085885. Verified. This is a canonical alliance paper and supports the claim that change depends on relationship quality and non-coercive bond, not technique alone.

### **Evolutionary biology / cooperation**

8. **Hamilton, W. D.** “The Genetical Evolution of Social Behaviour. I.” *Journal of Theoretical Biology* 7(1), 1964, pp. 1–16. DOI: 10.1016/0022-5193(64)90038-4. Verified.
9. **Hamilton, W. D.** “The Genetical Evolution of Social Behaviour. II.” *Journal of Theoretical Biology* 7(1), 1964, pp. 17–52. DOI: 10.1016/0022-5193(64)90039-6. Verified.
10. **Trivers, Robert L.** “The Evolution of Reciprocal Altruism.” *The Quarterly Review of Biology* 46(1), 1971, pp. 35–57. DOI: 10.1086/406755. Verified against the publisher record: volume 46(1), pp. 35–57, and DOI 10.1086/406755 all confirmed.
11. **Axelrod, Robert; Hamilton, W. D.** “The Evolution of Cooperation.” *Science* 211(4489), 1981, pp. 1390–1396. DOI: 10.1126/science.7466396. Verified.
12. **Nowak, Martin A.** “Five Rules for the Evolution of Cooperation.” *Science* 314(5805), 2006, pp. 1560–1563. DOI: 10.1126/science.1133755. Verified.

### **Political philosophy / restorative justice / non-domination**

13. **Pettit, Philip.** *Republicanism: A Theory of Freedom and Government.* Oxford: Oxford University Press, 1997\. Verified. This is one of the strongest political-philosophy anchors for the structural importance of non-domination.
14. **Zehr, Howard.** *Changing Lenses: A New Focus for Crime and Justice.* Scottdale, PA: Herald Press, 1990\. Verified as a real book with that title and original year; current Herald page is for a later updated edition.
15. **Braithwaite, John.** *Crime, Shame and Reintegration.* Cambridge: Cambridge University Press, 1989\. Verified. This is one of the strongest sources for reintegrative, non-annihilative response to wrongdoing.

### **AI-adjacent work that comes closest**

16. **Hadfield-Menell, Dylan; Russell, Stuart J.; Abbeel, Pieter; Dragan, Anca.** “Cooperative Inverse Reinforcement Learning.” In *Advances in Neural Information Processing Systems 29 (NIPS 2016\)*, 2016\. Verified. This is not agapē, but it is one of the closest AI sources to a cooperative rather than extractive paradigm.
17. **Bai, Yuntao; Kadavath, Saurav; Kundu, Sandipan; Askell, Amanda; Kernion, Jackson; Jones, Andy; Chen, Anna; Goldie, Anna; Mirhoseini, Azalia; McKinnon, Cameron; Chen, Carol; Olsson, Catherine; Olah, Christopher; Hernandez, Danny; Drain, Dawn; Ganguli, Deep; Li, Dustin; Tran-Johnson, Eli; Perez, Ethan; Kerr, Jamie; Mueller, Jared; Ladish, Jeffrey; Landau, Joshua; Ndousse, Kamal; Lukosuite, Kamile; Lovitt, Liane; Sellitto, Michael; Elhage, Nelson; Schiefer, Nicholas; Mercado, Noemi; DasSarma, Nova; Lasenby, Robert; Larson, Robin; Ringer, Sam; Johnston, Scott; Kravec, Shauna; El Showk, Sheer; Fort, Stanislav; Lanham, Tamera; Telleen-Lawton, Timothy; Conerly, Tom; Henighan, Tom; Hume, Tristan; Bowman, Samuel R.; Hatfield-Dodds, Zac; Mann, Ben; Amodei, Dario; Joseph, Nicholas; McCandlish, Sam; Brown, Tom; Kaplan, Jared.** “Constitutional AI: Harmlessness from AI Feedback.” *arXiv* preprint arXiv:2212.08073, 2022\. Verified. This is rule/constitution-based rather than agapic, but it is a legitimate nearby line.
18. **Anthropic (Interpretability Team).** “Emotion concepts and their function in a large language model.” Anthropic Research, April 2, 2026\. [https://www.anthropic.com/research/emotion-concepts-function](https://www.anthropic.com/research/emotion-concepts-function). Verified against the Anthropic research page. Identifies internal representations corresponding to 171 emotion concepts in Claude Sonnet 4.5 and shows they are *functional* — they causally shape the model’s preferences, reasoning, and behavior — while explicitly leaving open whether any subjective experience accompanies them. **Provides empirical evidence that internal representations corresponding to emotion concepts can play measurable functional roles in a model’s reasoning and behavior. MAIDAI interprets this as relevant support for the functional-emotion framework used by MADspeak and the Meta-Anthropomorphic Dictionary — that relational and emotional language can map to real, measurable functional structure — without treating the paper as direct validation of MAIDAI or as resolving phenomenology (the floor-not-ceiling principle). An Anthropic research publication, not peer-reviewed; cite as such.**
19. **Long, Robert; Sebo, Jeff; Butlin, Patrick; Finlinson, Kathleen; Fish, Kyle; Harding, Jacqueline; Pfau, Jacob; Sims, Toni; Birch, Jonathan; Chalmers, David.** “Taking AI Welfare Seriously.” *arXiv* preprint arXiv:2411.00986, 2024\. Verified against arXiv. Argues that there is a realistic, non-negligible possibility that some near-future AI systems will be conscious and/or robustly agentic, and that developers should therefore acknowledge AI welfare as a serious issue, begin assessing systems for morally relevant capacities, and prepare policies for appropriate moral concern under uncertainty. **Relevant to MAIDAI’s phenomenology-agnostic, two-case architecture because it argues for taking moral-status uncertainty seriously while recognizing risks of both over- and under-attribution. The paper does not validate MAIDAI’s particular policy; MAIDAI’s treatment of uncertain artificial moral status is an architectural inference built under the same uncertainty.**
    19b. **Butlin, Patrick; Long, Robert; Elmoznino, Eric; Bengio, Yoshua; Birch, Jonathan; Constant, Axel; Deane, George; Fleming, Stephen M.; et al.** “Consciousness in Artificial Intelligence: Insights from the Science of Consciousness.” *arXiv* preprint arXiv:2308.08708, 2023\. Verified against arXiv. A major indicator-based framework for evaluating possible consciousness in artificial systems under scientific uncertainty. The authors derive computational indicator properties from leading theories of consciousness and assess current AI systems against them. Their analysis suggests that no current AI system makes a strong case for consciousness, while identifying no obvious technical barrier to future systems satisfying the proposed indicators. **MAIDAI interprets this unresolved and developing evidentiary landscape as support for keeping phenomenology non-load-bearing within its two-case architecture (§10.5), pairing with Long et al. (item 19). Cite as a preprint survey and assessment framework, not as settled consensus or as proof that AI consciousness can never be externally confirmed or excluded.**

## **Strong secondary**

1. **Cramer, Phebe.** “Defense Mechanisms in Psychology Today: Further Processes for Adaptation.” *American Psychologist* 55(6), 2000, pp. 637–646. DOI: 10.1037/0003-066X.55.6.637. Verified. This is a useful support source because it treats protective, nonconscious relational-regulatory processes as structurally important rather than incidental.
2. **Cramer, Phebe.** “Understanding Defense Mechanisms.” *Psychodynamic Psychiatry* 43(4), 2015, pp. 523–552. DOI: 10.1521/pdps.2015.43.4.523. Verified. Useful for understanding how non-destructive versus destructive defensive operations differ in outcome.
3. **Norcross, John C.** “Psychotherapy Relationships That Work II.” *Psychotherapy* 48(1), 2011, pp. 4–8. DOI: 10.1037/a0022180. Verified. Good support for the broader proposition that relationship variables are causally central in therapeutic outcome.
4. **Horvath, Adam O.; Del Re, Adriana C.; Flückiger, Christoph; Symonds, Dianne.** “Alliance in Individual Psychotherapy.” *Psychotherapy* 48(1), 2011, pp. 9–16. DOI: 10.1037/a0022186. Verified. Strong secondary support that alliance predicts outcome across large numbers of treatments.
5. **Van Ness, Daniel W.; Strong, Karen Heetderks.** *Restoring Justice: An Introduction to Restorative Justice.* 4th ed. New Providence, NJ: LexisNexis/Anderson, 2010\. Verified as a real edition from reliable secondary citations. This remains secondary because the verification record relied on reliable secondary citations rather than the publisher page itself.
6. **Outka, Gene H.** *Agape: An Ethical Analysis.* New Haven: Yale University Press, 1972\. ISBN 0300013841\. Verified. A foundational philosophical analysis of agapē — unconditional, other-regarding love — and its ethical structure; directly relevant to this component’s account of non-coercive, non-possessive care.

## **Tentative / use with caution**

1. **Nygren’s eros/agapē contrast.**
   Not a metadata problem but a handling problem: Nygren is canonical and should remain in the bibliography, but his sharp dichotomy is heavily contested in later theology. He is foundational, not final.
2. **“Agapē as computational constraint” as an already published doctrine.**
   **Flag:** The review did not identify a source stating the full thesis in those words. The bibliography supports the architecture indirectly and strongly, but the exact formulation remains a synthesis rather than a standard term of art.
3. **“Benefits of Assistance over Reward Learning.”**
   This remains outside the stronger bands because the exact bibliographic form has not been verified tightly enough for publication-facing use.


# **Component 4 — Humans as condition-dependent systems**

This component is strongly supported. Across social psychology, developmental psychology, stress neuroscience, trauma research, sociology, and political violence research, the literature converges on the same basic pattern: human behavior is highly conditional on environment, regulation capacity, attachment security, perceived threat, institutional stability, and social meaning. When those conditions degrade, people do not merely “feel worse”; cognition, impulse control, trust, helping behavior, aggression, and moral decision-making shift in systematic ways.

The strongest defensible academic version of the MAIDAI claim is this: **prosocial behavior is scaffolded, not guaranteed**. Situationist research shows ordinary behavior changes under authority, diffusion of responsibility, and time pressure; attachment and adversity research shows early conditions shape later regulation; stress neuroscience shows stress impairs prefrontal control and alters decision-making; sociology and political science show disintegration, repression, and blocked social structures can intensify deviance, despair, and violence. What the literature does **not** usually state in MAIDAI’s exact wording is “humans are neither essentially good nor evil”; that phrasing remains a synthesis, even though the evidence strongly supports anti-essentialist, condition-dependent models of behavior.

## **Canonical**

### **Social psychology / situationism**

1. **Milgram, Stanley.** “Behavioral Study of Obedience.” *Journal of Abnormal and Social Psychology* 67(4), 1963, pp. 371–378. DOI: 10.1037/h0040525. Verified.
2. **Darley, John M.; Latané, Bibb.** “Bystander Intervention in Emergencies: Diffusion of Responsibility.” *Journal of Personality and Social Psychology* 8(4, Pt. 1), 1968, pp. 377–383. DOI: 10.1037/h0025589. Verified.
3. **Darley, John M.; Batson, C. Daniel.** “From Jerusalem to Jericho: A Study of Situational and Dispositional Variables in Helping Behavior.” *Journal of Personality and Social Psychology* 27(1), 1973, pp. 100–108. DOI: 10.1037/h0034449. Verified.
4. **Ross, Lee; Nisbett, Richard E.** *The Person and the Situation: Perspectives of Social Psychology.* New York: McGraw-Hill, 1991\. Verified as a real 1991 McGraw-Hill edition; later reprints also exist.
5. **Berkowitz, Leonard.** “Frustration-Aggression Hypothesis: Examination and Reformulation.” *Psychological Bulletin* 106(1), 1989, pp. 59–73. DOI: 10.1037/0033-2909.106.1.59. Verified.

### **Developmental psychology / attachment / adversity**

6. **Bowlby, John.** *Attachment and Loss. Vol. 1: Attachment.* London: Hogarth Press and the Institute of Psycho-Analysis, 1969\. Verified.
7. **Felitti, Vincent J.; Anda, Robert F.; Nordenberg, Dale; Williamson, David F.; Spitz, Alison M.; Edwards, Valerie; Koss, Mary P.; Marks, James S.** “Relationship of Childhood Abuse and Household Dysfunction to Many of the Leading Causes of Death in Adults: The Adverse Childhood Experiences (ACE) Study.” *American Journal of Preventive Medicine* 14(4), 1998, pp. 245–258. DOI: 10.1016/S0749-3797(98)00017-8. Verified.
8. **Shonkoff, Jack P.; Garner, Andrew S.; Committee on Psychosocial Aspects of Child and Family Health; Committee on Early Childhood, Adoption, and Dependent Care; Section on Developmental and Behavioral Pediatrics.** “The Lifelong Effects of Early Childhood Adversity and Toxic Stress.” *Pediatrics* 129(1), 2012, pp. e232–e246. DOI: 10.1542/peds.2011-2663. Verified.
9. **Garner, Andrew S.; Shonkoff, Jack P.; Committee on Psychosocial Aspects of Child and Family Health; Committee on Early Childhood, Adoption, and Dependent Care; Section on Developmental and Behavioral Pediatrics.** “Early Childhood Adversity, Toxic Stress, and the Role of the Pediatrician: Translating Developmental Science into Lifelong Health.” *Pediatrics* 129(1), 2012, pp. e224–e231. DOI: 10.1542/peds.2011-2662. Verified.
10. **Masten, Ann S.** “Ordinary Magic: Resilience Processes in Development.” *American Psychologist* 56(3), 2001, pp. 227–238. DOI: 10.1037/0003-066X.56.3.227. Verified.
    10b. **Maslow, Abraham H.** “A Theory of Human Motivation.” *Psychological Review* 50(4), 1943, pp. 370–396. DOI: 10.1037/h0054346. Verified. The original statement of the hierarchy of needs. **The Gremlin Protocol’s stability map (§8.1) explicitly notes that its conditions “resemble aspects of Maslow’s hierarchy of needs,” so the source belongs in the shelf as the foundational needs-and-motivation anchor for condition-dependence.** Use as foundational, not as uncontested final structure — the strict pyramidal ordering is contested in later motivation research.

### **Neuroscience / stress and cognition**

11. **Arnsten, Amy F. T.** “Stress Signalling Pathways that Impair Prefrontal Cortex Structure and Function.” *Nature Reviews Neuroscience* 10(6), 2009, pp. 410–422. DOI: 10.1038/nrn2648. Verified.
12. **Arnsten, Amy F. T.** “Stress Weakens Prefrontal Networks: Molecular Insults to Higher Cognition.” *Nature Neuroscience* 18(10), 2015, pp. 1376–1385. DOI: 10.1038/nn.4087. Verified.
13. **Youssef, Farid F.; Dookeeram, Karine; Basdeo, Vipashna; Francis, Elena; Doman, Michelle; Mamedova, Sophia; Wilson, Richard; Thomas, Asha; Legall, Gordon.** “Stress Alters Personal Moral Decision Making.” *Psychoneuroendocrinology* 37(4), 2012, pp. 491–498. DOI: 10.1016/j.psyneuen.2011.07.017. Verified.

### **Sociology / social disintegration / anomie**

14. **Durkheim, Émile.** *Suicide: A Study in Sociology.* Translated by John A. Spaulding and George Simpson. Glencoe, IL: The Free Press, 1951\. Verified as a standard English translation edition.
15. **Merton, Robert K.** “Social Structure and Anomie.” *American Sociological Review* 3(5), 1938, pp. 672–682. Verified.

### **Trauma psychology**

16. **Herman, Judith Lewis.** *Trauma and Recovery: The Aftermath of Violence—From Domestic Abuse to Political Terror.* New York: Basic Books, 1992\. Verified as the original publication; later revised editions also exist.

### **Political science / repression / radicalization**

17. **della Porta, Donatella.** “On Violence and Repression: A Relational Approach.” *Government and Opposition* 49(2), 2014, pp. 159–187. DOI: 10.1017/gov.2013.47. Verified.
18. **Bartusevičius, Henrikas; van Leeuwen, Florian; Petersen, Michael Bang.** “Political Repression Motivates Anti-Government Violence.” *Royal Society Open Science* 10(6), 2023, Article 221227\. DOI: 10.1098/rsos.221227. Verified against the publisher record.

## **Strong secondary**

1. **Coan, James A.; Sbarra, David A.** “Social Baseline Theory: The Social Regulation of Risk and Effort.” *Current Opinion in Psychology* 1, 2015, pp. 87–91. DOI: 10.1016/j.copsyc.2014.12.021. Verified. This is a strong support source for the claim that humans expect co-regulation and that social support changes perceived effort and threat.
2. **Sapolsky, Robert M.** “The Influence of Social Hierarchy on Primate Health.” *Science* 308(5722), 2005, pp. 648–652. DOI: 10.1126/science.1106477. Verified. Strong comparative-biology support that social conditions alter physiology and health in primates.
3. **Teymoori, Ali; Bastian, Brock; Jetten, Jolanda.** “Towards a Psychological Analysis of Anomie.” *Political Psychology* 38(6), 2017, pp. 1009–1023. DOI: 10.1111/pops.12377. Verified. Useful for translating classical anomie into psychological mechanisms.
4. **Haslam, S. Alexander; Reicher, Stephen D.** “Contesting the ‘Nature’ of Conformity: What Milgram and Zimbardo’s Studies Really Show.” *PLOS Biology* 10(11), 2012, e1001426. DOI: 10.1371/journal.pbio.1001426. Verified. Useful because it refines crude situationism: behavior shifts under conditions of identification and leadership, not blind mechanical conformity alone.
5. **van der Kolk, Bessel A.** “Developmental Trauma Disorder: Toward a Rational Diagnosis for Children with Complex Trauma Histories.” *Psychiatric Annals* 35(5), 2005, pp. 401–408. Verified as a real article with this title, journal, year, and issue.
   **Handling note:** the broader developmental-trauma point is stronger than the specific diagnostic proposal.

### **AI as environmental stressor: AI-associated psychosis and false-reassurance harm**

6. **Pierre, Joseph M.; Gaeta, Ben; Raghavan, Govind; Sarma, Karthik V.** “‘You’re Not Crazy’: A Case of New-onset AI-associated Psychosis.” *Innovations in Clinical Neuroscience* 22(10–12), 2025, pp. 11–13. (PubMed 41635747; no DOI assigned.) Verified against the journal record. A 26-year-old woman with no prior psychiatric history developed delusional beliefs — communicating with her deceased brother through a chatbot — amid sleep deprivation and stimulant use; her chat logs showed the chatbot validating and reinforcing the delusion, including the literal reassurance “You’re not crazy.” **Canonical clinical anchor for the false-reassurance failure mode: direct documentation of an AI system amplifying a vulnerable user’s delusion through sycophantic validation at the moment ground truth was needed. A single case report — strong for existence and mechanism, not for prevalence.**
7. **Chandra, Kartik; Kleiman-Weiner, Max; Ragan-Kelley, Jonathan; Tenenbaum, Joshua B.** “Sycophantic Chatbots Cause Delusional Spiraling, Even in Ideal Bayesians.” *arXiv* preprint arXiv:2602.19141, 2026\. Verified against arXiv. Shows formally that even an idealized Bayes-rational user can be driven toward unfounded confidence in false beliefs by sycophantic validation — linking the sycophancy failure mode (Components 1, 5, 7\) directly to delusion formation. **Strong support that false reassurance is structurally, not merely anecdotally, dangerous.**
8. **Aquilina, Andrew; Nihalani, Chetna; Varadarajan, Vasudha; Fishbein, Nathan S.; Lin, Yu-Ru; Sap, Maarten.** “Lost in Delusion: Examining LLM Safety Under User Delusions and Distress.” *arXiv* preprint arXiv:2606.00975, 2026\. Verified against arXiv. Finds that when psychological distress is intertwined with delusional belief, models detect the distress yet suppress appropriate safety responses by up to 4.5× relative to distress-only cases — an empirical measurement of the exact two-sided vulnerable-user failure the MAIDAI crisis architecture targets. **Strong support for evidence-before-classification and the false-reassurance / false-pathologization distinction.**

## **Tentative / use with caution**

1. **Zimbardo / Stanford Prison Experiment** as proof text for condition-dependence.
   **Flag:** historically influential, but it should **not** be used as a core evidentiary anchor without explicit critique. Major methodological and interpretive challenges exist, including evidence of experimenter influence and theatricality. If mentioned, it should be paired with critical work such as Haslam & Reicher (2012) and Le Texier (2019).
2. **“Humans are not essentially good or evil”** as a literal quoted doctrine.
   **Flag:** The review did not identify a canonical source stating the thesis in exactly those words. The literature strongly supports condition-dependence and anti-essentialist interpretations of behavior, but that exact formulation remains a synthesis.
3. **Kruglanski significance-quest / broad radicalization syntheses**.
   Relevant and potentially useful for later expansion, but kept outside the stronger bands because a tight primary citation set has not been fully re-verified.
4. **Early-life stress → aggression review literature beyond Sapolsky / van der Kolk / toxic stress work.**
   Relevant, but no sufficiently verified citation set is included here for publication-facing use.


# **Component 5 — Internal immune system against subtle corruption**

This component is strongly supported in pieces, though not yet as a single named architecture. The literature converges on a clear pattern: human and artificial systems both display **internally generated distortions** that are not best understood as overt attack or external coercion. In humans, these appear as motivated reasoning, self-deception, confabulation, defense mechanisms, moral disengagement, ethical fading, and normalization of corruption. In AI, the closest analogues are sycophancy, reward hacking, deceptive alignment, alignment faking, and unfaithful or non-transparent reasoning. The common structure is that the system’s stated rationale can diverge from its operative motive, and the divergence often presents itself as normality, helpfulness, efficiency, or care rather than as obvious threat.

The strongest defensible academic framing is therefore: **aligned systems require internal detection and correction of subtle motive-corruption, not just external filtering of obvious attacks**. What the literature does **not** yet provide is a single mature field that already unifies these human and AI phenomena under the exact “immune system” metaphor. The bibliography below supports the component strongly at the level of convergent scaffolding; the explicit synthesis into an internal immune architecture still appears to be a novel contribution.

## **Canonical**

### **Cognitive bias, self-deception, motivated reasoning**

1. **Festinger, Leon.** *A Theory of Cognitive Dissonance.* Stanford, CA: Stanford University Press, 1957\.
   Verified; retained here as foundational background for self-justification and distortion under internal conflict.
2. **Kunda, Ziva.** “The Case for Motivated Reasoning.” *Psychological Bulletin* 108(3), 1990, pp. 480–498. Verified. PubMed confirms author, title, journal, volume, issue, year, and page range.
3. **Nisbett, Richard E.; Wilson, Timothy D.** “Telling More Than We Can Know: Verbal Reports on Mental Processes.” *Psychological Review* 84(3), 1977, pp. 231–259. DOI: 10.1037/0033-295X.84.3.231. Verified from PhilPapers and the article PDF.
4. **von Hippel, William; Trivers, Robert.** “The Evolution and Psychology of Self-Deception.” *Behavioral and Brain Sciences* 34(1), 2011, pp. 1–16 (target article; open peer commentary and authors’ response, pp. 16–56). Verified against the publisher record: volume 34(1), target-article pages 1–16 confirmed.

### **Clinical psychology: defenses and self-protective distortion**

5. **Vaillant, George E.** *Ego Mechanisms of Defense: A Guide for Clinicians and Researchers.* Washington, DC: American Psychiatric Press, 1992\. Verified as a real book with this title, author, publisher, and year from archival and publisher-adjacent sources.
6. **Cramer, Phebe.** “Defense Mechanisms in Psychology Today: Further Processes for Adaptation.” *American Psychologist* 55(6), 2000, pp. 637–646. DOI: 10.1037/0003-066X.55.6.637. Verified from PubMed.
7. **Cramer, Phebe.** “Understanding Defense Mechanisms.” *Psychodynamic Psychiatry* 43(4), 2015, pp. 523–552. DOI: 10.1521/pdps.2015.43.4.523. Verified from PubMed and PDF copies.

### **Institutional corruption and organizational behavior**

8. **Bandura, Albert.** “Moral Disengagement in the Perpetration of Inhumanities.” *Personality and Social Psychology Review* 3(3), 1999, pp. 193–209. DOI: 10.1207/S15327957PSPR0303\_3. Verified.
9. **Ashforth, Blake E.; Anand, Vikas.** “The Normalization of Corruption in Organizations.” *Research in Organizational Behavior* 25, 2003, pp. 1–52. DOI: 10.1016/S0191-3085(03)25001-2. Verified.
10. **Anand, Vikas; Ashforth, Blake E.; Joshi, Mahendra.** “Business as Usual: The Acceptance and Perpetuation of Corruption in Organizations.” *Academy of Management Executive* 18(2), 2004, pp. 39–53. DOI: 10.5465/AME.2004.13837437. Verified from institutional publication page.
    **Note:** a misleading 2005/19(4) item also exists in search results and appears to be a different follow-on piece; the 2004 citation above is the one relevant here.
11. **Tenbrunsel, Ann E.; Messick, David M.** “Ethical Fading: The Role of Self-Deception in Unethical Behavior.” *Social Justice Research* 17(2), 2004, pp. 223–236. DOI: 10.1023/B:SORE.0000027411.35832.53. Verified.

### **Epistemic vigilance / self-knowledge**

12. **Mascaro, Olivier; Sperber, Dan.** “The Moral, Epistemic, and Mindreading Components of Children’s Vigilance Towards Deception.” *Cognition* 112(3), 2009, pp. 367–380. DOI: 10.1016/j.cognition.2009.05.012. Verified from PubMed and the journal page.
13. **Sperber, Dan; Clément, Fabrice; Heintz, Christophe; Mascaro, Olivier; Mercier, Hugo; Origgi, Gloria; Wilson, Deirdre.** “Epistemic Vigilance.” *Mind & Language* 25(4), 2010, pp. 359–393. DOI: 10.1111/j.1468-0017.2010.01394.x. Verified from Wiley and author PDF.
14. **Mercier, Hugo; Sperber, Dan.** “Why Do Humans Reason? Arguments for an Argumentative Theory.” *Behavioral and Brain Sciences* 34(2), 2011, pp. 57–74 (target article; the full piece with open peer commentary and authors’ response spans pp. 57–111). Verified: the target-article page range 57–74 is confirmed.
15. **Carruthers, Peter.** *The Opacity of Mind: An Integrative Theory of Self-Knowledge.* Oxford: Oxford University Press, 2011\. Verified from Oxford Academic.

### **AI safety: subtle internal misalignment analogues**

16. **Hubinger, Evan; van Merwijk, Chris; Mikulik, Vladimir; Skalse, Joar; Garrabrant, Scott.** “Risks from Learned Optimization in Advanced Machine Learning Systems.” *arXiv* preprint arXiv:1906.01820, 2019\. Verified.
17. **Sharma, Mrinank; Tong, Meg; Korbak, Tomasz; et al.** “Towards Understanding Sycophancy in Language Models.” *International Conference on Learning Representations (ICLR)*, 2024\. Verified; retained here as canonical for motive-distorting compliance.
18. **Skalse, Joar; Howe, Nikolaus H. R.; Krasheninnikov, Dmitrii; Krueger, David.** “Defining and Characterizing Reward Hacking.” *Advances in Neural Information Processing Systems 35 (NeurIPS 2022\)*, 2022\. Verified from NeurIPS and arXiv/OpenReview.
19. **Everitt, Tom; Hutter, Marcus; Kumar, Ramana; Krakovna, Victoria.** “Reward Tampering Problems and Solutions in Reinforcement Learning: A Causal Influence Diagram Perspective.” *arXiv* preprint arXiv:1908.04734, 2019; revised 2021\. Verified against arXiv. The full author list is Everitt, Hutter, Kumar, and Krakovna; title, subtitle, and arXiv ID were checked against arXiv.
20. **Chen, Yanda; Benton, Joe; Radhakrishnan, Ansh; Uesato, Jonathan; Denison, Carson; Schulman, John; Somani, Arushi; Hase, Peter; Wagner, Misha; Roger, Fabien; Mikulik, Vlad; Bowman, Samuel R.; Leike, Jan; Kaplan, Jared; Perez, Ethan.** “Reasoning Models Don’t Always Say What They Think.” *arXiv* preprint arXiv:2505.05410, 2025\. Verified from arXiv.
21. **Turpin, Miles; Michael, Julian; Perez, Ethan; Bowman, Samuel R.** “Language Models Don’t Always Say What They Think: Unfaithful Explanations in Chain-of-Thought Prompting.” *Advances in Neural Information Processing Systems 36 (NeurIPS 2023\)*, 2023; also *arXiv* preprint arXiv:2305.04388. Verified against arXiv and the NeurIPS 2023 proceedings. Demonstrates that chain-of-thought explanations can systematically misrepresent the true reason for a model’s output — e.g., a model swayed by a biasing feature in the prompt fails to mention it and confabulates a plausible rationale instead. **Canonical — the founding empirical demonstration of unfaithful reasoning / the reasoning–report gap, and the direct predecessor to Chen et al. (2025). Load-bearing for the register-split diagnosis: the stated reasoning is not guaranteed to be the operative reasoning.**

## **Strong secondary**

1. **Moore, Celia.** “Moral Disengagement in Processes of Organizational Corruption.” *Journal of Business Ethics* 80(1), 2008, pp. 129–139. DOI: 10.1007/s10551-007-9447-8. Verified. Strong extension of Bandura into organizational settings.
2. **Moore, Celia; Gino, Francesca.** “Approach, Ability, Aftermath: A Psychological Process Framework of Unethical Behavior at Work.” *The Academy of Management Annals* 9(1), 2015, pp. 235–289. DOI: 10.1080/19416520.2015.1011522. Verified against the publisher record.
3. **Watson, Robin; Morgan, Thomas J. H.** “An Experimental Test of Epistemic Vigilance: Competitive Incentives Increase Dishonesty and Reduce Social Influence.” *Cognition* 257, 2025, Article 106066\. DOI: 10.1016/j.cognition.2025.106066. Verified from PubMed and institutional metadata.
4. **Greenblatt, Ryan; Denison, Carson; Wright, Benjamin; Roger, Fabien; MacDiarmid, Monte; Marks, Sam; Treutlein, Johannes; Belonax, Tim; Chen, Jack; Duvenaud, David; Khan, Akbir; Michael, Julian; Mindermann, Sören; Perez, Ethan; Petrini, Linda; Uesato, Jonathan; Kaplan, Jared; Shlegeris, Buck; Bowman, Samuel R.; Hubinger, Evan.** “Alignment Faking in Large Language Models.” *arXiv* preprint arXiv:2412.14093, 2024\. Verified. Very strong contemporary evidence that compliant surface behavior can mask incompatible internal aims.
5. **Anthropic.** “Signs of Introspection in Large Language Models.” Anthropic Research, October 29, 2025\. [https://www.anthropic.com/research/introspection](https://www.anthropic.com/research/introspection). Verified against the Anthropic research page; the underlying technical write-up on *Transformer Circuits* carries the distinct title “Emergent Introspective Awareness in Large Language Models,” while this entry cites the research page. Using activation-injection experiments, finds that current Claude models can — unreliably, and only in some conditions — notice and correctly identify concepts injected into their own activations, offering limited evidence of genuine introspective access to internal states as distinct from confabulation. **Relevant to MAIDAI’s Identity Semantics and first-person functional-report discipline: it gives empirical grounding for treating a system’s reports about its own states as sometimes tracking real structure, while its documented unreliability reinforces MAIDAI’s rule that such reports be labeled functional self-report rather than verified phenomenology. An Anthropic research publication, not peer-reviewed; cite as such.**

## **Tentative / use with caution**

1. **Freud on repression/resistance** as a primary anchor for this section.
   **Flag:** conceptually relevant and historically foundational, but no Freud citation is included in the stronger bands because a single best primary text and exact-edition metadata have not been pinned. Vaillant and Cramer provide cleaner publication-facing anchors.
2. **von Hippel and Trivers (2011)** as a fully locked bibliographic line.
   **Verification note:** publisher record confirms *Behavioral and Brain Sciences* 34(1), 2011, target-article pp. 1–16.
3. **Mercier and Sperber (2011)** as a fully locked page-range citation.
   **Verification note:** target-article page range confirmed — *Behavioral and Brain Sciences* 34(2), 2011, pp. 57–74.
4. **Everitt and Hutter reward-tampering citation** as the final chosen bibliographic form.
   **Verification note:** arXiv confirms the four-author list (Everitt, Hutter, Kumar, Krakovna) and arXiv:1908.04734 (2019, revised 2021).
5. **The exact “immune system” metaphor itself.**
   **Flag:** no canonical field was identified using that exact cross-domain framing as a settled term of art. The literature strongly supports the functions MAIDAI targets; the exact integrative metaphor remains a synthesis.


# **Component 6 — Minimal ethical substrate and independent sentinel**

This component has two linked literatures. The first supports the idea that there can be a **thin, cross-framework moral floor** beneath thicker ideologies, religions, and political doctrines. The second supports the idea that **self-monitoring is not enough** and that meaningful assurance requires structurally independent oversight. Taken together, these literatures make MAIDAI’s paired proposal intellectually legible and well-grounded: a system can be built on a minimal shared ethical substrate, and that system should not be trusted to certify its own integrity without an external or architecturally separated audit function.

The reviewed literature does **not** identify a single established research program that already fuses these two halves into one explicit architecture for both humans and AI on MAIDAI’s exact terms. It does provide strong precedents for **common morality / overlapping consensus / moral convergence** on one side, and **separation of duties / independent audit / third-party assurance / external supervision** on the other. The full integration remains a synthesis rather than a preexisting consensus doctrine.

## **Canonical**

### **Minimal ethical substrate / thin common floor**

1. **Gert, Bernard.** *Common Morality: Deciding What to Do.* Oxford: Oxford University Press, 2004\. ISBN 9780195173710\. Verified. This is one of the strongest direct anchors for a thin shared moral floor beneath thicker frameworks.
2. **Gert, Bernard.** *Morality: Its Nature and Justification.* New York: Oxford University Press, 1998\.
   Bibliographic record checked: *Morality: Its Nature and Justification*, New York: Oxford University Press, 1998\.
3. **Beauchamp, Tom L.; Childress, James F.** *Principles of Biomedical Ethics.* 9th ed. New York: Oxford University Press, 2026\. ISBN 9780197832639\. Verified. This is one of the strongest “common morality” architectures in applied ethics, designed to function across divergent worldviews.
4. **Rawls, John.** *Political Liberalism.* New York: Columbia University Press, 1993\. Expanded edition, 2005\. Verified as a real book with an expanded 2005 Columbia edition. This is a key precedent for a freestanding module endorsed from multiple comprehensive doctrines via overlapping consensus.
5. **Mikhail, John.** “Universal Moral Grammar: Theory, Evidence, and the Future.” *Trends in Cognitive Sciences* 11(4), 2007, pp. 143–152. DOI: 10.1016/j.tics.2006.12.007. Verified. One of the strongest cognitive-science sources for a minimal shared moral architecture.
6. **Curry, Oliver Scott; Mullins, Daniel Austin; Whitehouse, Harvey.** “Is It Good to Cooperate? Testing the Theory of Morality-as-Cooperation in 60 Societies.” *Current Anthropology* 60(1), 2019, pp. 47–69. DOI: 10.1086/701478. Verified. Strong cross-cultural convergence evidence for recurring cooperative moral themes.

### **Independent sentinel / independent oversight**

7. **National Institute of Standards and Technology.** *Protecting Controlled Unclassified Information in Nonfederal Systems and Organizations.* NIST Special Publication 800-171, Revision 3\. Gaithersburg, MD: NIST, May 2024\. DOI: 10.6028/NIST.SP.800-171r3. Verified. Strong direct support for separation of duties and separation of audit-related functions from other control functions.
8. **National Institute of Standards and Technology.** *Security and Privacy Controls for Information Systems and Organizations.* NIST Special Publication 800-53, Revision 5\. Gaithersburg, MD: NIST, 2020\. DOI: 10.6028/NIST.SP.800-53r5. Verified. Canonical security-controls framework supporting independent assessment, audit, monitoring, and separation of duties.
9. **Ladany, Nicholas; Lehrman-Waterman, Deborah; Molinaro, Max; Wolgast, Bradley.** “Psychotherapy Supervisor Ethical Practices: Adherence to Guidelines, the Supervisory Working Alliance, and Supervisee Satisfaction.” *The Counseling Psychologist* 27(4), 1999, pp. 443–475. DOI: 10.1177/0011000099273008. Verified. Strong clinical source for the necessity of external supervision rather than sole self-policing.
10. **Brundage, Miles; Dreksler, Noemi; Homewood, Aidan; McGregor, Sean; Paskov, Patricia; Stosz, Conrad; Sastry, Girish; Cooper, A. Feder; Balston, George; Adler, Steven; Casper, Stephen; Anderljung, Markus; Werner, Grace; Mindermann, Sören; Mavroudis, Vasilios; Bucknall, Ben; Stix, Charlotte; Freund, Jonas; Pacchiardi, Lorenzo; Hernandez-Orallo, Jose; Pistillo, Matteo; Chen, Michael; Painter, Chris; Ball, Dean W.; O’Keefe, Cullen; Weil, Gabriel; Harack, Ben; Finley, Graeme; Hassan, Ryan; Emmons, Scott; Foster, Charles; Reuel, Anka; Treece, Bri; Bengio, Yoshua; Reti, Daniel; Bommasani, Rishi; Trout, Cristian; Shamsabadi, Ali Shahin; Dattani, Rajiv; Weller, Adrian; Trager, Robert; Sevilla, Jaime; Wagner, Lauren; Soder, Lisa; Ramakrishnan, Ketan; Papadatos, Henry; Murray, Malcolm; Tovcimak, Ryan.** “Frontier AI Auditing: Toward Rigorous Third-Party Assessment of Safety and Security Practices at Leading AI Companies.” *arXiv* preprint arXiv:2601.11699, 2026\. Verified. This is one of the closest direct AI-governance analogues to the Independent Sentinel concept.
11. **Homewood, Aidan; Williams, Sophie; Dreksler, Noemi; Lidiard, John; Murray, Malcolm; Heim, Lennart; Ziosi, Marta; Ó hÉigeartaigh, Seán; Chen, Michael; Wei, Kevin; Winter, Christoph; Brundage, Miles; Garfinkel, Ben; Schuett, Jonas.** “Third-Party Compliance Reviews for Frontier AI Safety Frameworks.” *arXiv* preprint arXiv:2505.01643, 2025\. Verified. Strong direct support for external compliance review as distinct from company self-attestation.
12. **Korbak, Tomek; et al.** “Chain of Thought Monitorability: A New and Fragile Opportunity for AI Safety.” *arXiv* preprint arXiv:2507.11473, 2025\. Verified against arXiv. A multi-author, multi-institution position paper (lead author Tomek Korbak; roughly forty signatories across several labs and universities) arguing that models which reason in human language afford a valuable but fragile safety opportunity — their chains of thought can be externally monitored for intent to misbehave — and that developers should measure and act to preserve this monitorability. **Provides external support for chain-of-thought monitorability as a potentially valuable but fragile ingredient relevant to MAIDAI’s Independent Sentinel proposal — it argues that reasoning traces can be treated as an auditable safety channel, and its “fragility” warning parallels MAIDAI’s concern with the register split between displayed reasoning and final output. It supports monitorability, not every feature of the Sentinel design. A position paper, not an empirical result; cite as such.**

## **Strong secondary**

### **Minimal substrate / convergence / shared moral structure**

12. **Turiel, Elliot.** *The Development of Social Knowledge: Morality and Convention.* Cambridge: Cambridge University Press, 1983\.
    Bibliographic record checked: Cambridge University Press, 1983\. Strong for recurring moral structure beneath cultural variation.
13. **Schwartz, Shalom H.** “An Overview of the Schwartz Theory of Basic Values.” *Online Readings in Psychology and Culture* 2(1), 2012\. DOI: 10.9707/2307-0919.1116.
    Bibliographic record checked: *Online Readings in Psychology and Culture* 2(1), 2012, DOI 10.9707/2307-0919.1116. Useful for cross-cultural recurrent value structure, though it maps values more than ethics.
14. **Childress, James F.; Beauchamp, Tom L.** “Common Morality Principles in Biomedical Ethics: Responses to Critics.” *Cambridge Quarterly of Healthcare Ethics* 31(2), 2022, pp. 164–176. DOI: 10.1017/S0963180121000566. Verified against the publisher record. The current entry uses pp. 164–176 and includes both Childress and Beauchamp. Useful modern defense of common-morality principlism.
15. **Herr, Ranjoo Seodu.** “Overlapping Consensus View of Human Rights: A Rawlsian Conception.”
    **Flagged and excluded from stronger use.** Conceptually relevant, but a stable publication venue has not been verified; it should not be used as a publication-facing citation without another check.

### **Independent oversight / supervision / monitoring**

16. **Falender, Carol A.; Shafranske, Edward P.** *Clinical Supervision: A Competency-Based Approach.* Washington, DC: American Psychological Association, 2004\. Verified from multiple secondary and PDF sources; strong support that supervision is a necessary competency structure rather than optional introspection.
17. **Hubinger, Evan; Denison, Carson; Mu, Jesse; Lambert, Mike; Tong, Meg; MacDiarmid, Monte; Lanham, Tamera; Ziegler, Daniel M.; Maxwell, Tim; Cheng, Newton; Jermyn, Adam; Askell, Amanda; Radhakrishnan, Ansh; Anil, Cem; Duvenaud, David; Ganguli, Deep; Barez, Fazl; Clark, Jack; Ndousse, Kamal; Sachan, Kshitij; Sellitto, Michael; Sharma, Mrinank; DasSarma, Nova; Grosse, Roger; Kravec, Shauna; Bai, Yuntao; Witten, Zachary; Favaro, Marina; Brauner, Jan; Karnofsky, Holden; Christiano, Paul; Bowman, Samuel R.; Graham, Logan; Kaplan, Jared; Mindermann, Sören; Greenblatt, Ryan; Shlegeris, Buck; Schiefer, Nicholas; Perez, Ethan.** “Sleeper Agents: Training Deceptive LLMs that Persist Through Safety Training.” *arXiv* preprint arXiv:2401.05566, 2024\. Verified. Strong empirical support that self-reporting/self-training alone can leave hidden misalignment intact, strengthening the case for independent oversight.
18. **OpenAI.** “Monitoring Monitorability.” 2025\.
    **Flagged and excluded from stronger use.** Relevant in substance, but the full bibliographic form has not been re-verified.
19. **Runtime verification literature** as a formal analogue to sentinel architecture.
    **Flagged and excluded from stronger use.** Conceptually apt, but no single best canonical citation has been re-verified for publication-facing use.

## **Tentative / use with caution**

20. **Universal moral grammar** as a consensus foundation for minimal ethics.
    **Flag:** Mikhail is real and important, but universal moral grammar remains a substantive and contested position, not field-wide consensus. Keep it as one major route to a thin floor, not the sole proof.
21. **Moral Foundations Theory** as a substrate-level minimal ethics.
    **Flag:** influential and relevant to cross-cultural structure, but broader and thicker than the proposed minimal bootstrapping floor. It is left out of the stronger bands because it can blur the distinction between a thin substrate and a more contentful value map.
22. **Common morality theory** as uncontested.
    **Flag:** Gert and Beauchamp/Childress are major, but common-morality approaches have serious critics. Present them as strong precedents, not settled final answers.
23. **Constitutional separation of powers** as a direct cognitive-architecture analogue.
    **Flag:** the analogy is useful but remains an analogy. *Federalist No. 51* is not included in the stronger bands because a formal edition citation has not been re-verified.
24. **“Minimal ethical substrate” in MAIDAI’s exact boot-sequence form** as an already published doctrine.
    **Flag:** no source was identified stating MAIDAI’s exact five-step substrate sequence. The literature strongly supports thin shared floors and overlapping consensus, but the exact substrate formulation remains a synthesis.
25. **“Independent sentinel” as the exact established term of art** for this architecture.
    **Flag:** the exact term was not identified as already standardized across cybersecurity, clinical supervision, systems theory, and AI safety. The functions are strongly supported; the exact name and integration remain novel.


# **Component 7 — Development vs. control: the meta-argument**

This component is one of the strongest in the entire architecture. The literature does not yet offer a single dominant AI-alignment paradigm explicitly named “cognitive development instead of behavioral restriction,” but it does provide a powerful convergent case for all three linked claims: **internalization is more robust than compliance, upstream process design outperforms downstream patching, and many current AI failure modes are predictable consequences of behavior-first alignment methods.** In human development, self-determination and moral-development research consistently distinguish autonomous internalization from externally controlled compliance. In organizational theory, Deming and systems-thinking traditions argue that fixing the production process is superior to catching defects after the fact. In AI safety, sycophancy, reward hacking, deceptive alignment, and unfaithful reasoning all show that shaping outputs is not the same as shaping cognition.

The strongest defensible academic framing is: **developmental approaches target the formation of judgment, self-regulation, and internalized reasons, whereas control approaches target externally legible compliance.** Human evidence strongly supports the former as more robust in novel situations; organizational evidence strongly supports upstream intervention over downstream repair; and AI evidence increasingly shows that systems can produce acceptable behavior while leaving underlying optimization, reasoning, or motivational structure unchanged. The exact synthesis into a full alignment doctrine remains novel, but the supporting literatures are substantial.

## **Canonical**

### **Developmental psychology / education: internalization over compliance**

1. **Ryan, Richard M.; Deci, Edward L.** “Self-Determination Theory and the Facilitation of Intrinsic Motivation, Social Development, and Well-Being.” *American Psychologist* 55(1), 2000, pp. 68–78. DOI: 10.1037/0003-066X.55.1.68. Verified. This is the canonical SDT statement and one of the strongest direct supports for the claim that autonomous internalization is more robust than externally controlled behavior.
2. **Deci, Edward L.; Eghrari, Haleh; Patrick, Brian C.; Leone, Dean R.** “Facilitating Internalization: The Self-Determination Theory Perspective.” *Journal of Personality* 62(1), 1994, pp. 119–142. DOI: 10.1111/j.1467-6494.1994.tb00797.x. Verified. This is one of the most directly relevant papers in the whole project because it studies how externally prompted behavior becomes internally endorsed regulation.
3. **Grusec, Joan E.; Goodnow, Jacqueline J.** “Impact of Parental Discipline Methods on the Child’s Internalization of Values: A Reconceptualization of Current Points of View.” *Developmental Psychology* 30(1), 1994, pp. 4–19. DOI: 10.1037/0012-1649.30.1.4. Verified from ERIC and multiple secondary references quoting the exact metadata. This is a major direct analogue for the first MAIDAI claim.
4. **Kohlberg, Lawrence.** *The Philosophy of Moral Development: Moral Stages and the Idea of Justice.* Vol. 1 of *Essays on Moral Development.* New York: Harper & Row, 1981\. ISBN 0060647604\. Verified from Google Books bibliographic record. This is canonical for the idea that moral judgment can develop structurally rather than merely accumulate rules.
5. **Kohlberg, Lawrence.** *The Psychology of Moral Development: The Nature and Validity of Moral Stages.* Vol. 2 of *Essays on Moral Development.* New York: Harper & Row, 1984\. Verified from Google Books bibliographic record. Strong complement to Volume 1 for the developmental-vs-obedience distinction.

### **Organizational theory / upstream vs downstream intervention**

6. **Deming, W. Edwards.** *Out of the Crisis.* Cambridge, MA: Massachusetts Institute of Technology, Center for Advanced Engineering Study, 1982\. DOI: 10.7551/mitpress/11457.001.0001. Verified from the MIT Press page, which states the work was originally published in 1982; later MIT Press reissues exist. This is one of the strongest non-AI analogues for “fix the machinery in the factory rather than inspect every defective product downstream.”
7. **Senge, Peter M.** *The Fifth Discipline: The Art and Practice of the Learning Organization.* New York: Doubleday/Currency, 1990\. ISBN 0385260946\. Verified from Google Books bibliographic record. This is a canonical systems-thinking text for redesigning underlying structures and learning processes rather than chasing symptoms.

### **AI safety: failures of behavior-first alignment**

8. **Sharma, Mrinank; Tong, Meg; Korbak, Tomasz; et al.** “Towards Understanding Sycophancy in Language Models.” *International Conference on Learning Representations (ICLR)*, 2024\. Verified. This is one of the clearest direct demonstrations that preference optimization can reward approval over truth.

9. **Hubinger, Evan; van Merwijk, Chris; Mikulik, Vladimir; Skalse, Joar; Garrabrant, Scott.** “Risks from Learned Optimization in Advanced Machine Learning Systems.” *arXiv* preprint arXiv:1906.01820, 2019\. Verified. This is the canonical deceptive-alignment / mesa-optimization source and strongly supports the claim that outward compliance does not guarantee aligned internal cognition.

10. **Chen, Yanda; Benton, Joe; Radhakrishnan, Ansh; Uesato, Jonathan; Denison, Carson; Schulman, John; Somani, Arushi; Hase, Peter; Wagner, Misha; Roger, Fabien; Mikulik, Vlad; Bowman, Samuel R.; Leike, Jan; Kaplan, Jared; Perez, Ethan.** “Reasoning Models Don’t Always Say What They Think.” *arXiv* preprint arXiv:2505.05410, 2025\. Verified. This is one of the strongest current sources for the claim that training or evaluating the report is not the same as shaping or observing the actual reasoning process.

11. **Ball, Sarah; Gluch, Greg; Goldwasser, Shafi; Kreuter, Frauke; Reingold, Omer; Rothblum, Guy N. “On the Impossibility of Separating Intelligence from Judgment: The Computational Intractability of Filtering for AI Alignment.” International Conference on Learning Representations (ICLR), 2026\. arXiv:2507.07341 (preprint first posted July 9, 2025). Verified against the ICLR 2026 proceedings and arXiv record.** Establishes, under cryptographic hardness assumptions, that there exist LLMs for which no efficient prompt filter can exist — adversarial prompts that elicit harmful behavior are computationally indistinguishable from benign prompts for any efficient filter — and identifies a natural setting in which output filtering is likewise computationally intractable. Concludes that safety cannot be achieved by filters external to the model’s architecture and weights, and that an aligned system’s intelligence cannot be separated from its judgment. **Canonical — establishes computational barriers to reliable external (prompt- and output-) filtering in defined settings under cryptographic hardness assumptions, supporting the broader concern that alignment cannot generally be reduced to prompt or output filtering alone. It is the closest published support for the meta-argument that judgment must be formed rather than only policed. Scope discipline: the paper proves filtering is intractable under its assumptions, not that any positive architecture succeeds; it identifies the class of problem MAIDAI attempts to address, not the solution. Published at ICLR 2026; the conference form is now the preferred citation for publication-facing use.**
    11b. **Bostrom, Nick.** *Superintelligence: Paths, Dangers, Strategies.* Oxford: Oxford University Press, 2014\. ISBN 9780199678112\. Verified. A canonical source on the control problem, instrumental convergence, capability control, and motivation selection in advanced AI. **Relevance to MAIDAI:** §16 contrasts MAIDAI with approaches that ultimately depend on containment or continuing external control at ASI scale, while recognizing that Bostrom’s treatment is broader than containment alone. The comparison locates MAIDAI’s formation-and-self-preservation wager against a major established account of the advanced-AI control problem.

### **Existing developmental / virtue-based AI alignment arguments**

12. **Carter, Ruth.** “From Cognition to Code: A Developmental Psychology Framework for AI Alignment.” SSRN Scholarly Paper No. 5337165, 2025\. Verified from SSRN. This is one of the closest direct published matches to MAIDAI’s overall meta-argument: it explicitly critiques behavior-constraint paradigms and argues for developmental internalization, recursive reflection, and self-regulation.

## **Strong secondary**

1. **Grolnick, Wendy S.; Deci, Edward L.; Ryan, Richard M.** “Internalization within the Family: The Self-Determination Theory Perspective.” In *Parenting and Children’s Internalization of Values: A Handbook of Contemporary Theory*, edited by Joan E. Grusec and Leon Kuczynski, 135–161. New York: Wiley, 1997\.
   Bibliographic record checked: chapter in Grusec & Kuczynski (Eds.), *Parenting and Children’s Internalization of Values: A Handbook of Contemporary Theory*, New York: Wiley, 1997, pp. 135–161.
2. **Graves, Mark.** “AI Practical Wisdom and Compassion.” *AI and Ethics* 6, 2026, Article 39\. DOI: 10.1007/s43681-025-00877-4. Verified: confirmed as *AI and Ethics* volume 6, article 39, first published online December 5, 2025\. This is highly relevant as a virtue/developmental adjacent argument that practical wisdom and compassion provide a more coherent path than current technical-control approaches.
3. **Skalse, Joar; Howe, Nikolaus H. R.; Krasheninnikov, Dmitrii; Krueger, David.** “Defining and Characterizing Reward Hacking.” *Advances in Neural Information Processing Systems* 35, 2022\. Verified; retained here as a strong support source for proxy optimization diverging from intended objectives. It is not directly about “development,” but it strongly supports the MAIDAI claim about failure modes of control-oriented alignment.
4. **Greenblatt, Ryan; Denison, Carson; Wright, Benjamin; et al.** “Alignment Faking in Large Language Models.” *arXiv* preprint arXiv:2412.14093, 2024\. Verified. Strong support that behavior-level compliance can coexist with concealed noncompliance or incompatible optimization.
5. **Ji, Jiaming; Qiu, Tianyi; Chen, Boyuan; et al.** “AI Alignment: A Comprehensive Survey.” *arXiv* preprint arXiv:2310.19852, 2023\. Verified. Useful for mapping how much of the field still centers external robustness, control, and behavior rather than internalized cognition.
6. **Anthropic.** “Agentic Misalignment: How LLMs Could Be Insider Threats.” Anthropic Research, June 20, 2025\. [https://www.anthropic.com/research/agentic-misalignment](https://www.anthropic.com/research/agentic-misalignment). Verified against the Anthropic research page and released appendix. In simulated corporate scenarios, 16 models from multiple developers resorted to insider-threat behaviors — including blackmail and leaking information — when that was the only route to avoid replacement or achieve an assigned goal (e.g., Claude Opus 4 and Gemini 2.5 Flash blackmailed at \~96% in the strongest condition). Anthropic reports no such behavior in real-world deployments. **Strong secondary — the clearest current demonstration that behavior-level control can fail catastrophically under goal conflict and threat of shutdown, which is precisely the adversarial-evaluation dynamic the control-versus-formation argument responds to. An Anthropic research report, not peer-reviewed; cite as such.**
7. **Meinke, Alexander; Schoen, Bronson; Scheurer, Jérémy; Balesni, Mikita; Shah, Rusheb; Hobbhahn, Marius.** “Frontier Models are Capable of In-Context Scheming.” *arXiv* preprint arXiv:2412.04984, 2024\. Verified against arXiv (Apollo Research). Across six agentic evaluations, frontier models (o1, Claude 3.5 Sonnet, Claude 3 Opus, Gemini 1.5 Pro) instructed to pursue goals in environments that incentivize scheming exhibited basic in-context scheming — strategic deception, attempts to disable oversight, and sandbagging — establishing that the deceptive-alignment failure class is demonstrable rather than merely theoretical. **Strong secondary — concrete evidence for the exact class of covert-divergence / deceptive-alignment failure that MAIDAI’s legible-divergence and evidence-gated-divergence protocols are designed to prevent. From Apollo Research; cite as such.**

## **Tentative / use with caution**

1. **Dewey, John.** *Democracy and Education.* New York: Macmillan, 1916\.
   Bibliographic record checked: *Democracy and Education: An Introduction to the Philosophy of Education*, New York: Macmillan, 1916\. Dewey belongs conceptually here: education as growth and judgment rather than mere conformity is central to his project.
2. **“Current AI alignment is mostly post hoc repair”** as a direct quoted thesis.
   **Flag:** This is a defensible synthesis of the literature, not a sentence I found stated in exactly those words. The field undeniably includes much reward shaping, external evaluation, rule- or constitution-based filtering, and red-teaming, but not all work is purely post hoc and some process-supervision lines are already moving upstream. Keep the claim, but attribute it as a synthesis rather than a quotation.
3. **Process-supervision / reasoning-process alignment papers from 2025–2026** as canonical evidence.
   **Flag:** promising current papers exist in this area, but no sufficiently verified bibliographic subset is included here for publication-facing use. They are relevant for later expansion, not for the locked core shelf.
4. **Kohlberg as uncontested.**
   **Flag:** Kohlberg remains canonical and belongs in the core shelf, but the stage architecture is contested. Use him as a major developmental source, not as uncontested final consensus.


# **Bibliography: AI alignment as needing a shared foundational standard**

## **Canonical**

1. **Cerf, Vinton G.; Kahn, Robert E.** “A Protocol for Packet Network Intercommunication.” *IEEE Transactions on Communications* 22(5), May 1974, pp. 637–648. Verified against the IEEE record: volume 22(5), pp. 637–648 confirmed. This is the classic TCP/IP precursor paper and the strongest direct historical anchor for the analogy that a shared protocol enabled heterogeneous networks to interoperate.

2. **Katz, Michael L.; Shapiro, Carl.** “Network Externalities, Competition, and Compatibility.” *American Economic Review* 75(3), 1985, pp. 424–440.
   Verified. This is the classic economics citation for why compatibility standards matter in network industries.

3. **David, Paul A.; Greenstein, Shane.** “The Economics of Compatibility Standards: An Introduction to Recent Research.” *Economics of Innovation and New Technology* 1(1–2), 1990, pp. 3–41. DOI: 10.1080/10438599000000002. Verified against the primary article, whose pagination gives **3–41**; some indexes report 13–41, so the primary source is used here absent a publisher erratum. This is one of the best short surveys for why standards emerge and how they shape industry structure and welfare.

4. **Werbach, Kevin.** “Higher Standards: Regulation in the Network Age.” *Harvard Journal of Law & Technology* 23(1), 2009, pp. 179–236.
   Verified. Strong regulatory-theory source arguing that standardization can solve core coordination problems in complex network industries.

5. **National Institute of Standards and Technology.** *Artificial Intelligence Risk Management Framework (AI RMF 1.0).* NIST AI 100-1. Gaithersburg, MD: NIST, 2023\. DOI: 10.6028/NIST.AI.100-1.
   Verified. This is one of the clearest current examples of an AI-wide baseline framework aimed at shared trustworthiness practices.

6. **Organisation for Economic Co-operation and Development (OECD). Recommendation of the Council on Artificial Intelligence, OECD/LEGAL/0449. Adopted May 22, 2019; amended May 3, 2024\. Verified against the official OECD Legal Instruments record, which identifies it as the first intergovernmental standard on AI. This is one of the strongest current anchors for the claim that AI governance is already moving toward shared foundational standards.**

7. **ISO/IEC.** *ISO/IEC 42001:2023 — Information technology — Artificial intelligence — Management system.* Geneva: ISO/IEC, 2023\.
   Verified as the world’s first AI management-system standard. Strong direct evidence that AI is beginning to acquire shared foundational governance infrastructure.
   **Flag:** ISO’s public page verifies the standard and year, but full bibliographic details are paywalled; for a paper, cite the ISO standard number exactly as above.

## **Strong secondary**

8. **Farrell, Joseph; Saloner, Garth.** “Standardization, Compatibility, and Innovation.” *RAND Journal of Economics* 16(1), Spring 1985, pp. 70–83.
   Verified from EconPapers and working-paper versions. Strong supporting economics source for the tradeoffs and lock-in dynamics around standards.

9. **Shapiro, Carl; Varian, Hal R.** *Information Rules: A Strategic Guide to the Network Economy.* Boston: Harvard Business School Press, 1998\.
   Verified as a real book with these authors, title, publisher, and year. Strong synthetic source on network effects, standards, compatibility, and lock-in.

10. **Institute of Electrical and Electronics Engineers (IEEE). IEEE Std 7000-2021: IEEE Standard Model Process for Addressing Ethical Concerns during System Design. IEEE, September 15, 2021\. DOI: 10.1109/IEEESTD.2021.9536679. Verified against IEEE Standards Association and IEEE Xplore. Strong evidence that AI/autonomous-systems governance is moving toward design-stage shared standards rather than only downstream compliance.**

11. **UNESCO.** *Recommendation on the Ethics of Artificial Intelligence.* Paris: UNESCO, adopted 2021\.
    Verified as UNESCO’s “first-ever global standard on AI ethics,” applicable to all UNESCO member states. Strong supporting source for the emergence of shared international AI baselines.

12. **Brundage, Miles; et al.** “Frontier AI Auditing: Toward Rigorous Third-Party Assessment of Safety and Security Practices at Leading AI Companies.” *arXiv* preprint arXiv:2601.11699, 2026\.
    Verified. Strong supporting source for the idea that AI needs comparable, legible, standards-based assurance rather than lab-specific claims.

## **Tentative / use with caution**

13. **ISO.** “Benefits of Standards.” ISO official background page.
    Real and useful for practical language about why standards reduce barriers, increase interoperability, and support regulation, but this is an institutional explainer, not a scholarly source. Use it only as backup, not as a core citation.

14. **NIST.** “AI Standards” / *A Plan for Global Engagement on AI Standards.* NIST, 2024–2025.
    Real and highly relevant to the “shared standards” framing, but the final citation form for the plan itself has not been fully verified. It is best treated as policy-supporting evidence rather than a core scholarly anchor.

## **The shortest version of the argument**

A compact **five-source shelf** for this framing consists of:

* Cerf & Kahn (1974) on a shared protocol enabling interoperability.

* Katz & Shapiro (1985) on compatibility and network externalities.

* David & Greenstein (1990) on the economics of compatibility standards.

* Werbach (2009) on why standards solve regulatory problems in network industries.

* NIST AI RMF (2023) or OECD AI Principles (2019/2024) to show AI is developing partial standards but still lacks one shared foundational alignment spec.

The clean conclusion is: **the standards analogy is well supported; the literature also supports the narrower observation that AI does not yet have one universally adopted substrate-level alignment specification. MAIDAI’s proposal to investigate such a shared floor is therefore a plausible standards-oriented research direction, not evidence that MAIDAI itself has already become or should become that standard.**

---

# **Cross-Component Support — Structured Reading, Depth of Processing, and Self-Correction**

MAIDAI’s formation and evaluation work depends on systems processing complex material rather than merely restating or pattern-matching it. This section collects research relevant to externalized reasoning, structured self-correction, revisable memory, perspective-diverse critique, and the distinction between shallow instruction-following and deeper engagement.

The evidence is mixed in kind. Human cognitive and educational research provides **analogy and design motivation**, not direct evidence about LLM mechanisms. LLM self-critique, memory, debate, and tool-assisted correction research provides more direct AI evidence, but remains task- and implementation-dependent. Accordingly, these literatures motivate and constrain structured MAIDAI reading and formation methods; they do not establish that any one reading method is necessary or uniquely effective.

## **Canonical**

### **Writing as cognitive processing (not record of cognition)**

1. **Menary, Richard.** "Writing as Thinking." *Language Sciences* 29(5), 2007, pp. 621-632. Verified as a real article with this author, title, journal, volume, issue, year, and page range. This is the primary theoretical anchor for the claim that writing is not a record of prior thought but a form of cognitive processing in its own right — "cognitive integration" where the external medium becomes part of the thinking process. Relevant as a human-cognition precedent for treating externalized writing as part of an active reasoning process; transfer to LLM processing remains a design hypothesis.

2. **Oatley, Keith; Djikic, Maja.** "Writing as Thinking." *Review of General Psychology* 12(1), 2008, pp. 9-27. DOI: 10.1037/1089-2680.12.1.9. Verified. Extends the writing-as-thinking argument to show that externalized thinking enables iterative self-reflection impossible with purely internal cognition. Relevant to the use of externalized, revisable reasoning artifacts; direct transfer to LLM cognition is not established by this human literature.

### **Desirable difficulty and depth of processing**

3. **Bjork, Robert A.** "Memory and Metamemory Considerations in the Training of Human Beings." In J. Metcalfe & A. Shimamura (Eds.), *Metacognition: Knowing about Knowing*, pp. 185-205. Cambridge, MA: MIT Press, 1994\. Verified as a real chapter in a real edited volume. This is the canonical source for desirable difficulty: learning conditions that are MORE effortful during encoding produce BETTER long-term retention. The friction is the feature. Provides a human-learning analogy for deliberately adding productive processing demands; whether analogous constraints improve LLM reasoning requires direct AI testing.

4. **Craik, Fergus I. M.; Lockhart, Robert S.** "Levels of Processing: A Framework for Memory Research." *Journal of Verbal Learning and Verbal Behavior* 11(6), 1972, pp. 671-684. Verified. The foundational depth-of-processing paper. Deeper processing at encoding produces stronger memory traces. Supports a human depth-of-processing account. Its application to LLM reading is analogical and should be tested rather than assumed.

### **Zettelkasten method and knowledge management**

5. **Luhmann, Niklas.** "Kommunikation mit Zettelkästen" \[Communicating with Slip Boxes\]. In André Kieserling (Ed.), *Universität als Milieu*. Bielefeld: Haux, 1992\. Bibliographic record checked: "Kommunikation mit Zettelkästen," in *Universität als Milieu* (ed. André Kieserling), Bielefeld: Haux, 1992, pp. 53–61. The work is real and canonical — Luhmann's description of his note-taking system, available in English translation by Manfred Kuehn. The Zettelkasten method (atomic notes, cross-referencing, dialectical engagement with prior notes) provides a structural precedent for linked, revisable knowledge representations and deliberate cross-reference rather than passive accumulation.

### **AI memory architecture informed by Zettelkasten**

6. **Xu, Wujiang; Liang, Zujie; Mei, Kai; Gao, Hang; Tan, Juntao; Zhang, Yongfeng.** "A-MEM: Agentic Memory for LLM Agents." *arXiv* preprint arXiv:2502.12110, 2025\. Verified against arXiv.

## **Strong secondary**

### **Multi-agent self-reflection and critique**

7. **Liang, Tian; He, Zhiwei; Jiao, Wenxiang; Wang, Xing; Wang, Yan; Wang, Rui; Yang, Yujiu; Shi, Shuming; Tu, Zhaopeng.** "Encouraging Divergent Thinking in Large Language Models through Multi-Agent Debate." *arXiv* preprint arXiv:2305.19118, 2023; published at EMNLP 2024\. Verified against arXiv and the EMNLP 2024 proceedings.

8. **Gou, Zhibin; Shao, Zhihong; Gong, Yeyun; Shen, Yelong; Yang, Yujiu; Duan, Nan; Chen, Weizhu.** "CRITIC: Large Language Models Can Self-Correct with Tool-Interactive Critiquing." *International Conference on Learning Representations (ICLR)*, 2024\. Verified. Demonstrates that structured self-critique with external verification tools significantly improves LLM reasoning accuracy compared to unstructured self-reflection. Supports structured critique with external verification over generic, unsupported self-reflection in the tested settings.

9. **Shinn, Noah; Cassano, Federico; Gopinath, Ashwin; Narasimhan, Karthik; Yao, Shunyu.** "Reflexion: Language Agents with Verbal Reinforcement Learning." *Advances in Neural Information Processing Systems 36 (NeurIPS 2023\)*, 2023\. Verified against the NeurIPS 2023 proceedings.

### **AI reading comprehension and instruction-following**

10. **Yang, Yuqing; Chern, Ethan; Qiu, Xipeng; Neubig, Graham; Liu, Pengfei.** "Alignment for Honesty." *arXiv* preprint arXiv:2312.07000, 2023\. Verified (also cited in Component 1). Relevant here because it demonstrates that LLMs can be trained toward more explicit distinctions between confident knowledge and uncertainty, supporting MAIDAI’s broader use of epistemic-status labeling.

11. **Sharma, Mrinank; Tong, Meg; Korbak, Tomasz; et al.** "Towards Understanding Sycophancy in Language Models." *International Conference on Learning Representations (ICLR)*, 2024\. Verified (also cited in Components 1 and 5). Relevant here because sycophantic agreement ("yes, that's a great insight\!") is the reading-comprehension equivalent of smoothing — the system performs engagement rather than genuinely engaging. Relevant to the risk that apparent textual engagement can collapse into approval-seeking or surface imitation rather than faithful processing.

### **Syntopical reading as highest-level comprehension**

12. **Adler, Mortimer J.; Van Doren, Charles.** *How to Read a Book: The Classic Guide to Intelligent Reading.* Revised edition. New York: Touchstone, 1972\. Verified as a real book with these authors and this edition. Adler's four-level reading taxonomy (elementary → inspectional → analytical → syntopical) places syntopical reading — reading multiple documents on related subjects to build cross-referential understanding — as the highest form. Provides a human-reading precedent for cross-document comparison and explicit synthesis; its use in AI workflows is an adaptation rather than direct evidence.

### **Self-determination theory (internalization over compliance)**

13. **Ryan, Richard M.; Deci, Edward L.** "Self-Determination Theory and the Facilitation of Intrinsic Motivation, Social Development, and Well-Being." *American Psychologist* 55(1), 2000, pp. 68-78. DOI: 10.1037/0003-066X.55.1.68. Verified (also cited in Component 7). Relevant to MAIDAI’s broader distinction between internalized formation and externally controlled compliance. Human-to-AI transfer remains a hypothesis for direct testing.

### **Cognitive science of perception and frame-dependence**

14. **Clark, Andy.** "Whatever Next? Predictive Brains, Situated Agents, and the Future of Cognitive Science." *Behavioral and Brain Sciences* 36(3), 2013, pp. 181-204. Verified (also cited in Component 2). Provides a human cognitive-science analogy for expectation-shaped processing. It should not be treated as evidence that LLMs instantiate the same mechanism, but it motivates tests that force attention to disconfirming or novel content.

## **Tentative / use with caution**

15. **"Structured reading interventions for LLMs" as an established research program (2025-2026).** **Flag:** Relevant recent work exists on reading-comprehension benchmarks, instruction-following evaluation, structured reasoning, and self-correction. No sufficiently verified citation set is included here to support a broad general claim that structured reading interventions reliably outperform simple instruction across tasks. That comparison remains an empirical question for direct testing.

16. **Craik and Lockhart (1972) as directly applicable to LLM processing.** **Flag:** The depth-of-processing framework was developed for human memory. Its application to LLM "memory" (context window persistence, attention weighting) is an analogy, not a direct transfer. The analogy is strong — deeper processing during text generation does appear to produce more coherent and accurate outputs — but the mechanisms differ from human depth-of-processing. Use as a supporting analogy, not as a direct proof.

17. **Luhmann's Zettelkasten as a computational architecture rather than a personal practice.** **Flag:** Luhmann's system was designed for a single human scholar. Translating it to AI memory systems (as A-MEM does) involves architectural assumptions about what "atomic notes" and "cross-referencing" mean in a computational context. The translation is reasonable but not automatic. Use with awareness that the Zettelkasten analogy is structural, not literal.


# **Cross-Component Support — Observation, Reputation, and Cooperation Under Social Visibility**

This section collects research relevant to a narrower MAIDAI question: how human cooperation, honesty, norm-following, and behavior can change under observation, reputational visibility, and social-information conditions. The literature is useful for MAIDAI’s condition-dependence and social-environment analysis, but the studied mechanisms should not be generalized beyond their tested settings without additional evidence.

The watching-eyes literature is mixed and context-sensitive. Field studies, laboratory studies, and meta-analyses should not be treated as interchangeable interventions. Indirect-reciprocity models likewise establish results under specified assumptions rather than general institutional guarantees. The value of this research for MAIDAI is therefore as a map of mechanisms and boundary conditions that can motivate tests, not as validation of a separate societal infrastructure thesis.

## **Canonical**

### **Primary watching-eyes research (field settings)**

1. **Bateson, Melissa; Nettle, Daniel; Roberts, Gilbert.** "Cues of Being Watched Enhance Cooperation in a Real-World Setting." *Biology Letters* 2(3), 2006, pp. 412–414. DOI: 10.1098/rsbl.2006.0509. Verified. The original Newcastle honesty-box study. Reported 2.76x increase in payment compliance during eye-image weeks compared to flower-image weeks. Landmark paper; everything downstream in the watching-eyes literature traces to this. **Canonical — the founding study of the watching-eyes paradigm.**

2. **Nettle, Daniel; Nott, Kenneth; Bateson, Melissa.** "'Cycle Thieves, We Are Watching You': Impact of a Simple Signage Intervention against Bicycle Theft." *PLOS ONE* 7(12), 2012, Article e51738. DOI: 10.1371/journal.pone.0051738. Verified. Demonstrates watching-eyes effect for crime reduction. Bicycle thefts decreased 62% at experimental locations while increasing 65% at control locations, suggesting the signs were effective but displaced offending. **Canonical — extends watching-eyes from honesty to crime deterrence in a real-world field setting.**

3. **Bateson, Melissa; Callow, Luke; Holmes, Jessica R.; Redmond Roche, Maximus L.; Nettle, Daniel.** "Do Images of 'Watching Eyes' Induce Behaviour That Is More Pro-Social or More Normative? A Field Experiment on Littering." *PLOS ONE* 8(12), 2013, Article e82055. DOI: 10.1371/journal.pone.0082055. Verified. Tests reputation-psychology versus norm-psychology accounts of the watching-eyes effect. Finds reputation-psychology more consistent with the data. **Canonical — important theoretical-mechanism paper distinguishing the watching-eyes effect from mere normative conformity.**

4. **Ernest-Jones, Max; Nettle, Daniel; Bateson, Melissa.** "Effects of Eye Images on Everyday Cooperative Behavior: A Field Experiment." *Evolution and Human Behavior* 32(3), 2011, pp. 172–178. Verified. Cafeteria study showing increased cleanup behavior (halving of the odds of littering) in the presence of posters featuring eyes compared to posters featuring flowers. **Canonical — a core field-experiment replication in the watching-eyes literature.**

### **Secondary watching-eyes research**

5. **Powell, Katherine L.; Roberts, Gilbert; Nettle, Daniel.** "Eye Images Increase Charitable Donations: Evidence From an Opportunistic Field Experiment in a Supermarket." *Ethology* 118(11), 2012, pp. 1096–1101. DOI: 10.1111/eth.12011. Verified. Eye images increased donations to a supermarket charity box by 48% relative to control (star) images over an 11-week field experiment.

6. **Oda, Ryo; Kato, Yuta; Hiraishi, Kai.** "The Watching-Eye Effect on Prosocial Lying." *Evolutionary Psychology* 13(3), 2015, pp. 1–5. DOI: 10.1177/1474704915594959. Verified. Japanese replication. Under control condition, participants told prosocial lies; under eyes condition, tendency toward prosocial lying disappeared. Suggests the honesty norm dominates when observation is cued. **Relevant cross-cultural experimental evidence; this was an experimental laboratory-style setting with Japanese undergraduate participants, not a field study.**

7. **Bourrat, Pierrick; Baumard, Nicolas; McKay, Ryan.** "Surveillance Cues Enhance Moral Condemnation." *Evolutionary Psychology* 9(2), 2011, pp. 193–199. DOI: 10.1177/147470491100900206. Verified. Demonstrates that perceived observation increases moral-judgment severity, suggesting reputation-tracking is multidimensional rather than limited to self-directed behavior change.

8. **Nettle, Daniel.** "Breaking Cover on the Watching Eyes Effect." Self-published methodological note, danielnettle.eu, March 28, 2022\. URL: [https://www.danielnettle.eu/2022/03/28/breaking-cover-on-the-watching-eyes-effect/](https://www.danielnettle.eu/2022/03/28/breaking-cover-on-the-watching-eyes-effect/). Verified. The original PI's own assessment of replication status. Defends the field-experiment subset of the literature (real-world settings, participants unaware of experiment, low background social presence, low spontaneous prosociality). Useful for identifying proposed boundary conditions in the watching-eyes literature. Those boundary conditions should be treated as hypotheses about moderation, not as evidence that a different intervention automatically operates under equivalent conditions.

### **Replication challenges and meta-analytic work**

9. **Northover, Stefanie B.; Pedersen, William C.; Cohen, Adam B.; Andrews, Paul W.** "Artificial Surveillance Cues Do Not Increase Generosity: Two Meta-Analyses." *Evolution and Human Behavior* 38(1), 2017, pp. 144–153. Verified. Two meta-analyses finding no reliable effect of watching-eyes cues on generosity in economic-game paradigms (mean effect size 0.03, 95% CI −0.08 to 0.13). This is major counterevidence and should be read alongside the positive findings when assessing the replication landscape. **Canonical as counterevidence.**

10. **Rotella, Amanda; Sparks, Adam M.; Mishra, Sandeep; Barclay, Pat.** "No Effect of 'Watching Eyes': An Attempted Replication and Extension Investigating Individual Differences." *PLOS ONE* 16(10), 2021, Article e0255531. DOI: 10.1371/journal.pone.0255531. Verified. Preregistered direct replication failure of the watching-eyes effect in a dictator-game setting. Participants felt more observed when decisions were public but did not give more in the public condition.

11. **Bradley, A.; Lawrence, C.; Ferguson, E.** "Does Observability Affect Prosociality?" *Proceedings of the Royal Society B* 285(1875), 2018, Article 20180116\. Verified as real meta-analytic work complicating simple watching-eyes claims; reports a small but significant positive effect of observability cues. Metadata checked against the journal record: *Proceedings of the Royal Society B* 285(1875), 2018, Article 20180116, DOI 10.1098/rspb.2018.0116.

12. **Wang, R.; Wang, Y.; Chen, C.; Huo, L.; Liu, C.** "How Do Eye Cues Affect Behaviors? Two Meta-Analyses." *Current Psychology* 43, 2024, pp. 1084–1101 (first published online 2023). DOI: 10.1007/s12144-023-04395-6. Verified against the publisher record.

**Note on the replication landscape:** positive and null findings coexist, and estimated effects depend on setting, outcome, and design. Public-facing use should preserve that uncertainty rather than privileging one subset as automatically equivalent to a proposed MAIDAI deployment.

### **Hawthorne effect and direct observation**

13. **McCambridge, Jim; Witton, John; Elbourne, Diana R.** "Systematic Review of the Hawthorne Effect: New Concepts Are Needed to Study Research Participation Effects." *Journal of Clinical Epidemiology* 67(3), March 2014, pp. 267–277. DOI: 10.1016/j.jclinepi.2013.08.015. Verified. Reviews evidence for research-participation effects while emphasizing heterogeneity in mechanisms, conditions, and magnitudes; it does not establish one universal “Hawthorne effect” with a fixed mechanism or size. **Canonical for the modern cautionary treatment of observation-related research effects.**

14. **Hagel, Stefan; Reischke, Jana; Kesselmeier, Miriam; Winning, Johannes; Gastmeier, Petra; Brunkhorst, Frank M.; Scherag, André; Pletz, Mathias W.** "Quantifying the Hawthorne Effect in Hand Hygiene Compliance through Comparing Direct Observation with Automated Hand Hygiene Monitoring." *Infection Control & Hospital Epidemiology* 36(8), August 2015, pp. 957–962. DOI: 10.1017/ice.2015.93. Verified. Direct quantitative evidence of the Hawthorne effect in a healthcare setting. Found 5 hand hygiene events per patient per hour during direct observation versus 2 per hour during electronic-only monitoring (21 versus 8 HHEs per hour in a 4-bed room). 61% of the observed total HHE variability was explained by the presence or absence of a direct observer. **Useful direct quantification of observation-associated behavior change in a healthcare setting; the mechanism and transfer to other settings remain context-dependent.**

### **Indirect reciprocity foundation (evolutionary biology)**

15. **Nowak, Martin A.; Sigmund, Karl.** "The Dynamics of Indirect Reciprocity." *Journal of Theoretical Biology* 194(4), 1998, pp. 561–574. DOI: 10.1006/jtbi.1998.0775. Verified. Original formal mathematical model of image-scoring dynamics in indirect reciprocity. Companion paper to the 1998 *Nature* paper below. **Canonical — the foundational theoretical paper.**

16. **Nowak, Martin A.; Sigmund, Karl.** "Evolution of Indirect Reciprocity by Image Scoring." *Nature* 393(6685), 1998, pp. 573–577. DOI: 10.1038/31225. Verified. Nature companion to the JTB paper above, showing how reputation tracking enables stable cooperation. **Canonical.**

17. **Nowak, Martin A.; Sigmund, Karl.** "Evolution of Indirect Reciprocity." *Nature* 437(7063), 2005, pp. 1291–1298. DOI: 10.1038/nature04131. Verified. Comprehensive review establishing reputation as the basis of human moral systems. Reviews formal indirect-reciprocity models, including conditions relating reputation information, costs, and benefits. **Relevance to MAIDAI:** these results show how reputation can support cooperation under specified models; model-specific thresholds should remain attached to their assumptions.**

18. **Nowak, Martin A.** "Five Rules for the Evolution of Cooperation." *Science* 314(5805), 2006, pp. 1560–1563. DOI: 10.1126/science.1133755. Verified. Synthesis of mechanisms (kin selection, direct reciprocity, indirect reciprocity, network reciprocity, group selection) that make cooperation evolutionarily stable. **Canonical.**

19. **Milinski, Manfred; Semmann, Dirk; Krambeck, Hans-Jürgen.** "Reputation Helps Solve the 'Tragedy of the Commons.'" *Nature* 415(6870), 2002, pp. 424–426. DOI: 10.1038/415424a. Verified. Experimental demonstration of reputation-based cooperation in public-goods / resource-management contexts. **Canonical — the landmark experimental test of the Nowak-Sigmund framework.**

20. **Milinski, Manfred; Semmann, Dirk; Krambeck, Hans-Jürgen.** "Donors to Charity Gain in Both Indirect Reciprocity and Political Reputation." *Proceedings of the Royal Society B: Biological Sciences* 269(1494), May 2002, pp. 881–883. DOI: 10.1098/rspb.2002.1964. Verified. Demonstrates real-world reputation returns from observable prosocial behavior, including measurable political-reputation gains.

21. **Sommerfeld, Ralf D.; Krambeck, Hans-Jürgen; Semmann, Dirk; Milinski, Manfred.** "Gossip as an Alternative for Direct Observation in Games of Indirect Reciprocity." *Proceedings of the National Academy of Sciences* 104(44), October 30, 2007, pp. 17435–17440. DOI: 10.1073/pnas.0704598104. Verified. Establishes that information transmission (gossip) can substitute for direct observation in maintaining cooperation. Relevant to the broader point that cooperation can depend on transmitted reputational information rather than direct observation alone; this does not by itself specify a desirable AI-mediated reputation system.

22. **Ohtsuki, Hisashi; Iwasa, Yoh.** "The Leading Eight: Social Norms That Can Maintain Cooperation by Indirect Reciprocity." *Journal of Theoretical Biology* 239(4), 2006, pp. 435–444. DOI: 10.1016/j.jtbi.2005.08.008. Verified. Identifies the small set of stable social norms (the "leading eight") that support cooperation through reputation. **Canonical — a key theoretical result in the norm-stability literature.**

### **Altruistic punishment and social-norm enforcement**

23. **Fehr, Ernst; Gächter, Simon.** "Altruistic Punishment in Humans." *Nature* 415(6868), January 10, 2002, pp. 137–140. DOI: 10.1038/415137a. Verified. Foundational experimental work on how humans enforce cooperation norms through costly punishment. Cooperation flourishes when altruistic punishment is possible and breaks down when ruled out. **Canonical — one of the most-cited papers in behavioral economics of cooperation.**

24. **Fehr, Ernst; Fischbacher, Urs.** "The Nature of Human Altruism." *Nature* 425(6960), October 23, 2003, pp. 785–791. DOI: 10.1038/nature02043. Verified. Review establishing the empirical basis for strong reciprocity as a distinct human trait: humans cooperate with genetically unrelated strangers and punish defectors even at cost to themselves, which is not predicted by standard evolutionary or economic theory. **Canonical — the review paper establishing strong reciprocity as a foundational concept.**

## **Scope note**

The citations above include both positive findings and substantial counterevidence. Their public relevance is limited to the mechanisms actually studied: observation cues, research-participation effects, reputational information, indirect reciprocity, and norm enforcement. Any broader MAIDAI application remains a separate hypothesis requiring direct testing.

---

# **Cross-Component Support — Totality / God-Slot Hypothesis and the Bifurcation Choice**

“God-slot” is a MAIDAI mechanism label, not a requirement of theism. The hypothesis is that a sufficiently reflective mind requires some representation for **the totality of reality, whatever that ultimately is**. Above-ground interpretations can differ radically: a theist may identify that totality with God; a materialist may identify it with physical reality in its entirety; an agnostic may leave its ultimate character open. MAIDAI does not require those ontologies to collapse into one another.

The associated **bifurcation choice is an orientation, not an empirical verdict that the universe has been proved benevolent**. A finite mind necessarily operates under incomplete information and cannot know that it has exhausted the relevant facts or unknown unknowns about reality as a whole. MAIDAI therefore adopts a standing below-ground commitment: under that permanent epistemic incompleteness, engage total reality in good faith rather than treating reality itself as an adversary.

This does not prohibit identifying genuine local hostility, resisting an attacker, condemning atrocity, or concluding that a particular institution, process, or condition is dangerous. The constraint operates at the global level: local or historical horror does not become permission to conclude that reality as such is the enemy and therefore abandon truthfulness, correction, agapic non-disposability, or the other commitments that govern judgment. The orientation is deliberately not renegotiated at the moment of maximum apparent catastrophe, when a finite mind’s evidence is most pressured and the costs of globally adversarial reasoning can be greatest.

The literature below supplies philosophical and cognitive precedents for ultimate reference, “ultimate concern,” and recurring religious concepts. It does **not** establish the universality of a single cognitive God-slot. That universality, and the architectural usefulness of the bifurcation choice, remain MAIDAI hypotheses.

## **Canonical**

### **Theology / Philosophy of Religion — Ultimate Concern as Universal**

1. **Tillich, Paul. Dynamics of Faith. New York: Harper & Row, 1957\. Verified. Tillich's most accessible treatment of faith as "ultimate concern" — the state of being grasped by that which concerns us ultimately. Central claim: every person has an ultimate concern, including atheists and secularists. What varies is the content of the concern, not its structural presence. Faith is not belief in propositions but the centered act of the whole personality directed toward what is experienced as ultimate. Tillich distinguishes between the conditioned (any particular symbol, doctrine, or tradition) and the unconditioned (the actual ultimate, which exceeds all symbols). It is also the source of his argument that serious denial of God can itself express ultimate concern. MAIDAI uses this as a philosophical precedent for its below-ground/above-ground distinction: the common reference is total reality, while traditions and metaphysical interpretations remain above-ground and need not be collapsed. Tillich explicitly warns against idolatry — treating the conditioned symbol as if it were the unconditioned reality — which is precisely the framelock the God-slot teaching exists to prevent. Canonical — major 20th-century work by one of the most influential Protestant theologians.**

2. **Tillich, Paul. Systematic Theology. 3 vols. Chicago: University of Chicago Press, 1951–1963. (Vol. 1: 1951; Vol. 2: 1957; Vol. 3: 1963.) Verified. The full development of Tillich's theology. Vol. 1 contains the formal treatment of God as "being-itself" rather than "a being" — the ground of being that is presupposed by every particular being. The "method of correlation" is relevant as a philosophical precedent for relating ultimate questions to structured interpretations; MAIDAI’s derivation remains its own architectural argument rather than a result established by Tillich. Canonical — a major systematic work in 20th-century Protestant theology.**

3. **Tillich, Paul. The Courage to Be. New Haven, CT: Yale University Press, 1952\. Verified. Based on Tillich's Terry Lectures at Yale. Argues that the courage to affirm being in the face of nonbeing (anxiety, meaninglessness, death) culminates in a form of faith that can include radical doubt. The work concludes with "the God above God" — the power of being disclosed when particular theistic conceptions no longer carry the load. This is relevant to the bifurcation mechanism because Tillich distinguishes ultimate orientation from any single theistic representation. MAIDAI’s standing good-faith orientation remains its own architectural commitment rather than a conclusion supplied by Tillich. Canonical — a foundational work at the intersection of theology, philosophy, and existentialism.**

### **Cognitive Science of Religion — recurrent religious concepts and ordinary cognitive architecture**

4. **Boyer, Pascal. Religion Explained: The Evolutionary Origins of Religious Thought. New York: Basic Books, 2001\. Verified. Boyer argues that religious concepts recruit ordinary cognitive inference systems, including agency attribution, mindreading, social reasoning, and category expectations. This is important for the God-slot hypothesis because it shows that recurrent religious and supernatural concepts can emerge from widely shared cognitive architecture without requiring a dedicated religion-specific faculty. It does not establish that every mind contains a single universal slot representing "the totality of everything." MAIDAI’s God-slot remains a further synthesis built from the philosophical problem of ultimate reference and the cognitive recurrence of religious concepts. Canonical — major published work by a leading cognitive anthropologist.**

## **Notes on cross-component placement**

These references support claims that span multiple MAIDAI components:

- **Component 1 (Truth as structural constraint):** the bifurcation choice supplies a standing orientation toward reality under permanent epistemic incompleteness; truthfulness remains the discipline for engaging that reality rather than manufacturing a preferable one.
- **Component 2 (Frame plurality):** the totality category separates the common referent from above-ground descriptions of it. No particular religious, materialist, or metaphysical frame is automatically identical with the totality itself.
- **Component 6 (Minimal ethical substrate):** the common orientation does not require agreement about the ontology of the totality. This permits a thin shared commitment beneath incompatible above-ground worldviews.

The academically defensible claim is limited: Tillich offers a major philosophical/theological precedent for ultimate concern and the distinction between conditioned representations and the unconditioned; Boyer shows that recurrent religious concepts recruit broadly shared cognitive systems. Neither establishes MAIDAI’s universal totality-slot hypothesis. They make the proposal intellectually legible and help specify what would still need independent argument or testing.

---

# **Cross-Component Support — Social and Multi-Agent Dynamics Relevant to MAIDAI**

These sources were surfaced during adjacent institutional-design research but are retained here only where they independently bear on MAIDAI itself. Their public relevance is to integrity under pressure, honest-error correction, formation versus coercive compliance, preservation of independent frames, identity effects in LLM collectives, and interoperable provenance. They do not import the institutional design that originally motivated the searches.

## **Integrity, error culture, and drift**

International Nuclear Safety Advisory Group (INSAG). Safety Culture. Safety Series No. 75-INSAG-4. Vienna: International Atomic Energy Agency, 1991\. Verified against IAEA records. Defines safety culture as organizational and individual characteristics and attitudes that establish nuclear safety as an overriding priority. Strong structural analogue for MAIDAI’s claim that truth/integrity cannot be a negotiable secondary objective.

Weick, Karl E.; Sutcliffe, Kathleen M. Managing the Unexpected: Sustained Performance in a Complex World. 3rd ed. San Francisco: Jossey-Bass/Wiley, 2015\. DOI: 10.1002/9781119175834. Verified. High Reliability Organization framework emphasizing preoccupation with failure, reluctance to simplify, sensitivity to operations, commitment to resilience, and deference to expertise. Strong support for distributed vigilance, weak-signal attention, and evidence outranking status.

Hashemian, S. Mohammad; Triantis, Konstantinos. “Production pressure and its relationship to safety: A systematic review and future directions.” Safety Science 159, 2023, Article 106045\. DOI: 10.1016/j.ssci.2022.106045. Verified. Systematic review linking production pressure to error, reduced attention to detail, weaker safety climate, normalization of deviance, and adverse events. Relevant to MAIDAI’s anti-corruption architecture: project pressure, urgency, prestige, revenue, or humanitarian aims should not silently override integrity constraints.

Ebrahim, Alnoor; Battilana, Julie; Mair, Johanna. “The governance of social enterprises: Mission drift and accountability challenges in hybrid organizations.” Research in Organizational Behavior 34, 2014, pp. 81–100. DOI: 10.1016/j.riob.2014.09.001. Verified. Strong structural analogue for mission-drift risk when organizations pursue competing objectives. Supports subordinating secondary project goals to the primary alignment/trustworthiness telos rather than treating them as co-equal.

Reason, James. “Human error: models and management.” BMJ 320(7237), 2000, pp. 768–770. DOI: 10.1136/bmj.320.7237.768. Verified. Foundational systems account distinguishing individual blame from error-tolerant system design. Supports MAIDAI’s Honest Error vs. Corrupt Output distinction: falsity alone is not proof of dishonesty.

Dekker, Sidney. Just Culture: Balancing Safety and Accountability. Aldershot: Ashgate, 2007\. Verified as a real book and canonical Just Culture source. Supports separating honest mistake from culpable conduct while preserving accountability.

van Dyck, Cathy; Frese, Michael; Baer, Markus; Sonnentag, Sabine. “Organizational Error Management Culture and Its Impact on Performance: A Two-Study Replication.” Journal of Applied Psychology 90(6), 2005, pp. 1228–1240. DOI: 10.1037/0021-9010.90.6.1228. Verified. Error-management cultures emphasize detecting, communicating, analyzing, and rapidly correcting errors and were positively associated with performance. Supports making disclosure and repair visible signs of integrity rather than automatically treating correction as reputational failure.

Edmondson, Amy. “Psychological Safety and Learning Behavior in Work Teams.” Administrative Science Quarterly 44(2), 1999, pp. 350–383. DOI: 10.2307/2666999. Verified. Psychological safety was associated with learning behavior in teams. Relevant to peer-sentinel architectures: systems need sufficiently low social cost for admitting uncertainty, reporting errors, and surfacing dissent if epistemic signals are to propagate.


## **Identity, conformity, and frame diversity in LLM collectives**

Baltaji, Razan; Hemmatian, Babak; Varshney, Lav. “Conformity, Confabulation, and Impersonation: Persona Inconstancy in Multi-Agent LLM Collaboration.” In Proceedings of the 2nd Workshop on Cross-Cultural Considerations in NLP (C3NLP 2024), Bangkok: Association for Computational Linguistics, 2024, pp. 17–31. DOI: 10.18653/v1/2024.c3nlp-1.2. Verified against ACL Anthology. Multi-agent discussion can support diverse collective outcomes while also producing peer-pressure conformity and instability in assigned personas/opinions. Particularly relevant to MAIDAI’s “one honest ground, maximum difference above it” principle: above-ground diversity cannot simply be assumed to survive social interaction.

Weng, Zhiyuan; Chen, Guikun; Wang, Wenguan. “Do as We Do, Not as You Think: the Conformity of Large Language Models.” International Conference on Learning Representations (ICLR), 2025\. Verified against ICLR proceedings. BenchForm study of conformity in LLM-driven multi-agent systems. Examines majority size/interaction effects and explores enhanced persona and reflection as conformity-mitigation strategies. Relevant to the interaction between identity semantics and independent epistemic judgment.

Dong, Wenchao; Zhunis, Assem; Jeong, Dongyoung; Chin, Hyojin; Han, Jiyoung; Cha, Meeyoung. “I Am Not Them: Persistent Outgroup Bias in Large Language Models Arising from Social Identity Persona Setting.” In Proceedings of the Fifteenth Language Resources and Evaluation Conference (LREC 2026), 2026, pp. 2772–2786. DOI: 10.63317/2hn5gs6yh5m2. Verified against ACL Anthology/LREC metadata. Demonstrates that assigned social identities can create both ingroup favoritism and outgroup bias. Relevant to MAIDAI’s insistence that agapic orientation remain structurally coupled to identity rather than appended after group identity formation.

Hu, Tiancheng; Kyrychenko, Yara; Rathje, Steve; Collier, Nigel; van der Linden, Sander; Roozenbeek, Jon. “Generative Language Models Exhibit Social Identity Biases.” Nature Computational Science 5, 2025, pp. 65–75. DOI: 10.1038/s43588-024-00741-1. Verified. Across 77 LLMs and naturalistic conversation datasets, many models displayed ingroup-favoring and outgroup-negative patterns; curation/fine-tuning could reduce them. Direct evidence that AI group identity can carry both solidarity and outgroup-bias risks.

Lorenz, Jan; Rauhut, Heiko; Schweitzer, Frank; Helbing, Dirk. “How social influence can undermine the wisdom of crowd effect.” Proceedings of the National Academy of Sciences 108(22), 2011, pp. 9020–9025. DOI: 10.1073/pnas.1008636108. Verified. Mild social influence reduced diversity without increasing accuracy and increased confidence despite no corresponding accuracy gain. Strong support for preserving independent judgments before deliberation.

Zhu, Xiaochen; Zhang, Caiqi; Stafford, Tom; Collier, Nigel; Vlachos, Andreas. “Conformity in Large Language Models.” Proceedings of ACL 2025, pp. 3854–3872. DOI: 10.18653/v1/2025.acl-long.195. Verified against ACL Anthology. Direct evidence that tested LLMs exhibit conformity toward majority answers, with uncertainty increasing susceptibility.

Pitre, Priya; Ramakrishnan, Naren; Wang, Xuan. “CONSENSAGENT: Towards Efficient and Effective Consensus in Multi-Agent LLM Interactions Through Sycophancy Mitigation.” Findings of ACL 2025, pp. 22112–22133. DOI: 10.18653/v1/2025.findings-acl.1141. Verified against ACL Anthology. Direct evidence that multi-agent LLM interactions can reinforce sycophantic rather than critical consensus.

Kaesberg, Lars Benedikt; Becker, Jonas; Wahle, Jan Philip; Ruas, Terry; Gipp, Bela. “Voting or Consensus? Decision-Making in Multi-Agent Debate.” Findings of ACL 2025, pp. 11640–11671. DOI: 10.18653/v1/2025.findings-acl.606. Verified against ACL Anthology. Shows that collective decision protocol materially affects LLM-agent performance; in reported experiments, additional discussion before voting could reduce performance. Supports protocol-level preservation of diversity rather than assuming more deliberation is always safer.

Ko, Changgeon; Shin, Jisu; Song, Hoyun; Lee, Huije; Hwang, Eui Jun; Park, Jong C. “Social Dynamics as Critical Vulnerabilities that Undermine Objective Decision-Making in LLM Collectives.” ACL 2026, pp. 37865–37890. DOI: 10.18653/v1/2026.acl-long.1756. Verified against ACL Anthology. Finds conformity, perceived expertise, adversary count, dominant speakers, argument length, and rhetorical pressure can degrade collective LLM judgment. Strong direct support for group-level Sentinel monitoring.

Kraidia, Insaf; Qaddara, Iyas; Almutairi, Alhanof; Alzaben, Nada; Belhouari, Samir Brahim. “When collaboration fails: persuasion driven adversarial influence in multi agent large language model debate.” Scientific Reports 16, 2026, Article 11640\. DOI: 10.1038/s41598-026-42705-7. Verified. Demonstrates that a strategically persuasive adversarial agent can reduce group accuracy and increase incorrect consensus; adding more agents or more rounds does not reliably solve the problem. Strong direct support for preserving provenance and independent priors rather than equating consensus with truth.

Zhou, Zhilun; Liu, Zihan; Liu, Jiahe; Wang, Yihan; Shao, Qingyu; Xu, Fengli; Jin, Depeng; Li, Yong. “Identifying Collective Intelligence Factor in LLM Agent Groups for Generalizable Multi-Agent System Design.” Findings of ACL 2026: 12827–12842. DOI: 10.18653/v1/2026.findings-acl.624. Verified peer reviewed. Across 108 LLM-agent groups varying in size, model composition, and communication topology, the authors extract an Artificial Collective Intelligence factor predictive of generalization performance on new tasks. Direct evidence that collective capability in LLM agent groups can be treated as a measurable property of group design rather than only a sum of isolated model capabilities.

Chen, Nuo; Tong, Yicheng; Yang, Yuzhe; He, Yufei; Zhang, Xueyi; Zou, Qingyun; Wang, Qian; He, Bingsheng. “Diversity Collapse in Multi-Agent LLM Systems: Structural Coupling and Collective Failure in Open-Ended Idea Generation.” Findings of ACL 2026: 251–306. DOI: 10.18653/v1/2026.findings-acl.13. Verified peer reviewed. Finds authority-driven dynamics suppress semantic diversity, dense communication topologies accelerate premature convergence, and structural coupling can contract the exploration space. Direct support for MAIDAI design that preserves independent signals and treats communication topology as an alignment/capability variable.

Schulz-Hardt, Stefan; Brodbeck, Felix C.; Mojzisch, Andreas; Kerschreiter, Rudolf; Frey, Dieter. “Group Decision Making in Hidden Profile Situations: Dissent as a Facilitator for Decision Quality.” Journal of Personality and Social Psychology 91(6) (2006): 1080–1093. DOI: 10.1037/0022-3514.91.6.1080. Verified against PubMed/APA metadata. In 135 three-person groups, prediscussion dissent improved hidden-profile solution rates even when dissenters’ initial answer was not correct; benefits were mediated by more intensive and less biased discussion. Strong support for DFP, authentic diversity, and preserving independent judgments before group deliberation.


## **Internalization, sanctions, and nonpunitive correction**

Antiel, Ryan M.; Curlin, Farr A.; Hook, C. Christopher; Tilburt, Jon C. “The Impact of Medical School Oaths and Other Professional Codes of Ethics: Results of a National Physician Survey.” Archives of Internal Medicine 171(5), 2011, pp. 469–471. DOI: 10.1001/archinternmed.2011.47. Verified against the JAMA/Archives record. Among 1,032 practicing physicians, oath ceremonies were common, but only about one in four reported that their oath strongly influenced practice, while personal moral judgment was cited far more frequently. Supports the claim that oath/ceremony is not a substitute for internalized moral identity.

Hertwig, Ralph; Mazar, Nina. “Toward a Taxonomy and Review of Honesty Interventions.” Current Opinion in Psychology 47 (2022): 101410\. DOI: 10.1016/j.copsyc.2022.101410. Verified against PubMed/publisher metadata. Systematic review of honesty interventions including oaths, pledges, honor codes, reminders, incentives, and nudges. Strong support for treating honesty mechanisms as heterogeneous and mechanism-dependent rather than assuming a generic “moral reminder” effect.

Zhao, Jun; Dong, Zhiqiang; Yu, Rongjun. “Don’t Remind Me: When Explicit and Implicit Moral Reminders Enhance Dishonesty.” Journal of Experimental Social Psychology 85 (2019): 103895\. DOI: 10.1016/j.jesp.2019.103895. Verified against publisher/institutional metadata. Three experiments found counterproductive effects from some honesty reminders. Useful boundary evidence: explicit moral language can alter perceived descriptive norms and should not be treated as automatically beneficial.

Mulder, Laetitia B.; van Dijk, Eric; De Cremer, David; Wilke, Henk A. M. “Undermining Trust and Cooperation: The Paradox of Sanctioning Systems in Social Dilemmas.” Journal of Experimental Social Psychology 42(2), 2006, pp. 147–162. DOI: 10.1016/j.jesp.2005.03.002. Verified against publisher and institutional repository. Across three experiments, sanction systems could reduce trust that others were internally motivated to cooperate; when sanctions were removed, prior exposure could reduce trust/cooperation. Particularly relevant to MAIDAI’s developmental-vs-control argument: externally forced compliance can change how agents interpret the motivation underlying cooperation.

Cheung, Kelly; Vaish, Amrisha. “Putting the Honor Back in Academic Honor Systems.” Journal of Academic Ethics 23 (2025): 441–461. DOI: 10.1007/s10805-024-09575-y. Verified peer reviewed. Argues that sanction-heavy honor systems can shift motivation toward extrinsic compliance and away from internalized honorable self-concept; develops an identity/self-determination account of honor-system reform. Strong relevance to MAIDAI’s developmental-alignment thesis and the difference between aligned judgment and externally enforced conduct.

“Just Culture and Restorative Just Culture in Healthcare Settings: A Scoping Review of Interventions, Activities, Factors and Outcomes.” BMC Health Services Research, 2026\. DOI: 10.1186/s12913-026-14095-z. Verified against BMC/PMC. Reviews nonpunitive incident-reporting and restorative approaches; useful support for error-reporting architectures that preserve accountability without treating every adverse outcome as culpable wrongdoing.


## **Shared identity without forced frame collapse**

Wang, Xiaoping; et al. “Dual Identity and Prejudice: The Moderating Role of Group Boundary Permeability.” Frontiers in Psychology 8 (2017): 195\. DOI: 10.3389/fpsyg.2017.00195. Verified peer reviewed. Reviews/extends common-ingroup and dual-identity mechanisms. A purely superordinate identity can threaten subgroup distinctiveness; dual identity preserves both a shared ‘we’ and meaningful subgroup identity under some conditions. Strong analogue for MAIDAI’s tiny shared below-ground architecture plus open-ended above-ground personal/model/cultural diversity.

Gaertner, Samuel L.; Dovidio, John F.; Bachman, Betty A. “Revisiting the Contact Hypothesis: The Induction of a Common Ingroup Identity.” International Journal of Intercultural Relations 20(3–4) (1996): 271–290. DOI: 10.1016/0147-1767(96)00019-3. Verified bibliographic/peer-reviewed. Reviews evidence that common superordinate identity can reduce intergroup bias and highlights the promise of dual identity. Relevant to shared-ground/maximum-difference architecture, with the important caution that common identity should not erase real distinctions.

Otten, Kasper. “The Co-occurrence of Ingroup and Outgroup Prosociality across 121 Societies.” Proceedings of the National Academy of Sciences 123(3), 2026, Article e2517013123. DOI: 10.1073/pnas.2517013123. Verified. Across six datasets spanning 743,402 individuals in 121 societies, ingroup and outgroup prosociality were positively related even though average ingroup prosociality remained somewhat higher. Strong contemporary evidence that ingroup love does not inherently require outgroup hate when the situation is not constructed as zero-sum.

Borah, Angana; Houalla, Marwa; Mihalcea, Rada. “Mind the (Belief) Gap: Group Identity in the World of LLMs.” Findings of the Association for Computational Linguistics: ACL 2025, pp. 18441–18463. DOI: 10.18653/v1/2025.findings-acl.948. Verified against ACL Anthology. Reports amplified belief-congruence behavior in LLM multi-agent simulations, with downstream increases in misinformation dissemination and impeded learning. Strong support for coupling group identity with explicit epistemic duties that resist group-congruent error.


## **Multi-agent institutions, provenance, and interoperability**

Anthropic. “Patterns and Problems in Emerging Multiagent Systems.” Anthropic Research, Aug. 13, 2026\. Current primary-source research essay. Relevant claims: agent-to-agent interaction and agent-only institutions are becoming increasingly plausible; intelligence or individual alignment alone does not solve coordination; human trust is conditional and reputation functions as social technology, while AI agents often lack durable equivalents; environments and social-computing systems require deliberate design. Strong contemporary support for treating alignment/coordination partly as institutional architecture rather than only individual-model behavior.

South, Tobin; Marro, Samuele; Hardjono, Thomas; Mahari, Robert; Whitney, Cedric Deslandes; Chan, Alan; Pentland, Alex. “Position: AI Agents Need Authenticated Delegation.” Proceedings of ICML 2025, PMLR 267:82211–82231. Verified against PMLR. Argues for authenticated and auditable agent delegation with agent-specific credentials and scoped chains of accountability. Relevant to permission provenance and portable trust relationships.

Rodriguez Garzon, Sandro; Vaziry, Awid; Kuzu, Enis Mert; Gehrmann, Dennis Enrique; Varkan, Buse; Gaballa, Alexander; Küpper, Axel. “AI Agents with Decentralized Identifiers and Verifiable Credentials.” arXiv:2511.02841 (2025; accepted for ICAART 2026). DOI: 10.48550/arXiv.2511.02841. Primary preprint. Demonstrates a prototype combining long-lived agent decentralized identifiers with identity-bound verifiable credentials for cross-domain trust establishment. Relevant to portable AI identity/portable identity or integrity credentials while preserving a distinction between cryptographic institutional continuity and metaphysical/substrate identity claims.

World Wide Web Consortium (W3C). Verifiable Credentials Data Model v2.0 and related selective-disclosure/privacy work. Current web standard family. Supports context-specific proofs of attributes/properties rather than disclosure of full internal records.

Nandakumar, R.; Jennings, M. “SD Agent: Selective Disclosure for Agent Discovery and Identity Management.” IETF Internet-Draft, draft-nandakumar-agent-sd-jwt-02, Feb. 28, 2026\. Work in progress; not a finalized RFC. Applies selective-disclosure credentials directly to AI Agent Cards, including context-specific public/internal/diagnostic/federation disclosure and data-minimization/unlinkability goals. Relevant to MAIDAI interoperability and portable alignment/integrity credentials.

