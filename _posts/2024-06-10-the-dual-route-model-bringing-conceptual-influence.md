---
title: "The Dual-Route Model: Bringing Conceptual Influences Back in Facial Trait Perception"
date: 2024-06-10
permalink: /posts/2024/06/the-dual-route-model-bringing-conceptual-influences-back-in-/
author: Amber Chen
tags:
  - social perception
  - facial traits
  - psychology
thumbnail: dual-route-image1.png
toc: true
toc_label: "Contents"
toc_sticky: true
excerpt: "A dual-route model of facial trait perception integrating bottom-up perceptual cues and top-down conceptual knowledge to explain consensus and variability in social judgments."
---

<img src="/images/dual-route-image1.png" alt="Illustration" style="max-width: 860px; width: 100%; height: auto; display: block; margin: 0.5em auto 1.25em;" />

## Abstract

Faces convey a wealth of social information, prompting perceivers to form rapid trait impressions with substantial consequences across social, professional, and legal domains. Although early frameworks emphasized either bottom-up, feature-driven processes or top-down, stereotype-based influences, a growing body of evidence indicates that both routes shape face perception in parallel. Research on two-dimensional trait models underscores the role of warmth and competence dimensions in guiding impressions; stereotype and learning theories further reveal how conceptual biases—from group membership and cultural norms to personal experiences—can override purely perceptual cues. The Dynamic Interactive (DI) model highlights a continuous interactive loop between visual input and social knowledge, yet it remains largely theoretical and relies on group-based concepts. In response, I propose a dual-route model that systematically integrates high-dimensional vision models and language-based systems to assess how faces are represented and interpreted. By explaining why trait judgments exhibit both consensus (when perceptual features dominate) and variability (when conceptual factors predominate), this model could clarify how familiarity evolves in real time. Ultimately, the model could shed light on offers a novel means of disentangling the interplay of bottom-up and top-down routes in facial trait perception, paving the way for more individualized, context-sensitive accounts of social cognition.

> Keywords: Facial Trait Perception, Dual-Route Model, Conceptual Influences, Familiarity, Large Language Models

Faces convey rich social information. Among them, facial trait perception is a ubiquitous and influential aspect of human social cognition. Within milliseconds of encountering a face, a perceiver can form rapid and automatic judgments about a target’s personality traits, such as trustworthiness, competence, and dominance (Todorov et al., 2015; Willis & Todorov, 2006), even when the perceiver is instructed not to make such judgments (Ritchie et al., 2017). These first impressions from faces can have far-reaching consequences in various domains of social life, from political elections to criminal sentencing, from hiring decisions to mate choices. For example, political candidates with competent looking faces are more likely to win elections, regardless of their actual qualifications or performance (Todorov et al., 2005). In the workplace, job candidates with faces perceived as more trustworthy or competent are more likely to be selected for interviews and receive job offers (Olivola et al., 2014). Perhaps most concerningly, facial impressions have been shown to affect criminal justice outcomes: untrustworthy-looking defendants receive harsher sentences (Wilson & Rule, 2015), while baby-faced ones are more likely to win intentional-harm cases but lose negligence claims (Zebrowitz & McDonald, 1991).

## Theoretical Review

### Two-dimensional models

There are a plethora of social traits a face can be judged on. How are these social traits conceptually organized? One of the most influential theories is the two-dimensional models of impression formation, which posits that social trait judgement function as one of the adaptive mechanisms for threat detection and individuals primarily judge others’ social traits along two key dimensions: a “horizontal” dimension related to social cooperation—often termed warmth, communion, or trustworthiness—and a vertical dimension associated with goal achievement, labeled competence, agency, or dominance (Abele et al., 2016; Fiske et al., 2007; Judd et al., 2005; Oosterhof & Todorov, 2008). These dimensions convey information critical for social perception and interactions: the first dimension reveals others' intentions toward us, while the second dimension indicates their capacity to fulfill those intentions (Fiske et al., 2002). Over time, while some studies advocated the theory showed that these two dimensions could explain most of the variances (Abele & Wojciszke, 2007; Oosterhof & Todorov, 2008; see Abele et al., 2021 for a review) and exert strong influence over other trait judgments (Yzerbyt et al., 2008), other researchers have proposed more nuanced trait structures—ranging from three (Koch et al., 2016; Vernon et al., 2014) and four (Lin et al., 2021) to twelve (Nicolas et al., 2022) or even fourteen dimensions (Connor et al., 2024) —to account for additional variance in person perception. Despite its broad appeal, the two-dimensional approach has faced critiques that theory-driven methods may restrict the range of traits under investigation and that key constructs such as trustworthiness and dominance may not be independent (Connor et al., 2024; Koch et al., 2016). These critiques pave the way for alternative and complementary perspectives—including stereotype-based accounts, social learning theories, and dynamic interactive frameworks—which collectively deepen our understanding of how facial traits are perceived and evaluated.

### Stereotype

A related theoretical approach to facial trait perception is through the lens of stereotype theories. Stereotypes are mental shortcuts that categorize individuals based on perceived group characteristics and people rely on such conceptual schemas to infer traits from a face such as the characteristics tied to gender, race, or occupation. One line of evidence suggests that stereotypes drive judgements of perceptually ambiguous social groups, indicating that gender and race as the most accessible stereotypes can overshadow other trait judgements (Bin Meshar et al., 2022). For example, one study found that youthful attractiveness explained more variance in female facial impressions, whereas perceived competence was more influential for male facial impressions (South Palomares & Young, 2018). Similarly, another study further revealed the gender asymmetry in trait judgement that even when visual information was held constant, female faces were judged less differentiated and more valence-laden than male faces, particularly among individuals with stronger gender stereotypes (Oh et al., 2020). These findings extend to racial stereotypes as well (Xie et al., 2021). Moreover, occupation-based stereotypes also shape trait judgments: labeling a face as belonging to a high-status profession (e.g., doctor or lawyer) can significantly increase perceived competence, whereas framing the same face as a service worker or artist might heighten perceptions of warmth (Imhoff et al., 2013; Oldmeadow et al., 2013). Even minimal group categorizations can bias mental representations of faces, resulting in more favorable impressions of ingroup members (Hong & Ratner, 2021). These studies demonstrate that as group-based conceptual representations, stereotypes can profoundly influence how individuals interpret facial cues, suggesting that broader social assumptions can override purely perceptual information when forming impressions.

Learning

From another perspective of learning mechanisms, people’s perceptions of facial traits are shaped by accumulated experiences, social partners, and cultural influences (Hassin & Trope, 2000; for a review, see Sutherland & Young, 2022). Laboratory studies reveal that people can learn facial trait associations through appearance-trait pairings (Over et al., 2023) and stereotypical associations with faces can also be trained to mitigate (Chua & Freeman, 2021). In social contexts, observers align their ratings of attractiveness and even their neural representations of faces with peers—particularly ingroup members under stricter social norms (Chen et al., 2024). Drawing on prior experiences, participants in financial trust games tended to choose partners who resemble previously encountered trustworthy partners and avoid those who resemble untrustworthy counterparts (FeldmanHall et al., 2018; Gawronski & Quinn, 2013; Verosky & Todorov, 2010). Researchers have captured these processes through statistical learning models, showing how people come to associate facial features with desirable attributes like trustworthiness based on accumulated interactions (Over & Cook, 2018; Uddenberg et al., 2023). Cultural learning theories assert that facial trait perception is not innate but arises from culturally acquired associative mappings, allowing activation to spread from facial representations to trait inferences (Cook et al., 2022). For example, a cross-cultural study found that variability in face impressions is related to regional personality structures, suggesting that cultural factors shape facial trait perception through conceptual understanding of personality structure (Oh et al., 2022). Twin studies further underscore that environmental factors—rather than genetics—have been shown to predominantly explain the variance in ratings of facial attractiveness and trustworthiness (Germine et al., 2015; Sutherland et al., 2020).

When these learning processes extend beyond their original contexts, they risk overgeneralization, where inferences about one individual spill over onto others who share superficial similarities (Zebrowitz & Montepare, 2008). For example, people exposed to a warm partner in one context tended to rate a visually similar face as kinder and friendlier in another, and this overgeneralization applied to both experimental settings (Gawronski & Quinn, 2013; Verosky & Todorov, 2010) and personal experiences (Sutherland et al., 2020). A related phenomenon, emotional overgeneralization arises when fleeting expressions (e.g., anger or happiness) are misconstrued as enduring personality traits (Knutson, 1996; Todorov et al., 2007) such that anger signals untrustworthiness; happiness conveys friendliness (Albohn & Adams Jr., 2021). This phenomenon has also been described as the Temporal Extension Hypothesis (Knutson, 1996; Secord, 1958; Sutherland & Young, 2022; Todorov, 2008). Likewise, the attractiveness halo effect leads to more positive attributions toward attractive individuals (Zebrowitz et al., 2012; Zebrowitz & Montepare, 2008). In another way, older adults' neutral facial expressions are more likely misinterpreted as anger compared to those of younger adults. This misattribution is linked to age-related facial features such as wrinkles and sagging, which possibly mimic the muscle movements associated with anger (Fölster et al., 2014). Recent modeling efforts bolster the learning perspective, demonstrating that face impressions can be explained as robust statistical interpretations of within-person variability (Kramer et al., 2018) or as emergent properties in computational networks trained on face recognition (Parde et al., 2019). In short, these findings collectively highlight how learning mechanisms—whether from laboratory tasks, social or cultural environments, or personal experiences—profoundly influence facial trait perception and can lead to both adaptive inferences and systematic biases.

### Dynamic Interactive (DI) model

Building upon the principles of dual-process theories of the mind (Kahneman, 2003), we can understand person perception through two systems: a rapid, bottom-up perceptual process and slower, top-down conceptual process. Early research either focused on facial features for trait perception or only studied the conceptual biases, stemming from stereotypes, cultural knowledge, and prior experiences, in the process of facial impression. An early framework, parallel-constraint-satisfaction theory of impression formation, posited that social judgements emerge from the activation of multiple constraints: stereotypes, behaviors and traits, which are represented as interconnected nodes in an activation network (Kunda & Thagard, 1996). However, these insights have become more systematically and quantitatively tested in recent years. Empirical studies revealed that both perceptual and conceptual routes contribute robustly and in parallel to face processing. Not only the object recognition is rich with perceptual and conceptual information (Lupyan & Spivey, 2008), but also the face processing (Schwartz & Yovel, 2016). A key development in this field is the Dynamic Interactive (DI) model of person perception (Freeman & Ambady, 2011), which emphasizes continuous interplay between top-down conceptual information (e.g., stereotypes, prior knowledge) and bottom-up sensory input (e.g., visual cues of a face). According to this view, rather than operating as independent systems, the DI model conceptualizes social perception as an ongoing process in which low-level perceptual data are continually integrated with higher-level cognitive factors. In line with this, recent researchers propose that unlike fixed dimensions, trait perceptions emerge from the continuous integration of individual conceptual associations with faces (Over & Cook, 2018; Stolier et al., 2018). Empirical studies further support these dynamic processes. For example, research shows that conceptual information (e.g., group membership) can independently (Kubota & Ito, 2007) or interactively (Brooks & Freeman, 2018) shape face perception. Over time, bottom-up signals (e.g., voice, motion) and top-down inputs (e.g., semantic narratives) jointly update initial impressions (Lin & Thornton, 2024). Moreover, stereotypes and culturally acquired associations exert strong effects on facial trait perception (Stolier et al., 2020; Xie et al., 2021).

Early models of face-based trait perception formation emphasized perceptual inputs from facial features but often overlooked conceptual influences. For example, data-driven models derived trait dimensions directly from facial morphology or open-ended descriptions of faces (Stolier et al., 2018). While such models capture common feature-driven impressions, they assume a fixed “face trait space” and cannot explain why impressions vary across perceivers (Freeman & Chwe, 2024). Similarly, pure stereotype-based accounts -where a face triggers social stereotypes (e.g., baby-faced = naive) or certain characteristics tie to a social group (e.g., man = aggressive) - provide a conceptual angel but often fail to specify how visual cues and beliefs interact in real time. The DI model attempts to address this by positing a continuous feedback loop between bottom-up visual cues and top-down social knowledge during person perception. However, the DI model remains largely theoretical and does not quantify separate contributions of perceptual vs conceptual inputs. Moreover, while the DI model is well suited for group-based conceptual knowledge (e.g., stereotypes), it is less directly applicable to person-specific familiarity, which also shapes everyday face perception. Such familiarity can arise through personal contact (e.g., family, friends), recognition of public figures, or induced exposure in laboratory settings, each type entailing distinct conceptual knowledge that influences social and affective judgments (for a comprehensive review, see Ramon & Gobbini 2018). In sum, prior accounts either treated trait perception as a fixed bottom-up process or a general stereotype influence, lacking a systematic way to disentangle and measure each route.

Introduction to the Dual-Route Model

Here I propose a dual-route model of facial trait perception, which posits that individuals derive trait judgments from two distinct yet interacting pathways: a perceptual route and a conceptual route (see Figure 1). The perceptual route processes visual cues from the face (e.g., shape, texture, configuration) and generates category-consistent impressions through low-level, image-based mechanisms. In contrast, the conceptual route integrates contextual and semantic knowledge—such as stereotypes, group memberships, and personal experiences—to influence trait inferences. While some existing frameworks (e.g., the Dynamic Interactive model) acknowledge that bottom-up and top-down processes operate in tandem, they typically lack a systematic way of isolating and quantifying each route’s contribution. By bridging state-of-the-art vision models (which capture the high-dimensional visual representations underlying face perception) with language models (which encode the person- and group-specific conceptual associations guiding social inference), our dual-route framework aims to precisely measure and predict how these two routes converge—thus offering a more comprehensive account of individual differences, contextual effects, and the dynamic nature of social judgments.

Recent research supports a distinction between perceptual and conceptual routes in forming facial trait perception. For example, studies have shown that individuals’ idiosyncratic conceptual frameworks shape their face impressions: observers who believe two traits tend to go together (e.g., “trustworthy” and “intelligent”) also judge faces in a more similar way on those traits (Stolier et al., 2018; Xie et al., 2021) and this tendency was also found across cultures (Oh et al., 2022; Sutherland et al., 2020). Across studies, they showed that a data-driven face trait space is systematically influenced by a conceptual trait space reflecting the perceiver’s beliefs about trait correlations. This implies trait impressions are not solely “read off” the face; they are also shaped by conceptual knowledge that the observers bear from their prior experience.

Evidence for Conceptual Contributions to Trait Perception

Recent studies have examined how the perceptual route influences person perception. For example, a fMRI study showed that face-elicited neural patterns in fusiform gyrus aligned with the observers’ stereotypical trait associations​, implying that stereotypes bias the visual representation of faces​ (Barnett et al., 2021). Masking specifically reduced connectivity between fusiform and orbitofrontal cortex, and this loss of interaction eliminated the stereotype influence​. These results indicate a distinct conceptual route (via orbitofrontal feedback) that injects social knowledge into the perceptual processing of faces. When that route is cut off, trait judgments must rely on the perceptual route alone, reducing biased impressions. This finding validates a core idea of the DI model (interaction of facial input and stereotypes) while highlighting that top-down conceptual input plays a critical role in face impressions.

Taking the two routes together, behavioral and neuroimaging studies echo this dual-route distinction in the context of face processing. Using deep neural networks including a vision model, a large language model and multimodal model to quantify the visual and semantic contributions of celebrities’ face and name similarity judgements, a behavioral study showed a larger visual than semantic contribution when images were viewed and a reversed pattern when names were recalled (Shoham et al., 2024). Utilizing a similar method, a neuroimaging study showed that a stronger association between semantic representations and neural representations predicted better face recognition (Faghel-Soubeyrand et al., 2024). Thus, a dual-route model of person perception is supported: one pathway analyzes the face’s perceptual features, and another takes conceptual knowledge into account.

Familiar Faces: Stronger Conceptual Influences

What further questions can the dual-route model answer? Familiarization provides a key avenue for exploration: as a face becomes familiar, conceptual influences grow stronger while visual influences remain relatively stable. Familiar faces, tied to identity-specific knowledge (e.g., names, known traits, and past interactions), are perceived more holistically and consistently, with even subtle facial cues becoming more salient (see Figure 1). In contrast, unfamiliar face impressions rely heavily on the perceptual route since no stored identity or semantics are available. Neurocognitive models of face recognition suggest that recognizing a familiar person recruits an extended system (anterior temporal and frontal regions) that encodes personal knowledge, beyond the core visual face areas (Gobbini & Haxby, 2007; Ramon & Gobbini, 2018). Empirical studies confirm that familiarity modulates neural processing. For instance, EEG studies found that simply seeing a face repeatedly (perceptual familiarization) produced little change in neural patterns, but richer familiarization – especially social interaction – induced a neural signature of “familiarity” that emerged around 400 ms after seeing the face (Ambrus et al., 2021). In a related fMRI study, multiple images of the same familiar person evoked more similar activation patterns in high-level visual cortex than images of unfamiliar person, meaning the neural representations of the images clustered together​ (Ramon et al., 2015). Single-unit recordings likewise revealed greater representational distances among familiar identities compared to those among unfamiliar ones (R. Cao et al., 2024). In other words, once you know someone, your brain groups different photos of the person together, instead of processing them independently; your brain also tells the identity apart from other identities.

From the dual-route model perspective, this familiarization process can be understood as a process of accumulating conceptual knowledge related to a face. Computationally, becoming familiar with faces means learning idiosyncratic dimensions of variability in appearance; then binding those images to a stable identity requires a conceptual label or abstraction in conceptual processing (Burton et al., 2016). For example, behavioral and fMRI studies showed that learning a novel face with conceptual labels or seeing a face with known personal information engaged the social brain network (e.g., medial prefrontal cortex), more than purely perceptual encoding, and improved later recognition (Cloutier et al., 2011; Schwartz & Yovel, 2016; Shoham et al., 2021). Furthermore, a recent study found the temporal pole responded selectively to familiar faces over unfamiliar faces, objects, and scenes and connected visual images of familiar faces with conceptual information (Deen et al., 2024). These indicate that the conceptual route matching person knowledge to the face markedly alters processing for familiar faces, consistent with the idea that familiar face recognition is person recognition, not just visual recognition.

Bridging Vision and Language: A Dual-Route Computational Framework

Quantifying Perceptual Information Using Computer Vision Models

Along with the rapid advancement in the field of computer vision, studies incorporating computer vision algorithms and trait ratings showed that specific morphological or textural attributes reliably predict certain trait inferences (R. Cao et al., 2023; Diego-Mas et al., 2020; Parde et al., 2019; Peterson et al., 2022). Moreover, neural representations in face-processing brain regions aligned closely with a dominance-trustworthiness trait space, suggesting that visual input is automatically mapped onto these evaluative dimensions (Chwe et al., 2024). Together, these results confirm a distinct visual contribution to face-based trait judgments—one that coexists and interacts with broader conceptual influences such as stereotypes, prior experiences, and cultural norms.

Quantifying Conceptual Knowledge Using Large Language Models

While the dual-route framework highlights the importance of conceptual knowledge—particularly for familiar targets—quantitatively measuring that knowledge remains challenging. This is in part due to the difficulty in quantifying the conceptual information associated with a target person. For instance, Barack Obama and Michael Jordan are two public figures most Americans are familiar with. However, it is challenging to comprehensively characterize their conceptual (dis)similarity due to the almost infinite dimensions on which they can be compared (e.g., race, career, political orientation, socio-economic status, personality). Recent rapid developments in artificial intelligence (AI), especially Large Language Models (LLMs), have made it more accessible to comprehensively quantify conceptual/semantic information associated with public figures (i.e., individuals whose information are publicly available in the form of text data). LLMs, such as Bidirectional Encoder Representations from Transformers (BERT) and Generative Pre-trained Transformer (GPT), are built using neural networks trained on vast amounts of text data to predict and generate coherent language. They learn patterns, grammar, and context by modeling the relationships between words, phrases, and sentences. Sentence embeddings, derived from LLMs or specialized models, represent sentences as dense numerical vectors in a high-dimensional space, capturing their semantic meaning and enabling comparisons, clustering, or other analyses based on their contextual similarity. With this enormous capacity to capture conceptual information in high-dimensional space, LLMs can encode complex social information. In the above example, we can enter public texts about Obama and Jordan (e.g., news articles, social media posts, books, etc.) into LLMs, which can then characterize the two “concepts” (Obama and Jordan) in the high-dimensional conceptual space, a process termed embedding. The conceptual relationship between the two public figures can then be comprehensively and quantitatively characterized by their relative positions in the conceptual space. Using this approach, researchers could predict person similarity perceptions  (Shoham et al., 2024) and perceived personality traits of public figures (Cao & Kosinski, 2024), decode face recognition abilities (Faghel-Soubeyrand et al., 2024), and processing emotional information across various channels (Ong et al., 2023). Moreover, models trained on diverse datasets with natural language supervision have demonstrated improved performance in modeling high-level visual cortex activity (A. Y. Wang et al., 2023). Consequently, LLMs offer a promising route for operationalizing the conceptual route in face perception—particularly for well-known individuals whose textual records are publicly available.

Challenges and Limitations

Despite these advances, applying language embedding techniques to measure conceptual knowledge in trait perception is not without pitfalls. First, LLMs may reinforce historical biases present in their training data, potentially perpetuating and amplifying societal stereotypes rather than objectively modeling them (Bai et al., 2025; Nicolas & Caliskan, 2024). Second, prediction accuracy varies systematically across demographic groups, with higher accuracies for younger and female users (Peters & Matz, 2024). This suggests that language embeddings may not equally represent conceptual structures across diverse populations. Similarly, many studies rely on celebrity face datasets, which rarely represent diverse populations. Such sampling biases, when combined with model-level biases, can produce skewed trait inferences, particularly for underrepresented groups. Nevertheless, these concerns do not diminish the broader potential of AI-based approaches. Rather, they highlight the importance of embedding LLMs within a theoretical framework that balances perceptual and conceptual influences, ensuring that social biases are recognized, quantified, and—ideally—mitigated.

## Conclusion

Together, these findings support a dual-route model of face perception: one route is a bottom-up visual analysis, as captured by vision models or deep face networks, and another is a top-down conceptual route drawing on semantic representations. Methodologically, a hybrid model that combines a vision CNN (to represent facial feature patterns) with a language model (to represent semantic or stereotype knowledge) could quantify each component’s contribution to person perception. For example, the vision model could predict trait impressions based on facial structure (perceptual route), while the language model predicts impressions based on associations (conceptual route); discrepancies between the two predictions might indicate where conceptual bias overrides pure visual cues. By leveraging state-of-the-art deep learning models as proxies for human vision and language systems, researchers can measure and manipulate the routes independently. In summary, an integrated model that combines visual and conceptual representations is well-positioned to capture the full complexity of facial trait perception. It can explain not only the consensus driven by facial features, but also the individual differences and context effects driven by conceptual knowledge – bridging the gap that earlier single-route or static models could not address. In doing so, we could advance to a comprehensive understanding of how facial impressions form, how they become entrenched through familiarity, and how they can be modified—or even overridden—by conceptual insight.

## References

Abele, A. E., Ellemers, N., Fiske, S. T., Koch, A., & Yzerbyt, V. (2021). Navigating the social world: Toward an integrated framework for evaluating self, individuals, and groups. Psychological Review, 128(2), 290–314. https://doi.org/10.1037/rev0000262

Abele, A. E., & Wojciszke, B. (2007). Agency and communion from the perspective of self versus others. Journal of Personality and Social Psychology, 93(5), 751–763. https://doi.org/10.1037/0022-3514.93.5.751

Albohn, D. N., & Adams Jr., R. B. (2021). The expressive triad: Structure, color, and texture similarity of emotion expressions predict impressions of neutral faces. Frontiers in Psychology, 12. https://doi.org/10.3389/fpsyg.2021.612923

Ambrus, G. G., Eick, C. M., Kaiser, D., & Kovács, G. (2021). Getting to Know You: Emerging Neural Representations during Face Familiarization. The Journal of Neuroscience, 41(26), 5687–5698. https://doi.org/10.1523/JNEUROSCI.2466-20.2021

Andrew H. Chwe, J., & Freeman, J. B. (2024). Trustworthiness of Crowds Is Gleaned in Half a Second. Social Psychological and Personality Science, 15(3), 351–359. https://doi.org/10.1177/19485506231164703

Bai, X., Wang, A., Sucholutsky, I., & Griffiths, T. L. (2025). Explicitly unbiased large language models still form biased associations. Proceedings of the National Academy of Sciences of the United States of America, 122(8), e2416228122. https://doi.org/10.1073/pnas.2416228122

Barnett, B. O., Brooks, J. A., & Freeman, J. B. (2021). Stereotypes bias face perception via orbitofrontal-fusiform cortical interaction. Social Cognitive and Affective Neuroscience, 16(3), 302–314. https://doi.org/10.1093/scan/nsaa165

Bin Meshar, M., Stolier, R. M., & Freeman, J. B. (2022). Facial Stereotyping Drives Judgments of Perceptually Ambiguous Social Groups. Social Psychological and Personality Science, 13(8), 1221–1229. https://doi.org/10.1177/19485506211062285

Brooks, J. A., & Freeman, J. B. (2018). Conceptual knowledge predicts the representational structure of facial emotion perception. Nature Human Behaviour, 2(8), Article 8. https://doi.org/10.1038/s41562-018-0376-6

Burton, A. M., Kramer, R. S. S., Ritchie, K. L., & Jenkins, R. (2016). Identity From Variation: Representations of Faces Derived From Multiple Instances. Cognitive Science, 40(1), 202–223. https://doi.org/10.1111/cogs.12231

Cao, R., Wang, J., Brunner, P., Willie, J. T., Li, X., Rutishauser, U., Brandmeir, N. J., & Wang, S. (2024). Neural mechanisms of face familiarity and learning in the human amygdala and hippocampus. Cell Reports, 43(1), 113520. https://doi.org/10.1016/j.celrep.2023.113520

Cao, R., Zhang, N., Yu, H., Webster, P. J., Paul, L. K., Li, X., Lin, C., & Wang, S. (2023). Comprehensive Social Trait Judgments From Faces in Autism Spectrum Disorder. Psychological Science, 34(10), 1121–1145. https://doi.org/10.1177/09567976231192236

Cao, X., & Kosinski, M. (2024). Large language models know how the personality of public figures is perceived by the general public. Scientific Reports, 14(1), 6735. https://doi.org/10.1038/s41598-024-57271-z

Chen, D., Yao, Z., Liu, J., Wu, H., & Hu, X. (2024). Social conformity updates the neural representation of facial attractiveness. Communications Biology, 7(1), 1–10. https://doi.org/10.1038/s42003-024-06791-5

Chua, K.-W., & Freeman, J. B. (2021). Facial stereotype bias is mitigated by training. Social Psychological and Personality Science, 12(7), 1335–1344. https://doi.org/10.1177/1948550620972550

Chwe, J. A. H., Vartiainen, H. I., & Freeman, J. B. (2024). A Multidimensional Neural Representation of Face Impressions. The Journal of Neuroscience, 44(39), e0542242024. https://doi.org/10.1523/JNEUROSCI.0542-24.2024

Cloutier, J., Kelley, W. M., & Heatherton, T. F. (2011). The Influence of Perceptual and Knowledge-based Familiarity on the Neural Substrates of Face Perception. Social Neuroscience, 6(1), 63–75. https://doi.org/10.1080/17470911003693622

Connor, P., Nicolas, G., Antonoplis, S., & Koch, A. (2024). Unconstrained Descriptions of Facebook Profile Pictures Support High-Dimensional Models of Impression Formation. Personality & Social Psychology Bulletin, 1461672241266651. https://doi.org/10.1177/01461672241266651

Cook, R., Eggleston, A., & Over, H. (2022). The cultural learning account of first impressions. Trends in Cognitive Sciences, 26(8), 656–668. https://doi.org/10.1016/j.tics.2022.05.007

Deen, B., Husain, G., & Freiwald, W. A. (2024). A familiar face and person processing area in the human temporal pole. Proceedings of the National Academy of Sciences of the United States of America, 121(28), e2321346121. https://doi.org/10.1073/pnas.2321346121

Diego-Mas, J. A., Fuentes-Hurtado, F., Naranjo, V., & Alcañiz, M. (2020). The Influence of Each Facial Feature on How We Perceive and Interpret Human Faces. I-Perception, 11(5), 2041669520961123. https://doi.org/10.1177/2041669520961123

Faghel-Soubeyrand, S., Ramon, M., Bamps, E., Zoia, M., Woodhams, J., Richoz, A.-R., Caldara, R., Gosselin, F., & Charest, I. (2024). Decoding face recognition abilities in the human brain. PNAS Nexus, 3(3), pgae095. https://doi.org/10.1093/pnasnexus/pgae095

FeldmanHall, O., Dunsmoor, J. E., Tompary, A., Hunter, L. E., Todorov, A., & Phelps, E. A. (2018). Stimulus generalization as a mechanism for learning to trust. PNAS Proceedings of the National Academy of Sciences of the United States of America, 115(7), E1690–E1697. https://doi.org/10.1073/pnas.1715227115

Fölster, M., Hess, U., & Werheid, K. (2014). Facial age affects emotional expression decoding. Frontiers in Psychology, 5. https://doi.org/10.3389/fpsyg.2014.00030

Freeman, J. B., & Chwe, J. A. (2024). Social Categorization: Looking Toward the Future. In D. E. Carlston, K. Hugenberg, & K. L. Johnson (Eds.), The Oxford Handbook of Social Cognition, Second Edition (2nd ed., pp. 198–221). Oxford University Press. https://doi.org/10.1093/oxfordhb/9780197763414.013.7

Gawronski, B., & Quinn, K. A. (2013). Guilty by mere similarity: Assimilative effects of facial resemblance on automatic evaluation. Journal of Experimental Social Psychology, 49(1), 120–125. https://doi.org/10.1016/j.jesp.2012.07.016

Germine, L., Russell, R., Bronstad, P. M., Blokland, G. A. M., Smoller, J. W., Kwok, H., Anthony, S. E., Nakayama, K., Rhodes, G., & Wilmer, J. B. (2015). Individual Aesthetic Preferences for Faces Are Shaped Mostly by Environments, Not Genes. Current Biology, 25(20), 2684–2689. https://doi.org/10.1016/j.cub.2015.08.048

Gobbini, M. I., & Haxby, J. V. (2007). Neural systems for recognition of familiar faces. Neuropsychologia, 45(1), 32–41. https://doi.org/10.1016/j.neuropsychologia.2006.04.015

Guan, J., Ryali, C. K., & Yu, A. J. (2018). Computational modeling of social face perception in humans: Leveraging the active appearance model [Preprint]. Animal Behavior and Cognition. https://doi.org/10.1101/360776

Hassin, R., & Trope, Y. (2000). Facing faces: Studies on the cognitive aspects of physiognomy. Journal of Personality and Social Psychology, 78(5), 837–852. https://doi.org/10.1037/0022-3514.78.5.837

Hausladen, C. I., Knott, M., Camerer, C. F., & Perona, P. (2024). Social perception of faces in a vision-language model (arXiv:2408.14435). arXiv. https://doi.org/10.48550/arXiv.2408.14435

Hong, Y., & Ratner, K. G. (2021). Minimal but not meaningless: Seemingly arbitrary category labels can imply more than group membership. Journal of Personality and Social Psychology, 120(3), 576–600. https://doi.org/10.1037/pspa0000255

Hong, Y., Reed, M., & Ratner, K. G. (2023). Facial Stereotypes of Competence (Not Trustworthiness or Dominance) Most Resemble Facial Stereotypes of Group Membership. Social Cognition, 41(6), 562–578. https://doi.org/10.1521/soco.2023.41.6.562

Imhoff, R., Woelki, J., Hanke, S., & Dotsch, R. (2013). Warmth and competence in your face! Visual encoding of stereotype content. Frontiers in Psychology, 4, 386. https://doi.org/10.3389/fpsyg.2013.00386

Kahneman, D. (2003). A perspective on judgment and choice: Mapping bounded rationality. American Psychologist, 58(9), 697–720. https://doi.org/10.1037/0003-066X.58.9.697

Knutson, B. (1996). Facial expressions of emotion influence interpersonal trait inferences. Journal of Nonverbal Behavior, 20(3), 165–182. https://doi.org/10.1007/BF02281954

Koch, A., Imhoff, R., Dotsch, R., Unkelbach, C., & Alves, H. (2016). The ABC of stereotypes about groups: Agency/socioeconomic success, conservative–progressive beliefs, and communion. Journal of Personality and Social Psychology, 110(5), 675–709. https://doi.org/10.1037/pspa0000046

Kramer, R. S. S., Young, A. W., & Burton, A. M. (2018). Understanding face familiarity. Cognition, 172, 46–58. https://doi.org/10.1016/j.cognition.2017.12.005

Kubota, J. T., & Ito, T. A. (2007). Multiple Cues in Social Perception: The Time Course of Processing Race and Facial Expression. Journal of Experimental Social Psychology, 43(5), 738–752. https://doi.org/10.1016/j.jesp.2006.10.023

Lin, C., Keles, U., & Adolphs, R. (2021). Four dimensions characterize attributions from faces using a representative set of English trait words. Nature Communications, 12(1), Article 1. https://doi.org/10.1038/s41467-021-25500-y

Lin, C., & Thornton, M. A. (2024). Bottom-up and top-down information determinants of naturalistic trait impression updating. https://doi.org/10.31234/osf.io/jxzca

Lupyan, G., & Spivey, M. J. (2008). Perceptual processing is facilitated by ascribing meaning to novel stimuli. Current Biology, 18(10), R410–R412. https://doi.org/10.1016/j.cub.2008.02.073

Marini, F., Sutherland, C. A. M., Ostrovska, B., & Manassi, M. (2023). Three’s a crowd: Fast ensemble perception of first impressions of trustworthiness. Cognition, 239, 105540. https://doi.org/10.1016/j.cognition.2023.105540

Nicolas, G., Bai, X., & Fiske, S. T. (2022). A spontaneous stereotype content model: Taxonomy, properties, and prediction. Journal of Personality and Social Psychology, 123(6), 1243–1263. https://doi.org/10.1037/pspa0000312

Nicolas, G., & Caliskan, A. (2024). Directionality and representativeness are differentiable components of stereotypes in large language models. PNAS Nexus, 3(11), pgae493. https://doi.org/10.1093/pnasnexus/pgae493

Oh, D., Dotsch, R., Porter, J., & Todorov, A. (2020). Gender biases in impressions from faces: Empirical studies and computational models. Journal of Experimental Psychology: General, 149(2), 323–342. https://doi.org/10.1037/xge0000638

Oh, D., Martin, J. D., & Freeman, J. B. (2022). Personality Across World Regions Predicts Variability in the Structure of Face Impressions. Psychological Science, 33(8), 1240–1256. https://doi.org/10.1177/09567976211072814

Oldmeadow, J. A., Sutherland, C. A. M., & Young, A. W. (2013). Facial Stereotype Visualization Through Image Averaging. Social Psychological and Personality Science, 4(5), 615–623. https://doi.org/10.1177/1948550612469820

Olivola, C. Y., Funk, F., & Todorov, A. (2014). Social attributions from faces bias human choices. Trends in Cognitive Sciences, 18(11), 566–570. https://doi.org/10.1016/j.tics.2014.09.007

Oosterhof, N. N., & Todorov, A. (2008). The functional basis of face evaluation. Proceedings of the National Academy of Sciences, 105(32), 11087–11092. https://doi.org/10.1073/pnas.0805664105

Over, H., & Cook, R. (2018). Where do spontaneous first impressions of faces come from? Cognition, 170, 190–200. https://doi.org/10.1016/j.cognition.2017.10.002

Over, H., Lee, R., Flavell, J., Vestner, T., & Cook, R. (2023). Contextual modulation of appearance-trait learning. Cognition, 230, 105288. https://doi.org/10.1016/j.cognition.2022.105288

Parde, C. J., Hu, Y., Castillo, C., Sankaranarayanan, S., & O’Toole, A. J. (2019). Social Trait Information in Deep Convolutional Neural Networks Trained for Face Identification. Cognitive Science, 43(6), e12729. https://doi.org/10.1111/cogs.12729

Peters, H., & Matz, S. C. (2024). Large language models can infer psychological dispositions of social media users. PNAS Nexus, 3(6), pgae231. https://doi.org/10.1093/pnasnexus/pgae231

Peterson, J. C., Uddenberg, S., Griffiths, T. L., Todorov, A., & Suchow, J. W. (2022). Deep models of superficial face judgments. Proceedings of the National Academy of Sciences, 119(17), e2115228119. https://doi.org/10.1073/pnas.2115228119

Ramon, M., & Gobbini, M. I. (2018). Familiarity matters: A review on prioritized processing of personally familiar faces. Visual Cognition, 26(3), 179–195. https://doi.org/10.1080/13506285.2017.1405134

Ramon, M., Vizioli, L., Liu-Shuang, J., & Rossion, B. (2015). Neural microgenesis of personally familiar face recognition. Proceedings of the National Academy of Sciences of the United States of America, 112(35), E4835-4844. https://doi.org/10.1073/pnas.1414929112

Ritchie, K. L., Palermo, R., & Rhodes, G. (2017). Forming impressions of facial attractiveness is mandatory. Scientific Reports, 7(1), 469. https://doi.org/10.1038/s41598-017-00526-9

Schuster, C. M., Dinisor, M.-A., Ghatiwala, S., & Groh, G. (2025). Profiling Bias in LLMs: Stereotype Dimensions in Contextual Word Embeddings (arXiv:2411.16527). arXiv. https://doi.org/10.48550/arXiv.2411.16527

Schwartz, L., & Yovel, G. (2016). The roles of perceptual and conceptual information in face recognition. Journal of Experimental Psychology: General, 145(11), 1493–1511. https://doi.org/10.1037/xge0000220

Secord, P. F. (1958). Facial features and inference processes in interpersonal perception. Person Perception and Interpersonal Behavior, 300–315.

Shoham, A., Grosbard, I. D., Patashnik, O., Cohen-Or, D., & Yovel, G. (2024). Using deep neural networks to disentangle visual and semantic information in human perception and memory. Nature Human Behaviour, 8(4), 702–717. https://doi.org/10.1038/s41562-024-01816-9

Shoham, A., Kliger, L., & Yovel, G. (2021). Learning faces as concepts improves face recognition by engaging the social brain network. Social Cognitive and Affective Neuroscience, 17(3), 290–299. https://doi.org/10.1093/scan/nsab096

South Palomares, J. K., & Young, A. W. (2018). Facial first impressions of partner preference traits: Trustworthiness, status, and attractiveness. Social Psychological and Personality Science, 9(8), 990–1000. https://doi.org/10.1177/1948550617732388

Steed, R., & Caliskan, A. (2021). A set of distinct facial traits learned by machines is not predictive of appearance bias in the wild. AI and Ethics, 1(3), 249–260. https://doi.org/10.1007/s43681-020-00035-y

Stolier, R. M., Hehman, E., & Freeman, J. B. (2020). Trait knowledge forms a common structure across social cognition. Nature Human Behaviour, 4(4), 361–371. https://doi.org/10.1038/s41562-019-0800-6

Stolier, R. M., Hehman, E., Keller, M. D., Walker, M., & Freeman, J. B. (2018). The conceptual structure of face impressions. Proceedings of the National Academy of Sciences of the United States of America, 115(37), 9210–9215. https://doi.org/10.1073/pnas.1807222115

Sutherland, C. A. M., Burton, N. S., Wilmer, J. B., Blokland, G. A. M., Germine, L., Palermo, R., Collova, J. R., & Rhodes, G. (2020). Individual differences in trust evaluations are shaped mostly by environments, not genes. Proceedings of the National Academy of Sciences, 117(19), 10218–10224. https://doi.org/10.1073/pnas.1920131117

Sutherland, C. A. M., Oldmeadow, J. A., & Young, A. W. (2016). Integrating social and facial models of person perception: Converging and diverging dimensions. Cognition, 157, 257–267. https://doi.org/10.1016/j.cognition.2016.09.006

Sutherland, C. A. M., & Young, A. W. (2022). Understanding trait impressions from faces. British Journal of Psychology, 113(4), 1056–1078. https://doi.org/10.1111/bjop.12583

Todorov, A. (2008). Evaluating Faces on Trustworthiness: Extension of Systems for Recognition of Emotions Signaling Approach/Avoidance Behaviors. Annals of the New York Academy of Sciences, 1124(1), 208–224. https://doi.org/10.1196/annals.1440.012

Todorov, A., Gobbini, M. I., Evans, K. K., & Haxby, J. V. (2007). Spontaneous retrieval of affective person knowledge in face perception. Neuropsychologia, 45(1), 163–173. https://doi.org/10.1016/j.neuropsychologia.2006.04.018

Todorov, A., Mandisodza, A. N., Goren, A., & Hall, C. C. (2005). Inferences of Competence from Faces Predict Election Outcomes. Science, 308(5728), 1623–1626. https://doi.org/10.1126/science.1110589

Todorov, A., Olivola, C. Y., Dotsch, R., & Mende-Siedlecki, P. (2015). Social Attributions from Faces: Determinants, Consequences, Accuracy, and Functional Significance. Annual Review of Psychology, 66(1), 519–545. https://doi.org/10.1146/annurev-psych-113011-143831

Uddenberg, S., Thompson, B. D., Vlasceanu, M., Griffiths, T. L., & Todorov, A. (2023). Iterated learning reveals stereotypes of facial trustworthiness that propagate in the absence of evidence. Cognition, 237, 105452. https://doi.org/10.1016/j.cognition.2023.105452

Vernon, R. J. W., Sutherland, C. A. M., Young, A. W., & Hartley, T. (2014). Modeling first impressions from highly variable facial images. Proceedings of the National Academy of Sciences of the United States of America, 111(32), E3353-3361. https://doi.org/10.1073/pnas.1409860111

Verosky, S. C., & Todorov, A. (2010). Generalization of affective learning about faces to perceptually similar faces. Psychological Science, 21(6), 779–785. https://doi.org/10.1177/0956797610371965

Wang, A., Morgenstern, J., & Dickerson, J. P. (2025). Large language models that replace human participants can harmfully misportray and flatten identity groups. Nature Machine Intelligence, 1–12. https://doi.org/10.1038/s42256-025-00986-z

Willis, J., & Todorov, A. (2006). First Impressions: Making Up Your Mind After a 100-Ms Exposure to a Face. Psychological Science, 17(7), 592–598. https://doi.org/10.1111/j.1467-9280.2006.01750.x

Wilson, J. P., & Rule, N. O. (2015). Facial trustworthiness predicts extreme criminal-sentencing outcomes. Psychological Science, 26(8), 1325–1331. https://doi.org/10.1177/0956797615590992

Xie, S. Y., Flake, J. K., Stolier, R. M., Freeman, J. B., & Hehman, E. (2021). Facial Impressions Are Predicted by the Structure of Group Stereotypes. Psychological Science, 32(12), 1979–1993. https://doi.org/10.1177/09567976211024259

Yzerbyt, V. Y., Kervyn, N., & Judd, C. M. (2008). Compensation versus halo: The unique relations between the fundamental dimensions of social judgment. Personality and Social Psychology Bulletin, 34(8), 1110–1123. https://doi.org/10.1177/0146167208318602

Zebrowitz, L. A., & McDonald, S. M. (1991). The impact of litigants’ baby-facedness and attractiveness on adjudications in small claims courts. Law and Human Behavior, 15(6), 603–623. https://doi.org/10.1007/BF01065855

Zebrowitz, L. A., & Montepare, J. M. (2008). Social Psychological Face Perception: Why Appearance Matters. Social and Personality Psychology Compass, 2(3), 1497. https://doi.org/10.1111/j.1751-9004.2008.00109.x

Zebrowitz, L. A., Wang, R., Bronstad, P. M., Eisenberg, D., Undurraga, E., Reyes-García, V., & Godoy, R. (2012). First Impressions From Faces Among U.S. and Culturally Isolated Tsimane’ People in the Bolivian Rainforest. Journal of Cross-Cultural Psychology, 43(1), 119–134. https://doi.org/10.1177/0022022111411386

Figure 1. Dual-Route Person Perception Model. A schematic illustrating how facial trait perception derives from two interrelated sources: (1) perceptual features gleaned from bottom-up visual processing (green circle) and (2) conceptual knowledge about the individual (gray circle), which encompasses stereotypes, cultural beliefs, and personal familiarity. The figure shows that these routes jointly shape evaluations along dimensions such as warmth, competence, or criticality. As familiarity with the person increases, conceptual information exerts a stronger influence.
