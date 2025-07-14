# FreshLLMs


Data and code for our paper [FreshLLMs: Refreshing Large Language Models with Search Engine Augmentation](https://arxiv.org/abs/2310.03214).

:star: Our data and method have inspired or been used for the development of recent large language models (LLMs) including [Google's Gemini](https://gemini.google.com), [Perplexity.AI's Online LLMs](https://blog.perplexity.ai/blog/introducing-pplx-online-llms), [You.com](https://about.you.com/introducing-the-you-api-web-scale-search-for-llms), and [Contextual AI's RAG 2.0](https://contextual.ai/introducing-rag2) :star:

:star: We are excited to introduce [SealQA](https://arxiv.org/abs/2506.01062), a new evaluation benchmark that builds on FreshQA with a stronger focus on reasoning. SealQA is available at https://huggingface.co/datasets/vtllms/sealqa and has been used to benchmark recent search-augmented LLMs and search agents, e.g., see [Kimi-Researcher
's blog](https://moonshotai.github.io/Kimi-Researcher/) :star:

Quick links

[FreshQA](https://github.com/freshllms/freshqa?tab=readme-ov-file#freshqa)

[FreshPrompt](https://github.com/freshllms/freshqa?tab=readme-ov-file#freshprompt)

[FreshEval](https://github.com/freshllms/freshqa?tab=readme-ov-file#fresheval)


## FreshQA

[FreshQA July 14, 2025](https://docs.google.com/spreadsheets/d/1B9vaXV7K_2WPAxkO4OuLrN1YS8zOQ0bBFPU5apnUpU0/edit?usp=sharing)

**Next update:** July 21, 2025

We update our dataset weekly or upon request. If you find any updates or misclassifications in our `FreshQA` questions or answers that we may have overlooked, please notify us by commenting on the dataset spreadsheet above or sending an email to freshllms@google.com.


Older versions:

[FreshQA July 7, 2025](https://docs.google.com/spreadsheets/d/1_3Qtf6kILIKzEVRaG4DchNhU5mbAbEGjgl8FX1GzHr8/edit?usp=sharing)

[FreshQA June 23, 2025](https://docs.google.com/spreadsheets/d/19lsv-6YVvsB8nlrhYE1O82LT4TpjLQink8lKYn5Cxmc/edit?usp=sharing)

[FreshQA June 13, 2025](https://docs.google.com/spreadsheets/d/17OhuPWlH2CuL9jgHoVlvQRLYmHlyWvkDpjctgI7VX3Y/edit?usp=sharing)

[FreshQA June 5, 2025](https://docs.google.com/spreadsheets/d/1Udty_LnNp1l97rJBvmFWRP9hTR1uhDq3amCPbCFd2Sg/edit?usp=sharing)

[FreshQA May 6, 2025](https://docs.google.com/spreadsheets/d/1gg7tOqVvae8cYHbZWsbTkr0RRQFXQqVrIPbO_VIvy-4/edit?usp=sharing)

[FreshQA April 28, 2025](https://docs.google.com/spreadsheets/d/1GjyHES7YDEbcVsrXx8dBxSG6mfYBeBqpRAB5a0MWouA/edit?usp=sharing)

[FreshQA April 14, 2025](https://docs.google.com/spreadsheets/d/1ME3i1Ln1eVOpAZMOFvIU5q2FpTw_xR-Zz_hqH3RrvAE/edit?usp=sharing)

[FreshQA April 7, 2025](https://docs.google.com/spreadsheets/d/1tSq24yACs1CrwzyUh1tg8U7Ej2CUcQYNjrGZgn4UtEI/edit?usp=sharing)

[FreshQA March 31, 2025](https://docs.google.com/spreadsheets/d/1wphfq_HQTmKghWGMAL18dyo4ZLTcjEuTmmnMEOtZxI4/edit?usp=sharing)

[FreshQA March 24, 2025](https://docs.google.com/spreadsheets/d/1kJuCOHe4p3RBvNUxIlA5fBg7fzOxWm0fgi1Y50jrCm8/edit?usp=sharing)

[FreshQA March 17, 2025](https://docs.google.com/spreadsheets/d/1PWYzWFXY4Oa6hCVJqd_2ac9FaQMoEeUazXy928tgQIA/edit?usp=sharing)

[FreshQA March 10, 2025](https://docs.google.com/spreadsheets/d/1pR1ETI3cX9_295HhfPfRUOHNlEYE5aJhbNFqN7DJ5Xk/edit?usp=sharing)

[FreshQA March 03, 2025](https://docs.google.com/spreadsheets/d/1IcgM8cRmW8Xa2RDIiTuMvZgyogB1fc9oSSNaJfURPhk/edit?usp=sharing)

[FreshQA February 24, 2025](https://docs.google.com/spreadsheets/d/1e_0mORRXJsCgLR2ZaaBWm2tzfWB2msjQ---a9jaBZnE/edit?usp=sharing)

[FreshQA February 17, 2025](https://docs.google.com/spreadsheets/d/12aWIs2Vw8mlrs6iKfuEj_ZEDoW10wEfQ2N0qy2raPA8/edit?usp=sharing)

[FreshQA February 10, 2025](https://docs.google.com/spreadsheets/d/1LWf-6NIYtmi_Eu6VTGexwLH4V0A5vncRASAdVRxRDLo/edit?usp=sharing)

[FreshQA February 03, 2025](https://docs.google.com/spreadsheets/d/1t3n4vP3-49-_lz8nHaH5JXC21s_EfhxqL1vI3bhPEnU/edit?usp=sharing)

[FreshQA December 18, 2024](https://docs.google.com/spreadsheets/d/1llFQDYuwX95L7yYDQ4aLCwJmkEh9VOSHNu6g7HjT8e0/edit?usp=sharing)

[FreshQA December 09, 2024](https://docs.google.com/spreadsheets/d/1MAli0K89SfYq_hFv7J6DhiU2Ovbu9xirksaK7v_YEuY/edit?usp=sharing)

[FreshQA December 02, 2024](https://docs.google.com/spreadsheets/d/1jSRMJTyYTuoavS-f6LRPdkD8ndNtHokGzBjFfFxHgXg/edit?usp=sharing)

[FreshQA November 25, 2024](https://docs.google.com/spreadsheets/d/1d7clVEos4LNy0oJ61QYwrXUVN4LG-APtszjAC0As-i8/edit?usp=sharing)

[FreshQA November 18, 2024](https://docs.google.com/spreadsheets/d/1o1Hcpjqn4jZmQBL-kqbwsm7zK_vpaYmehHODalMHGdQ/edit?usp=sharing)

[FreshQA November 4, 2024](https://docs.google.com/spreadsheets/d/1JtSVXl5M5xT-fyEF32uI2YRozMjP1RIICB7zYGC9gLI/edit?usp=sharing)

[FreshQA October 28, 2024](https://docs.google.com/spreadsheets/d/1j6qr14l8oK_7gJ_XdnTBi8Pj1NVt5yeQEBKxFPkKn_g/edit?usp=sharing)

[FreshQA October 21, 2024](https://docs.google.com/spreadsheets/d/13McP8V9S5bHqwNj-Bc8-2iy6NnsPAqoPdT_U2rPnf4A/edit?usp=sharing)

[FreshQA October 14, 2024](https://docs.google.com/spreadsheets/d/1L6iHkseRKNrx32iYA5ptiwf8rbM0S1W3zgcLTqXqdEE/edit?usp=sharing)

[FreshQA October 7, 2024](https://docs.google.com/spreadsheets/d/1yvTJzfD5Rf64gd0xSekfK0yGHaAIv-nOZenKYfoAT_0/edit?usp=sharing)

[FreshQA September 30, 2024](https://docs.google.com/spreadsheets/d/1mNW3QOlQmujaOn-9BKrD6ujhJr4MGjkgmSKKedKeU8E/edit?usp=sharing)

[FreshQA September 23, 2024](https://docs.google.com/spreadsheets/d/1PnCh2Tg_K4eRdpbe-nnN9REMoK8QGdKAQ4KrNNBPhWA/edit?usp=sharing)

[FreshQA September 16, 2024](https://docs.google.com/spreadsheets/d/1739rsb_Lzm7EMxYzGHxsuBMzetLCdMHKsYUA0LwvWlQ/edit?usp=sharing)

[FreshQA September 5, 2024](https://docs.google.com/spreadsheets/d/19Fn-lqkrZsJt4I6EpAGn0dm2tBcfz_86dKWT3VkERLo/edit?usp=sharing)

[FreshQA August 26, 2024](https://docs.google.com/spreadsheets/d/1l6gLnJvHPHL80RM2FtNumkD6szsvtp8E7JV7cR61lX0/edit?usp=sharing)

[FreshQA August 19, 2024](https://docs.google.com/spreadsheets/d/1XDgfCx2sOG4JVP9aFUfny7dd2jYnse6fEdSTIptPDoo/edit?usp=sharing)

[FreshQA August 12, 2024](https://docs.google.com/spreadsheets/d/19bl0W9bw2Ro3I0SjTu8G-y49-ZJVN2dHyEnC-M82gDY/edit?usp=sharing)

[FreshQA August 2, 2024](https://docs.google.com/spreadsheets/d/1gQ8VKZJSAoZATWO1sdnmmQaSuhtQH2pVUwexKkHIxfQ/edit?usp=sharing)

[FreshQA July 26, 2024](https://docs.google.com/spreadsheets/d/18cz7kmmQFk3jHbowOrzTGjPusdb5GnFEZYKXQL-girw/edit?usp=sharing)

[FreshQA July 19, 2024](https://docs.google.com/spreadsheets/d/1aHg4rFTYNtgYXFERDLXTsoYCPvfuZkenflrwPLjMPnU/edit?usp=sharing)

[FreshQA July 11, 2024](https://docs.google.com/spreadsheets/d/16x3-m3iLRk5ljK_93EKxhOFRLf8o2L4sqmKZO0CkhU8/edit?usp=sharing)

[FreshQA July 3, 2024](https://docs.google.com/spreadsheets/d/1hJPGja3DuUSkVROoIZGfjZroGFugqT-AO6bzbREQDlI/edit?usp=sharing)

[FreshQA June 24, 2024](https://docs.google.com/spreadsheets/d/11oqtBYZiO0I0niWLJqo6shQRCinwLSczNIGSq9hafbQ/edit?usp=sharing)

[FreshQA June 17, 2024](https://docs.google.com/spreadsheets/d/1ONVJy_f1WdCVJ_N9mmHfOpJPQ-eC8eK4oekjCBHDygY/edit?usp=sharing)

[FreshQA June 10, 2024](https://docs.google.com/spreadsheets/d/1PDLReKlbKxbnu66v_-PKoxqx50OdiYhHc192kYnaqWI/edit?usp=sharing)

[FreshQA June 3, 2024](https://docs.google.com/spreadsheets/d/1GxL0kr0IC3kDeisjxPLRHgM5uOhDFVgDpqcINibD0uk/edit?usp=sharing)

[FreshQA May 27, 2024](https://docs.google.com/spreadsheets/d/1cPtDoCgBG3weih7AuAnXk9jsgEH8XMWYHzKMD1OgX-4/edit?usp=sharing)

[FreshQA May 20, 2024](https://docs.google.com/spreadsheets/d/1EWc3w_dBfJONl_HtL7LtRsmZ-XYi-gKFCkUZAs62o_I/edit?usp=sharing)

[FreshQA May 13, 2024](https://docs.google.com/spreadsheets/d/1p0qXk1iqSwV9Pq2DpivwtxfKUjLyK_n-k3jgtlDb_54/edit?usp=sharing&resourcekey=0-rddWsLSn8JaYS1PygZPVYw)

[FreshQA May 10, 2024](https://docs.google.com/spreadsheets/d/166xjz7rGaN3MaeimuZJBbEXPzT8PvEpHBno7iJ2obss/edit?usp=sharing)

[FreshQA May 6, 2024](https://docs.google.com/spreadsheets/d/1i1vqjOvGh2LQ9L_AimalzezuU-AQDANubvh4OE-iJcs/edit?usp=sharing)

[FreshQA Apr 29, 2024](https://docs.google.com/spreadsheets/d/1qWhTS1aR57eHa6LQlYyJKEnXaItlQ0_19vYrIPxMtI0/edit?usp=sharing)

[FreshQA Apr 22, 2024](https://docs.google.com/spreadsheets/d/1dI54REjfTpFCrvpXvpO1D1QeAXRuTrLbvenjklmuj8k/edit?usp=sharing)

[FreshQA Apr 15, 2024](https://docs.google.com/spreadsheets/d/1c5pn-FIFZl4MV02dEZ-_R2JsKywD7ZzL7dfG2T-OGt4/edit?usp=sharing)

[FreshQA Apr 8, 2024](https://docs.google.com/spreadsheets/d/1nDEWXXG2VcXEktYiLhQ8QWmw4DFshiodgGh6A4dlgUQ/edit?usp=sharing)

[FreshQA Apr 1, 2024](https://docs.google.com/spreadsheets/d/1L9V0pRqyBl1476zyQh32NquCnv7-pe3Y7VOfGPwQTDo/edit?usp=sharing)

[FreshQA Mar 25, 2024](https://docs.google.com/spreadsheets/d/1DLTGhLCmOgau-np1oQqoeRRyd7Ow6y0bJHmNFrsPmeQ/edit?usp=sharing)

[FreshQA Mar 18, 2024](https://docs.google.com/spreadsheets/d/13tzqv1oquj-GvdCkWlS13lmVaZqhWQ61CIDE1Ngh71A/edit?usp=sharing)

[FreshQA Mar 11, 2024](https://docs.google.com/spreadsheets/d/1wuaanfgOA4cHodseXs6H4MBTsRs5JaUbnqleo7o4vPM/edit?usp=sharing)

[FreshQA Mar 4, 2024](https://docs.google.com/spreadsheets/d/1ta7vIcCxShdFWEPY2AMt-F1DFmpfa2j0wewwJO3mC60/edit?usp=sharing)

[FreshQA Feb 26, 2024](https://docs.google.com/spreadsheets/d/1V6nIxVTI9tqZ-wfgK-uFuUPiGEa1Zmnz53OeGbaNtO0/edit?usp=sharing)


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


We thank Hailey Joren, William Zhang, Varun Singh, Peter Hart, and Filipe Mesquita for their help in updating our `FreshQA` questions/answers.

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
