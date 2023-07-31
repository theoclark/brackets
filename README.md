This project was completed over a weekend as part of the [Alignment Jam Interpretability Hackathon 3.0](https://alignmentjam.com/jam/interpretability). You can see the original submission [here](https://alignmentjam.com/project/who-cares-about-brackets).

We explored the mechanism by which GPT2-small is accurately able to predict a closing bracket having seen an opening bracket earlier in the sequence. It is clear that there is a lot of redundancy in the system and, most interestingly, that the final position does not need to attend directly to the opening bracket in order to make the prediction. The information is largely passed through intermediate positions. The exact mechanism or circuit by which this takes place is unclear.

![fig 1](https://github.com/theoclark/brackets/blob/master/fig1.png)

*Although patching direct attention to the opening bracket reduces the likelihood of predicting a closing bracket, the likelihood remains high*

![fig 2](https://github.com/theoclark/brackets/blob/master/fig2.png)

*We identified heads that may contribute to this circuit but none that remained consistent and held up to scrutiny when approached from different angles*

