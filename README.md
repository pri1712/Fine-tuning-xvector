# Fine-tuning-xvector
Recipe for finetuning xvectors
1.Run run_xvector script before running the full pipeline. This overwrites the initial final.raw model with our fine-tuned model.

2.Run the full pipeline and in diarize_fbank in 2nd and 3rd stage , it uses the final.raw to extract the x-vectors.

**CURRENT RESULTS**:

The results obtained are as expected as the current PLDA model is not tuned for the newly tuned embedding extractor, thus it leads to a DER of **65 on DEV data without any resegmentation**.

**FUTURE WORK:**

1. Need to train the PLDA model so it reflects the tuned xvectors, this would potentially lead to a better DER as our PLDA Model would then reflect the newly obtained xvectors.
