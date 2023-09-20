
## Section 1 (Behavior Cloning)
Command for problem 1:

### TEST1_BC_ANT

```
python cs285/scripts/run_hw1.py \
	--expert_policy_file cs285/policies/experts/Ant.pkl \
	--env_name Ant-v4 --exp_name bc_ant --n_iter 1 \
	--expert_data cs285/expert_data/expert_data_Ant-v4.pkl \
	--video_log_freq -1 --ep_len 1000 --eval_batch_size 5000
```
### TEST1_BC_ANT

```
python cs285/scripts/run_hw1.py \
	--expert_policy_file cs285/policies/experts/Hopper.pkl \
	--env_name Hopper-v4 --exp_name bc_hopper --n_iter 1 \
	--expert_data cs285/expert_data/expert_data_Hopper-v4.pkl \
	--video_log_freq -1 --ep_len 1000 --eval_batch_size 5000
```



## Section 2 (DAgger)
Command for section 1:
(Note the `--do_dagger` flag, and the higher value for `n_iter`)

### DAGGER_TEST1_ANT

	```
	python cs285/scripts/run_hw1.py \
		--expert_policy_file cs285/policies/experts/Ant.pkl \
		--env_name Ant-v4 --exp_name dagger_ant --n_iter 10 \
		--do_dagger --expert_data cs285/expert_data/expert_data_Ant-v4.pkl \
		--video_log_freq -1
	```

### DAGGER_TEST2_Hopper
	```
	python cs285/scripts/run_hw1.py \
		--expert_policy_file cs285/policies/experts/Hopper.pkl \
		--env_name Hopper-v4 --exp_name dagger_Hopper --n_iter 10 \
		--do_dagger --expert_data cs285/expert_data/expert_data_Hopper-v4.pkl \
		--video_log_freq -1
	```


