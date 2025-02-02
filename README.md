# Multi-view Ranking: Tasking Transformers To Generate And Validate Solutions To Math Word Problems.

## Abstract

The recent developments and success of the Transformer model have resulted in the
creation of massive language models that have led to significant improvements in natural language comprehension.
When fine-tuned for downstream natural language processing tasks with limited data, they achieve state-of-the-art performance.
However, these robust models cannot reason mathematically. It has been
demonstrated that when fine-tuned on the small-scale Math Word Problems (MWPs)
benchmark datasets, these models are not able to generalize.
Therefore, to overcome this limitation, this study proposes to augment the generative
objective used in the MWP task with complementary objectives that can assist the model
in reasoning more deeply about the MWP task. Specifically, we propose a multi-view
generation objective that allows the model to understand the generative task as an
abstract syntax tree traversal beyond the sequential generation task.
In addition, we propose a complementary verification objective to enable the model to
develop heuristics that can distinguish between correct and incorrect solutions. These
two goals comprise our multi-view ranking (MVR) framework, in which the model is
tasked to generate the prefix, infix, and postfix traversals for a given MWP, and then
use the verification task to rank the generated expressions.
Our experiments show that the verification objective is more effective at choosing the
best expression than the widely used beam search. We further show that when our
two objectives are used in conjunction, they can effectively guide our model to learn
robust heuristics for the MWP task. In particular, we achieve an absolute percentage
improvement of 9.7% and 5.3% over our baseline and the state-of-the-art models on
the SVAMP datasets. 

>> Code to be released after publication.
