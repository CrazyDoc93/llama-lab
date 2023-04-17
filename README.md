# 🦙🧪  Llama Lab 🧬🦙

Llama Lab is dedicated to hosting cutting-edge project demonstrations, backed by the [LlamaIndex](https://github.com/jerryjliu/llama_index) library!

Each folder is organized into stand-alone examples that showcase how LlamaIndex can be used in different ways.

## Current Labs

### llama_agi

Inspired from [babyagi](https://github.com/yoheinakajima/babyagi), using LlamaIndex as a task manager and LangChain as a task executor.

The current version of this folder will start an with an overall objective ("solve world hunger" by default), and create/prioritize the tasks needed to achieve that objective. LlamaIndex is used to create and prioritize tasks, while LangChain is used to guess the "result" of completing each action.

This will run in a loop until the task list is empty (or maybe you run out of OpenAI credits 😉).

Example Usage:

```python
cd llama_agi
python ./run_llama_agi.py --initial-task "Create a task list" --objective "Solve world hunger" --sleep 2
```

```bash
python ./run_llama_agi.py -h
usage: Llama AGI [-h] [-it INITIAL_TASK] [-o OBJECTIVE] [--sleep SLEEP]

A baby-agi/auto-gpt inspired application, powered by Llama Index!

options:
  -h, --help            show this help message and exit
  -it INITIAL_TASK, --initial-task INITIAL_TASK
                        The initial task for the system to carry out. Default='Create a list of tasks'
  -o OBJECTIVE, --objective OBJECTIVE
                        The overall objective for the system. Default='Solve World Hunger'
  --sleep SLEEP         Sleep time (in seconds) between each task loop. Default=2
```
