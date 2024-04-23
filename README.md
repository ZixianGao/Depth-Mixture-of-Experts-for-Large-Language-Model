# Depth MoE 改动处

## 文件：
```
open_instruct/transformers/models/llama/modeling_llama.py
```

## 改动处：	

1.类LlamaForCausalLM   ：
```
1319-1334行：添加了loss
```
2.类LlamaModel：
```	          
927-929行：增添layer_router初始化
1007-1123行：增加depth MoE的操作
1135-1140行：输出中增加route weight的预测和label
```