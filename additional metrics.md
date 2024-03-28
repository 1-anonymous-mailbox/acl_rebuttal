To further demonstrate the effectiveness of our KPDD, we will list the model's performance on additional evaluation metrics below. Although these metrics are also commonly used to evaluate dialogue tasks, past research [3] [4] has shown that metrics such as BLEU and ROUGE focus on the consistency between generated responses and the gold responses, which is more suitable for tasks like translation rather than flexible dialogue generation tasks. This is also why we did not include these metrics in the paper.

[3] Song H, Zhang W N, Cui Y, et al. Exploiting persona information for diverse generation of conversational responses[J]. IJCAI, 2019.

[4] Tang Y, Wang B, Fang M, et al. Enhancing personalized dialogue generation with contrastive latent variables: Combining sparse and dense persona[J]. ACL, 2023.

|            | BLEU-2    | BLEU-4    | ROUGE-L   | PPL       |
| ---------- | --------- | --------- | --------- | --------- |
| BART       | 0.086     | 0.028     | 0.164     | 46.89     |
| Llama2     | 0.104     | 0.035     | 0.217     | 40.74     |
| Multi-GPT2 | 0.092     | 0.021     | 0.198     | 57.89     |
| $D^3$      | 0.112     | 0.039     | 0.206     | 38.91     |
| SimOAP     | 0.097     | 0.034     | 0.187     | 61.23     |
| LMEDR      | 0.085     | 0.027     | 0.160     | 35.25     |
| KPDD       | **0.131** | **0.046** | **0.223** | **30.72** |

It can be seen that our KPDD also has a clear advantage in metrics such as BLEU-2/BLEU-4/ROUGE-L/PPL.