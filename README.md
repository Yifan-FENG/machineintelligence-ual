### <em>IU000128 Coding Three: Exploring Machine Intelligence</em>
# Digital Storytelling: Explore AI Ethics by Aritifical Intelligence
##### by Yifan Feng, MA/MSc Computing and Creative Industry (modular)

## Project Overview
This mini project explores two generative models GPT-2 (small) and Char-RNN to investigate their creativity and bias by investigating philosophical discussions on ethics and accoubtability in the AI technologies domain. The first step is to fine tune GPT-2 (small) model on a pre-processed textbook “Oxford Handbook of Ethics of AI” and uses this refined model to generate new content and save them for the next training cycle. The second step is to incoperate GPT-2 (small)-generated content (through the question) into cleaned texbook document and implement Char-RNN model to further create artificial content about ethics. 

## Dataset
The original dataset is [The Oxford Handbook of Ethics of AI](https://www.oxfordhandbooks.com/view/10.1093/oxfordhb/9780190067397.001.0001/oxfordhb-9780190067397). For more information, please check [data folder](https://git.arts.ac.uk/21036265/ExploringMachineIntelligence/tree/main/data). 

The original input source is downloaded as PDF file and converted into plain text file. In the first part of GPT-2 notebook, several data cleaning methods are introduced to re-format input file. Please check [Coding_Three_Part_One.ipynb](https://git.arts.ac.uk/21036265/ExploringMachineIntelligence/blob/main/Coding_three_part_one.ipynb). 

## Training Process & Evaluation 
This Char-RNN/GPT-2(small) text generation starts from examining results after 20 epochs on an M1-Pro Macbook (approx. 50 mins). For detailed implementation & evaluation, please read <em>**[Coding3 technical report](https://git.arts.ac.uk/21036265/ExploringMachineIntelligence/blob/main/Coding3_report_YifanFENG.pdf)**.</em>

## Interactive Exploration 
For interactive technical prototype on Google Colab, please go to [Coding3_PartOne](https://colab.research.google.com/drive/1NPteSsCJ89l697_ztAmcLCU_pGGjzvi5?usp=sharing) and [Coding3_PartTwo](https://colab.research.google.com/drive/1l3z4I9KehQgtLqnOCSWH3m6II_xshuiF?usp=sharing).


## Main Take-away
* Potential bias (in the outcome) correlates highly with input source rather than the model's architecture. 
* The quality of input data file makes a significant effect on the outcome quality. However, increasing data flow and training time can potentially improve the quality of final result for a generative model. 

## Index of .ipynb Notebook
* <em>Code source cited in the notebook</em>

### Coding_three_part_one
##### Main Reference
######
* [Fine-Tuning GPT-2 on a Custom Dataset](https://colab.research.google.com/gist/MattPitlyk/45541145ad48b93da395f0a72ec2e7dc/fine-tuning-gpt-2-on-a-custom-dataset.ipynb) 
* [Beginner’s Guide to Retrain GPT-2 (117M) to Generate Custom Text Content](https://medium.com/ai-innovation/beginners-guide-to-retrain-gpt-2-117m-to-generate-custom-text-content-8bb5363d8b7f)

**1.** Import Libs and Set up Env 

**2.** Basic Text Cleaning

       2.1 Six newly defined functions 
       2.2 Write a new text file 

**3.** GPT-2 Fine-Tuning 

       3.1 Import GPT-2 355Mb version
       3.2 Fine-tuning the model

**4.** Explore Conditional Text

       4.1 Write new text to the cleaned file   
       4.2 Display some results
    

### Coding_three_part_two_updated
##### Main Reference
######
* [char-rnn Trump-like text generation](https://github.com/jctestud/char-rnn) 
* [RNN- Character level text generation with Tensorflow 2.0 from scratch to deep insights](https://geeks-today.medium.com/rnn-character-level-text-generation-with-tensorflow-2-0-from-scratch-to-deep-insights-41bac0e07f86)

**1.** Import Libs and Set up Env 

**2.** Text Processing: from Word to Character 

       2.1 Six newly defined functions 
       2.2 Write a new text file 

**3.** Reconstruct Char-RNN Model 

       3.1 Edit new layers based on the basic model
       3.2 Fine-tine and Reload training weights 

**4.** Explore Conditional Text

       4.1 Define a text generation function 
       4.2 Display some results
