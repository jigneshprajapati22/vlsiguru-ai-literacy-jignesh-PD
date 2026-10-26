# AI Tools Exploration

## 1. Tools and intended uses

| Tool | Intended use explored | Example task |
|---|---|---|
| ChatGPT | Beginner-friendly explanations, coding help, and quizzes | Explain Python functions with an example |
| Google Gemini | Explanations and research assistance | Explain supervised versus unsupervised learning |
| Claude | Text analysis, reasoning, and coding support | Review a Python function and explain possible errors |
| NotebookLM | Asking questions about supplied sources and study notes | Turn lecture notes into revision questions |
| Perplexity | Research and source discovery | Find documentation for open-source EDA tools |

Official websites:
- ChatGPT: https://chatgpt.com/
- Gemini: https://gemini.google.com/
- Claude: https://claude.ai/
- NotebookLM: https://notebooklm.google.com/
- Perplexity: https://www.perplexity.ai/

## 2. Prompt examples and refinement

### Prompt 1 — Beginner-friendly explanation

**Initial prompt:**  
“Explain machine learning.”

**Refined prompt:**  
> Explain machine learning in beginner-friendly language. Use a real-world example, explain how training data is used, and describe one limitation. Keep the answer concise and include a simple analogy.

**Why the refinement helps:** It specifies the audience, desired details, and response length.

### Prompt 2 — Engineering applications

**Initial prompt:**  
“Explain AI in engineering.”

**Refined prompt:**  
> Explain three applications of AI in semiconductor engineering for a beginner. For each application, describe the engineering problem, how AI may help, one limitation, and one example. Present the answer in a table and distinguish established applications from emerging research.

**Why the refinement helps:** It adds context, constraints, and a clear output format.

### Prompt 3 — Quiz and feedback

> Quiz me on Python functions, lists, loops, and basic machine learning. Ask one question at a time, wait for my answer, explain mistakes, and gradually increase the difficulty.

## 3. Compare two tools on the same question

**Question to ask both ChatGPT and Gemini:**  
“Explain the difference between supervised and unsupervised machine learning, with one engineering example of each.”

Record the actual responses here after running the prompt in both tools.

| Criterion | Tool 1: ChatGPT | Tool 2: Gemini |
|---|---|---|
| Clarity for a beginner | Add your observation | Add your observation |
| Technical accuracy | Verify definitions and examples | Verify definitions and examples |
| Engineering relevance | Add your observation | Add your observation |
| Useful sources provided | Add your observation | Add your observation |

**Comparison note:** Do not assume either answer is correct just because it sounds confident. Compare the explanations and verify technical claims against reliable sources.

## 4. Example of a claim checked

**Claim:** OpenROAD supports stages of digital physical design such as floorplanning, placement, clock-tree synthesis, and routing.

**Source:** OpenROAD official documentation:  
https://openroad.readthedocs.io/en/latest/main/README.html

**Conclusion:** The official documentation describes these physical-design operations, so it supports the claim that OpenROAD can automate significant parts of digital chip implementation. The exact steps and results depend on the design, technology files, constraints, and flow configuration.

## 5. Example of technical learning

- **Supervised learning** uses labelled examples. An engineering example is classifying component images as defective or non-defective using labelled training images.
- **Unsupervised learning** identifies patterns in data without predefined labels. An example is clustering manufacturing measurements to identify groups of similar operating conditions.

AI outputs should be checked against authoritative documentation, especially for technical or safety-relevant decisions.

## 6. Evidence to add

- Paste short excerpts or summaries from the two actual tool responses.
- Record one difference you observed.
- Note the source used to verify the claim and what it established.
- Include any follow-up prompt that improved the answer.

