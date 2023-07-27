# Summarizing dialogue with generative AI
This tutorial shows how you can load a pre-trained Large Language Model (LLM) from Hugging Face; improve its completion performance for dialogue summarization with prompt engineering (zero-, one-, and few-shot inference); refine the model with full and parameter-efficient fine-tuning; and, finally, use Reinforcement Learning with Human Feedback (RLHF) to make its responses less toxic. 

The actual models trained in the script only use 1/100th of the Dialogsum dataset, so the script is essentially a toy example of how these steps are performed. In principle, though, given enough compute resources it would work with an actual dataset :)

More details: the script uses the Dialogsum dataset (10,000+ short dialogues with human-annotated summaries) and the FLAN-T5 language model, i.e., the T5 model improved with the Fine-Tuned Language Net (FLAN) method for better performance with various language tasks.

The Parameter-Efficient Fine Tuning method I used is LoRA (Low-Rank Adaptation).

Finally, the reinforcement model used towards the end to "detoxify" the model comes from the Roberta Toxicity Classifier (see https://huggingface.co/s-nlp/roberta_toxicity_classifier)
