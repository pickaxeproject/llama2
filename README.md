# Our process for fine-tuning Llama 2 with custom data

We successfully trained **LLaMA-2-7b-hf** on a custom dataset to perform a *single, routine task* (keyword extraction). We thought this would be easy, but it was WAY HARDER than we expected. We went down a lot of wrong turns, and many of the notebooks/code examples either didn't work or were improperly documented. 

**Much of the code in this notebook is borrowed from other walkthroughs. There are a few key changes that took us a while to figure out, and so we were inspired to share.**

# What you'll need...

1. About **10K inputs and outputs** you'd like to train the model on. We generated these using some python scripts and openai's gpt3.5. For us, the average total token count of each input/output pair was ~300, and **no pair was longer than 800 tokens**.
2. A **runpod account**, and about **~$25**. That's what it cost us, once we had everything figured out. 
3. **ChatGPT** open in another tab. This notebook works for us as of **September 2023** but there's no gaurantee it'll work for you. With any luck, you (and ChatGPT) should be able to overcome any obstacles that arise. 
4. About **2 hours** of setup and the patience to wait **5-8 hours** for results.

**Take a look at ```llama2-finetune.ipynb``` to  get started!**
