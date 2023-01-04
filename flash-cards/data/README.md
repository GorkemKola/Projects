# HARVESTING QA Dataset

This folder contains the one million paragraph-level QA-pairs dataset (split into Train, Dev and Test set) described in:
[Harvesting Paragraph-Level Question-Answer Pairs from Wikipedia](https://arxiv.org/pdf/1805.05942.pdf)
	@@ -7,8 +7,15 @@ This folder contains the one million paragraph-level QA-pairs dataset (split int

[https://goo.gl/a2NzZR](https://goo.gl/a2NzZR)

# SQUAD QA Dataset

combines the 100,000 questions in SQuAD1.1 with over 50,000 unanswerable questions written adversarially by crowdworkers to look similar to answerable ones. To do well on SQuAD2.0, systems must not only answer questions when possible, but also determine when no answer is supported by the paragraph and abstain from answering.

## Dataset Link

[https://huggingface.co/datasets/squad_v2](https://huggingface.co/datasets/squad_v2)

## Format

```
file.json
├── "data"
   └── [i]
       ├── "paragraphs"
       │   └── [j]
       │       ├── "context": "paragraph text"
       │       └── "qas"
       │           └── [k]
       │               ├── "answers"
       │               │   └── [l]
       │               │       ├── "answer_start": N
       │               │       └── "text": "answer"
       │               ├── "id": "<uuid>"
       │               └── "question": "paragraph question?"
       └── "title": "document id"
```

<!--- ## Performance
The Table below shows the neural machine reading system ([DocReader](https://github.com/facebookresearch/DrQA/tree/master/scripts/reader))'s performance on our corpus.

<p align="left"><img width="50%" src="img/performance2.png" /></p>
-->


