# EIS-GRPO
Replication of the EIS-GRPO Paper

Paper: J4R: Learning to Judge with Equivalent Initial State Group Relative Policy Optimization

The usage is to replace the **grpo_config.py** and **grpo_trainer.py** file in the TRL library.

## GRPOConfig

```python
training_args = GRPOConfig(
    ...
    num_equivalent_states=4,
    ...
)
```

```num_equivalent_states``` is template number.

## How to change template

Replace on line 885 of **grpo_trainer.py**. Function ```transform_prompt```
