# FreshLLMs


Data and code for our paper [FreshLLMs: Refreshing Large Language Models with Search Engine Augmentation](https://arxiv.org/abs/2310.03214).

## FreshQA


[FreshQA Dec 19, 2023](https://docs.google.com/spreadsheets/d/1VgNv2e12hyTyHFuZ-7F3QzVcdbenA4Sz-W47VaKKTck/edit?usp=sharing).

**Next update:** Dec 26, 2023

We update our dataset weekly or upon request. If you find any updates or misclassifications in our `FreshQA` questions or answers that we may have overlooked, please notify us by commenting on the dataset spreadsheet above or sending an email to freshllms@google.com.

### Automatic evaluation


To facilitate future evaluations, we have developed `FreshEval`, a simple automatic metric that uses few-shot in-context learning to teach an LLM to judge model responses, which achieved high agreement with human raters (see Appendix B in our paper for details).

To use `FreshEval` under a specific evaluation mode (`Relaxed` or `Strict`), please follow the instructions below:

1. Make a copy of our latest data spreadsheet and store it in your Google Drive with a new filename (e.g., `fresheval_relaxed` or `fresheval_strict`).
2. Insert 3 new columns `D`, `E`, `F` in the new spreadsheet for model responses, evaluation rating, evaluation explanation, respectively and save your model's responses in column `D` (see our sample evaluation spreadsheet below).  
3. Run the associated `FreshEval` notebook with the evaluation mode. Note that for demonstration purposes, we evaluated only the first 10 model responses. You can adjust the number as needed. 

Here are our `FreshEval` notebooks.

FreshEval (Relaxed) notebook: [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mFDg-KZQLDSh_drwoXm9VL7ItfreXGJw?usp=sharing)
* [sample evaluation spreadsheet](https://docs.google.com/spreadsheets/d/1rmycAEgBZaPoBbMOlZNJRxd-9yXwmCwt9BrHHx5GbAA/edit?usp=sharing)
* [sample evaluation results](https://docs.google.com/spreadsheets/d/1j6HH879cwGb5ZIT5jFGO47ftoqzmIigz1lQ_g8wTGkA/edit?usp=sharing)

FreshEval (Strict) notebook: [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Euim1Tz-jqT1zuBTkH_RfwpEENp_29R9?usp=sharing)
* [sample evaluation spreadsheet](https://docs.google.com/spreadsheets/d/1QJq8OJwUVz_gd7fP-pAaT_0qcm9oj2__90CjliLQE_s/edit?usp=sharing)
* [sample evaluation results](https://docs.google.com/spreadsheets/d/1pRGQjg8CZVku664H20mSjHwua7EAvSzPcb_Cozwz3yA/edit?usp=sharing)

### Accuracy


After obtaining TRUE/FALSE ratings for model responses, follow these instructions to calculate the accuracy for each question category:

1. Download our latest data spreadsheet in a Comma Separated Values (.csv) format and store it as `freshqa.csv`.
2. Open this notebook [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/18LlmElJkt0joCkkpQffa1UtF9dtUdLmC?usp=sharing) and upload the `freshqa.csv` file to the session storage (`Files > Upload file to session storage`).
3. Replace the existing ratings in the notebook with your ratings and run the notebook.


## FreshPrompt


FreshPrompt notebook: [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RbGXczxI5dn9LjcJm6ndpimELihbjdYL?usp=sharing)

## Acknowledgements


We thank Peter Hart and Filipe Mesquita for their help in updating our `FreshQA` questions/answers.

We are grateful to the following people for their contributions to creating our original FreshQA dataset: Marzena Karpinska, Dustin Tran, Daniel Cer, Sam Fullerton, Elizabeth Clark, Nishant Raj, Xiaoyu Song, Yapei Chang, Yixiao Song, Nader Akoury, Ankita Gupta, Bill Ray, Chau Pham, Wenlong Zhao, Maximilian Mozes, Simeng Sun, Ronan Salz, Kalpesh Krishna, Katherine Thai, Kanishka Misra, Salaheddin Alzu'bi, Erica Cai, Thibault Sellam, Jiao Sun, Dhruv Agarwal, Tessa Masis, Andrew Drozdov, Brian Lester, George Wei, Naveen Jafer Nizar, Shufan Wang, Youngwoo Kim, and Shib Sankar Dasgupta.

## Sponsors


We are grateful to [SerpApi](https://serpapi.com) for their generous sponsorship of 20,000 searches for `FreshPrompt`.

[<img src='serpapi.png' width='50'>](https://serpapi.com)

## Citation


If you use our data or method, please cite our paper:
```bibtex
@misc{vu2023freshllms,
      title={FreshLLMs: Refreshing Large Language Models with Search Engine Augmentation}, 
      author={Tu Vu and Mohit Iyyer and Xuezhi Wang and Noah Constant and Jerry Wei and Jason Wei and Chris Tar and Yun-Hsuan Sung and Denny Zhou and Quoc Le and Thang Luong},
      year={2023},
      eprint={2310.03214},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
