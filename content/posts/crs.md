---
title: "Biased chats in RecSys"
date: 2022-09-16T17:53:40+01:00
draft: false
---

Recommender systems present a vast set of problems that have all been more than tackled in previous literature: two of the most important ones are fairness and bias.

Conversational AI, on the other hand, is booming. Integrating the conversational element into recommender systems was an almost obvious task to do in terms of importance: these agents move the recommendation in the dialogue space, and make the whole experience much more interactive, precise and overall advanced.

Conversational recommender systems (CRSs) are still pretty new and premature, but this doesn’t mean they are exempted from facing problems. Specifically we need to think more about fairness and bias in CRSs. An interesting study<sup>[1]</sup> has showed how CRSs are not only prone to popularity bias (a well-known bias type in the recsys world) but also to other ones like user preference assumption bias and recommendation evaluation bias.

The first one refers to:

> […] the phenomenon of the user preference elicitation process being dominated by the system only asking the user’s preferences on a small subset of the entire domain-specific attributes. 

while the second is the wrong assumption that success rate (SR@t, the system ability to recommend the ground truth item by turn t) is the ideal evaluation metric for CRS.

The study sums up the need to further investigate bias and fairness in CRSs by posing three important and interesting questions:

To what degree does bias exist in CRSs? And how should we quantify and mitigate it?
Could the preference elicitation process itself be biased?
How should we evaluate a CRS in an unbiased way?
I think these are great starting points for future research and they can lead to increasingly substantial improvements in this technology.

### References

[1] Allen Lin, Ziwei Zhu, Jiangling Wang, James Caverlee. Towards Fair Conversational Recommender Systems. arXiv:2208.03654.
