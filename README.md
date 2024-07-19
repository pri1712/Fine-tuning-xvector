# Fine-tuning-xvector
Recipe for finetuning xvectors
1.Run run_xvector script before running the full pipeline. This overwrites the initial final.raw model with our fine-tuned model.

2.Run the full pipeline and in diarize_fbank in 2nd and 3rd stage , it uses the final.raw to extract the x-vectors.
