# Lottery Prompt Tuning

This repository is the Pytorch implementation of our paper "[Prompts Can Play Lottery Tickets Well: Achieving Lifelong Learning Information Extraction via Lottery Prompt Tuning](https://aclanthology.org/2023.acl-long.16.pdf)" in ACL 2023.

In this paper, we study the UIE system under a more challenging yet practical scenario, i.e., “lifelong learning” settings, to evaluate its abilities in three aspects, including knowledge sharing and expansion, catastrophic forgetting prevention, and rapid generalization on few-shot and unseen tasks. To achieve these three goals, we present a novel parameter- and deployment-efficient prompt tuning method namely Lottery Prompt Tuning (LPT). LPT freezes the PLM’s parameters and sequentially learns compact pruned prompt vectors for each task leveraging a binary prompt mask, while keeping the prompt parameters selected by the previous tasks insusceptible.

Coming soon!


## Citation

If you find this paper helps your research, please kindly consider citing our paper in your publications.

```BibTeX
@inproceedings{liang-etal-2023-prompts,
    title = "Prompts Can Play Lottery Tickets Well: Achieving Lifelong Information Extraction via Lottery Prompt Tuning",
    author = "Liang, Zujie  and
      Wei, Feng  and
      Jie, Yin  and
      Qian, Yuxi  and
      Hao, Zhenghong  and
      Han, Bing",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.acl-long.16",
    doi = "10.18653/v1/2023.acl-long.16",
    pages = "277--292",
    abstract = "Thanks to the recent success of Pre-trained Language Models (PLMs), it has become a promising research direction to develop a universal model (UIE) that can solve all typical information extraction tasks within one generative framework. Nonetheless, in real-world scenarios of UIE applications, new data of different IE tasks and domains usually come in a stream over time. A desirable UIE system should be capable of continually learning new tasks without forgetting old ones, thereby allowing knowledge and functionalities expansion without re-training the whole system. In this paper, we study the UIE system under a more challenging yet practical scenario, i.e., {``}lifelong learning{''} settings, to evaluate its abilities in three aspects, including knowledge sharing and expansion, catastrophic forgetting prevention, and rapid generalization on few-shot and unseen tasks.To achieve these three goals, we present a novel parameter- and deployment-efficient prompt tuning method namely Lottery Prompt Tuning (LPT).LPT freezes the PLM{'}s parameters and sequentially learns compact pruned prompt vectors for each task leveraging a binary prompt mask, while keeping the prompt parameters selected by the previous tasks insusceptible.Furthermore, we use a simple yet effective method to perform mask selection and show the powerful transferability of Lottery Prompts to novel tasks.Extensive experiments demonstrate that LPT consistently sets state-of-the-art performance on multiple lifelong learning settings of UIE, including task-incremental setting on seen tasks, few-shot adaptation, and zero-shot generalization on novel tasks.",
}
```
