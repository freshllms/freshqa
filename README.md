# FreshLLMs


Data and code for our paper [FreshLLMs: Refreshing Large Language Models with Search Engine Augmentation](https://arxiv.org/abs/2310.03214).

:star: Our data and method have inspired or been used for the development of recent large language models (LLMs) including [Google's Gemini](https://gemini.google.com), [Perplexity.AI's Online LLMs](https://blog.perplexity.ai/blog/introducing-pplx-online-llms), [You.com](https://about.you.com/introducing-the-you-api-web-scale-search-for-llms), and [Contextual AI's RAG 2.0](https://contextual.ai/introducing-rag2) :star:

Quick links

[FreshQA](https://github.com/freshllms/freshqa?tab=readme-ov-file#freshqa)

[FreshPrompt](https://github.com/freshllms/freshqa?tab=readme-ov-file#freshprompt)

[FreshEval](https://github.com/freshllms/freshqa?tab=readme-ov-file#fresheval)


## FreshQA

[FreshQA Apr 1, 2024](https://docs.google.com/spreadsheets/d/1L9V0pRqyBl1476zyQh32NquCnv7-pe3Y7VOfGPwQTDo/edit?usp=sharing)

**Next update:** Apr 8, 2024

Older versions:

[FreshQA Mar 25, 2024](https://docs.google.com/spreadsheets/d/1DLTGhLCmOgau-np1oQqoeRRyd7Ow6y0bJHmNFrsPmeQ/edit?usp=sharing)

[FreshQA Mar 18, 2024](https://docs.google.com/spreadsheets/d/13tzqv1oquj-GvdCkWlS13lmVaZqhWQ61CIDE1Ngh71A/edit?usp=sharing)

[FreshQA Mar 11, 2024](https://docs.google.com/spreadsheets/d/1wuaanfgOA4cHodseXs6H4MBTsRs5JaUbnqleo7o4vPM/edit?usp=sharing)

[FreshQA Mar 4, 2024](https://docs.google.com/spreadsheets/d/1ta7vIcCxShdFWEPY2AMt-F1DFmpfa2j0wewwJO3mC60/edit?usp=sharing)

[FreshQA Feb 26, 2024](https://docs.google.com/spreadsheets/d/1V6nIxVTI9tqZ-wfgK-uFuUPiGEa1Zmnz53OeGbaNtO0/edit?usp=sharing)

We update our dataset weekly or upon request. If you find any updates or misclassifications in our `FreshQA` questions or answers that we may have overlooked, please notify us by commenting on the dataset spreadsheet above or sending an email to freshllms@google.com.


## FreshPrompt


FreshPrompt notebook: [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1YKL3wN1LdaY5Aqlz8IRlag7zzMr7FSTQ?usp=sharing)


## FreshEval


We believe that human evaluators possess the expertise and common sense required to detect issues like hallucinations, making them more reliable than automated evaluation metrics for assessing LLMs' factuality. However, researchers have the flexibility to adjust their evaluation methods if human evaluation proves challenging. An easily implemented alternative is to use standard metrics like F1/exact match or recall, which assess the overlap between the model response and the ground truth answer(s) (e.g., see You.com's recent [blog](https://about.you.com/introducing-the-you-api-web-scale-search-for-llms) where they report `FreshQA` recall). Researchers can also use LLM-based automatic evaluation metrics such as [FactScore](https://arxiv.org/abs/2305.14251) or our `FreshEval` metric below.

### Automatic evaluation


To facilitate future evaluations, we have developed `FreshEval`, a simple automatic metric that uses few-shot in-context learning to teach an LLM to judge model responses, which achieved high agreement with human raters (see Appendix B in our paper for details).

To use `FreshEval` under a specific evaluation mode (`Relaxed` or `Strict`), please follow the instructions below:

1. Make a copy of our latest data spreadsheet and store it in your Google Drive with a new filename (e.g., `fresheval_relaxed` or `fresheval_strict`).
2. Insert 3 new columns `D`, `E`, `F` in the new spreadsheet for model responses, evaluation rating, evaluation explanation, respectively and save your model's responses in column `D` (see our sample evaluation spreadsheet below).  
3. Run the associated `FreshEval` notebook with the evaluation mode. Note that for demonstration purposes, we evaluated only the first 10 model responses. You can adjust the number as needed. 

**Note:** Currently, we recommend `gpt-4-1106-preview` over `gpt-4-0125-preview` for `FreshEval` as it yielded slightly better agreement with human annotations in our small-scale evaluation.

Here are our `FreshEval` notebooks.

FreshEval (Relaxed) notebook: [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mFDg-KZQLDSh_drwoXm9VL7ItfreXGJw?usp=sharing)
* [sample evaluation spreadsheet](https://docs.google.com/spreadsheets/d/1rmycAEgBZaPoBbMOlZNJRxd-9yXwmCwt9BrHHx5GbAA/edit?usp=sharing)
* [sample evaluation results](https://docs.google.com/spreadsheets/d/1j6HH879cwGb5ZIT5jFGO47ftoqzmIigz1lQ_g8wTGkA/edit?usp=sharing)

FreshEval (Strict) notebook: [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Euim1Tz-jqT1zuBTkH_RfwpEENp_29R9?usp=sharing)
* [sample evaluation spreadsheet](https://docs.google.com/spreadsheets/d/1QJq8OJwUVz_gd7fP-pAaT_0qcm9oj2__90CjliLQE_s/edit?usp=sharing)
* [sample evaluation results](https://docs.google.com/spreadsheets/d/1pRGQjg8CZVku664H20mSjHwua7EAvSzPcb_Cozwz3yA/edit?usp=sharing)

After obtaining TRUE/FALSE ratings for model responses, follow the instructions below to calculate the accuracy for each question category:

1. Download our latest data spreadsheet in a Comma Separated Values (.csv) format and store it as `freshqa.csv`.
2. Open this notebook [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/18LlmElJkt0joCkkpQffa1UtF9dtUdLmC?usp=sharing) and upload the `freshqa.csv` file to the session storage (`Files > Upload file to session storage`).
3. Replace the existing ratings in the notebook with your ratings and run the notebook.


## Acknowledgements


We thank William Zhang, Varun Singh, Peter Hart, and Filipe Mesquita for their help in updating our `FreshQA` questions/answers.

We are grateful to the following people for their contributions to creating our original FreshQA dataset: Marzena Karpinska, Dustin Tran, Daniel Cer, Sam Fullerton, Elizabeth Clark, Nishant Raj, Xiaoyu Song, Yapei Chang, Yixiao Song, Nader Akoury, Ankita Gupta, Bill Ray, Chau Pham, Wenlong Zhao, Maximilian Mozes, Simeng Sun, Ronan Salz, Kalpesh Krishna, Katherine Thai, Kanishka Misra, Salaheddin Alzu'bi, Erica Cai, Thibault Sellam, Jiao Sun, Dhruv Agarwal, Tessa Masis, Andrew Drozdov, Brian Lester, George Wei, Naveen Jafer Nizar, Shufan Wang, Youngwoo Kim, and Shib Sankar Dasgupta.

We are also grateful to SerpApi for their generous sponsorship of 10,000 searches for `FreshPrompt`'s users upon its release.


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
