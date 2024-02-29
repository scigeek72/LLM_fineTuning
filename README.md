# LLM_fineTuning
Resources on fine tuning LLMs on specific set of data

## Specific quotes from "Fine Tuning Large Language Models" By S.Raschka 

--[Different ways to use LLMs for specific data](https://open.substack.com/pub/sebastianraschka/p/finetuning-large-language-models?r=3vdx8&selection=09194600-1336-4b6d-8f35-48bf0528f559&utm_campaign=post-share-selection&utm_medium=web) by Raschka

--[LLM Fine Tunning ](https://open.substack.com/pub/sebastianraschka/p/finetuning-large-language-models?r=3vdx8&selection=b25098cb-abf4-4638-a138-6c6c40583b60&utm_campaign=post-share-selection&utm_medium=web) by  Raschka

-- There are two(2) types of LLMs: 1) Encoder type (BERT) 2) Decoder type (GPT)

-- Encoder type LLM is more suitable for Classification task (???) while Decoder type LLMs are more suitable for sentence generation (...WARNING: Verify this statement ... )

-- For large LLMs, such as the latest generative models, we can use "[Parameter-Efficient Fine Tuning approach]"(https://open.substack.com/pub/sebastianraschka/p/finetuning-large-language-models?r=3vdx8&selection=e351cc70-a86c-455d-8a90-281fd590ef85&utm_campaign=post-share-selection&utm_medium=web) which is an attempt to reduce the cost associated with training LLMs such as GPTs and BERTs. Raschka's article: [Finetuning LLMs Efficiently with Adapters](https://magazine.sebastianraschka.com/p/finetuning-llms-with-adapters) is an important article (and worth the read).

## Notes from "Finetuning LLMs Efficiently with Adapters"

LLMs such as BERT, GPTs, LLaMA are trained on large corpus of data but they may not perform well on domain specific areas (such as querying product manuals like ours). So finetuning these models on domain specific task will significantly improve their performance. However, they are expensive and time consuming. Hence the adea of "Parameter-Efficeint" finetuning methods.

#### Parameter Efficient Finetuning (with adapters)

The article is [here](https://magazine.sebastianraschka.com/p/finetuning-llms-with-adapters)

Many different types of Parameter Efficient Finetuning exists (such as prompt and prefix tuning). 

Key idea [Prompt Tuning]: add a small number of "new" parameters to a pretrained LLM and only finetune these newly added parameters (and keep the original weights of the LLM frozen) and this makes it cheaper to finetune than finetune the entire model (expensive). 


Key idea [Adapters]: add "tunable layers to the transformer blocks" of LLM instead of modifying prompts as in prompt tuning. 






-- 

## About LLMs

-- [A very nice set of papers for getting into LLMs](https://www.linkedin.com/feed/update/urn:li:activity:7028449312300834816?commentUrn=urn%3Ali%3Acomment%3A%28activity%3A7028449312300834816%2C7028519126105030656%29&dashCommentUrn=urn%3Ali%3Afsd_comment%3A%287028519126105030656%2Curn%3Ali%3Aactivity%3A7028449312300834816%29) By S. Raschka

-- [Building LLM application for production](https://huyenchip.com/2023/04/11/llm-engineering.html) by Chip Huyen
