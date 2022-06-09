# t5_grammar_checker
T5 Grammar Checker model and workshop, trained using PyTorch FSDP

Goal - train a 800M / 3B / 11B T5 Model to serve as a grammar checker using PyTorch FSDP.  We'll cover both single node (one machine, multi-gpu) and multi-node (2+ machines, each with multi-gpus) training scenarios.  
Result - a trained model that can accept incoming sentences and correct a number of common grammar mistakes.

Examples:</br>
<img width="595" alt="3B_demo_grammar_samples" src="https://user-images.githubusercontent.com/46302957/172918714-8b11944c-0268-4de7-b120-1f993edeb35b.png">



## Getting Started - the environment

For single node, we'll use an A100 (p4dn on AWS) or V100 (p3* on AWS).  
For multi-node, we'll use AWS ParallelCluster and Slurm.  


