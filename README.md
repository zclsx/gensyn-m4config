# gensyn-m4config


```
model_name_or_path: Gensyn/Qwen2.5-0.5B-Instruct  
model_revision: main  
torch_dtype: float32  
attn_implementation: default  
bf16: false  
tf32: false  
output_dir: runs/gsm8k/multinode/Qwen2.5-0.5B-Instruct-Gensyn-Swarm  
  
dataset_id_or_path: 'openai/gsm8k'  
  
max_steps: 50  
per_device_train_batch_size: 1  
gradient_accumulation_steps: 5  
gradient_checkpointing: true  
gradient_checkpointing_kwargs:  
use_reentrant: true  
learning_rate: 5.0e-6  
lr_scheduler_type: cosine  
warmup_ratio: 0.1  
beta: 0.001  
max_prompt_length: 96  
max_completion_length: 96  
num_generations: 1  
use_vllm: false  
vllm_gpu_memory_utilization: 0.5  
  
device: mlx_gpu  
  
logging_strategy: steps  
logging_steps: 10  
report_to:  
- tensorboard  
save_strategy: steps  
save_steps: 100  
seed: 42  
  
max_rounds: 10000  
max_grad_norm: 0.5

```
