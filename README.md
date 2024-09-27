# Depth-Mixture-of-Experts-for-Large-Language-Model
This is the code for the project Depth-Mixture-of-Experts-for-Large-Language-Model.

## Prepare data：
```
python open_instruct/reformat_datasets.py --dataset evol_codealpaca meta_math SlimOrca WizardLM_evol_instruct_V2_196k
```

## Fine-tuning：	
```
1319-1334行：添加了loss
```
bash scripts/finetune_codealpaca.sh
```	          
