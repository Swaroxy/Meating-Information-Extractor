Our project is a Meeting Intelligence Extractor. It takes meeting transcripts and uses LLMs to extract useful information automatically.
Workflow diagram
1. Meeting Transcript
Sample meeting text
2. Prompt Engineering
System prompts, examples, JSON format, versions V1–V4
3. LLM Processing
Local Qwen 0.5B and hosted Qwen 7B
4. Validate & Evaluate
Check JSON, compare prompts, measure latency and recall
5. Meeting Intelligence Output
Summary, decisions, action items and open questions
What each tool does
Python: Runs the complete workflow in the notebook.
Hugging Face Transformers + PyTorch: Run the smaller LLM locally.
Hugging Face Inference API: Access the larger hosted LLM.
Prompt engineering: Tests different instructions and examples to improve extraction.
JSON parsing and validation: Checks whether the model's response follows the expected structure.
Evaluation code: Compares prompt performance, keyword recall, token usage and response time.
prompts_registry.json: Stores prompt versions for reuse and comparison.
In simple words: We have built a system that extracts structured meeting information, compares two LLM approaches, experiments with prompt versions, and evaluates their results. It is also a practical lab for learning prompt engineering and LLM evaluation.

