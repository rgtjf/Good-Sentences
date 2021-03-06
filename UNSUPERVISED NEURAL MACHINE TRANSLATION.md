# UNSUPERVISED NEURAL MACHINE TRANSLATION

## Related Work
- In spite of [the recent success of neural machine translation], the lack of [large parallel corpora] poses a major practical problem for [many language pairs].
- alleviate this issue
- relying (solely) on nothing but [monolingual corpora]
- using a combination of [denoising] and [back-translation]


## Introduction

- background -> problem -> in this work -> results
- The remaining of this paper is organized as follows. Section 2 analyzes the related work. Section 3 then describes the proposed method. The experimental settings are discussed in Section 4, while Section 5 presents and discusses the obtained results. Section 6 concludes the paper

## Related Work

- We will first discuss unsupervised cross-lingual embeddings, hich are the basis of our proposal, in Section 2.1. Section 2.2 then addresses statistical decipherment, an SMT-inspired approach to build a machine translation system in an unsupervised manner. Finally, Section 2.3 presents previous work on training NMT systems in different low-resource scenarios.

- Closer to our scenario, embedding mapping methods independently rain the embeddings in different languages using monolingual corpora, and then learn a linear transformation that maps them to a shared space based on a bilingual dictionary

- They model the process by which this ciphertext is generated as a two-state process **involving** the generation of the original English sequence and the probabilistic replacement of the words in it.

- To the best of our knowledge, the more ambitious scenario where [an NMT model is trained on monolingual corpora alone] has never been explored to data, but [He et al. (2016)] made an important contribution in this direction. More concretely, ...


## model
- 总起：This section describes the proposed unsupervised NMT approach. Section 3.1 first presents the architecture of the proposed system, and Section 3.2 then describes the method to train it in an unsupervised manner.

- 具体来说：More concretely / Specifically / In particular

- 注意：Note that, even if ..., we ...

- 目的：For that purpose, [We alter the word order of the input sequence by making random swaps between continuous words]

- 进一步解释：At the same time, by doing ..., we can better account for ...

- 缺点：without considering sth


## Expriments

## results

- We **thus conclude that** both denoising and backtranslation **play an essential role** during training: denoising **forces** the system to capture broad word-level equivalences, while backtranslation **encourages it** to learn more subtle relations in an increasingly natural setting.

- As for the role of [subword translation], we observe that BPE is slightly beneficial

- 不一致：Having a closer look, however, we observe that, while ..., it also introduces some errors. In particular, 

- For instance / For example

- 局限性：[sth] may also be a factor limiting its potential performance.

### QUALITATIVE ANALYSIS 
- 起：In order to better understand the behavior of the proposed system, we manually analyzed some translations for French->English, and present some illustrative examples in Table 2.

- 好的：Our analysis shows that the proposed system is able to roduce high-quality translations, adequately modeling non-trivial translation relations. For instance,

- 缺点：Nevertheless, our analysis also points that the proposed system has limitations and, perhaps not surprisingly, its translation quality often lags behind that of a standard  upervised NMT system. In particular, ...

- Finally, there are also some cases where there are both fluency and adequacy problems that severely hinders understanding the original message from the proposed translation. For instance,...


## Conclusions
This Work -> Expriments -> Future work
