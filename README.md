# Depth-Mixture-of-Experts-for-Large-Language-Model
This is the code for the project Depth-Mixture-of-Experts-for-Large-Language-Model.

## Prepare data：
```
python open_instruct/reformat_datasets.py --dataset evol_codealpaca meta_math SlimOrca WizardLM_evol_instruct_V2_196k
```

## Fine-tuning：	
```
bash scripts/finetune_codealpaca.sh
```

## Evaluation：	
Use the lm-evaluation-harness[https://github.com/hills-code/lm-evaluation-harness/tree/81e9bcc6557dfeb3fea8e40c560532f8108c39fe] library for testing, and check the ranking on the Open-LLM-Leaderboard[https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard].
The script can be used through the following command:
```
bash scripts/leaderboard.sh YOUR_MODEL_PATH YOUR_MODEL_NAME
```      
