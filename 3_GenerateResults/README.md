# Generate Results
This code processes the caption and produces the results

### RQ1 Fail ODD detection

First you should run the human analysis to compute a baseline:

```bash
$ python3 RQ1a_failures_ODD_compare.py --dataset OpenPilot_comma_ai --size 200 --llm_model "vicuna, llama, chat_gpt, human" --baseline human --show_plot
$ python3 RQ1a_failures_ODD_compare.py --dataset OpenPilot_2k19 --size 200 --llm_model "vicuna, llama, chat_gpt, human" --baseline human --show_plot
$ python3 RQ1a_failures_ODD_compare.py --dataset External_jutah --size 200 --llm_model "vicuna, llama, chat_gpt, human" --baseline human --show_plot
```

```bash
python3 RQ1_time_comparison.py
```

```bash
python3 RQ1_human_comparison.py
```

### RQ2 ODD Comparison

Next we want to see what ODD dimensions are most likely to cause failures. To generate these plots you can simply run:

```bash
$ python3 RQ1b_dataset_compare.py --dataset OpenPilot_comma_ai --size 200 --llm_model "vicuna, llama, chat_gpt, human" --pass_fail pass --show_plot
$ python3 RQ1b_dataset_compare.py --dataset OpenPilot_2k19 --size 200 --llm_model "vicuna, llama, chat_gpt, human" --pass_fail pass --show_plot
$ python3 RQ1b_dataset_compare.py --dataset External_jutah --size 200 --llm_model "vicuna, llama, chat_gpt, human" --pass_fail pass --show_plot

$ python3 RQ1b_dataset_compare.py --dataset OpenPilot_comma_ai --size 200 --llm_model "vicuna, llama, chat_gpt, human" --pass_fail fail --show_plot
$ python3 RQ1b_dataset_compare.py --dataset OpenPilot_2k19 --size 200 --llm_model "vicuna, llama, chat_gpt, human" --pass_fail fail --show_plot
$ python3 RQ1b_dataset_compare.py --dataset External_jutah --size 200 --llm_model "vicuna, llama, chat_gpt, human" --pass_fail fail --show_plot
```

# RQ3

```bash
python3 RQ2_ODD_clustering.py --llm_models "vicuna, llama, chat_gpt, human" --size 200 --max_clusters 100 --clustering_iterations 25 --dataset OpenPilot_comma_ai --show_plot
python3 RQ2_ODD_clustering.py --llm_models "vicuna, llama, chat_gpt, human" --size 200 --max_clusters 100 --clustering_iterations 25 --dataset OpenPilot_2k19 --show_plot
python3 RQ2_ODD_clustering.py --llm_models "vicuna, llama, chat_gpt, human" --size 200 --max_clusters 100 --clustering_iterations 25 --dataset External_jutah --show_plot
```