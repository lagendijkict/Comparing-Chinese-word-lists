# Find new words in vocab list

## Introduction
When learning Mandarin Chinese, I often encounter words I want to save for later. My favourite tool to list them is [Quizlet](https://quizlet.com/latest), it's easy to use on both computer and mobile.

One of the websites I use to find vocab & practice material is [Mandarin Corner](mandarincorner.org).
They have varied learning materials in native Chinese for a fair price. Here I found a long list, which made me wonder how many of these words already existed in my Quizlet.
I could read through all, but that's a bit boring, because many I already know.

## Project Goals
* Read content of (old) source Excel file
* Read content of (new) source csv file
* Compare content
* Translate new content

## Module Requirements
* [pandas](https://pypi.org/project/pandas/) (any version will do)
* [googletrans](https://pypi.org/project/googletrans/) version 4.0.0-rc1 (or newer)

Both of these can be installed with pip.

## Step by step

0. To avoid double entries across my lists, I have an Excel document that keeps track of all records (Chinese only). If you don't have this yet, but still want to follow along, you should export your Quizlet lists. More info here: [Exporting Quizlet sets](https://help.quizlet.com/hc/en-us/articles/360034345672-Exporting-your-sets) Place the result in an Excel column with Term as column name.
1. Copy data from the vocab website of your choice. Paste this in new_data.csv Keep copyright into account, only scrape when allowed.

For the remaining steps, run each cell in the Jupyter Notebook.

## Other remarks
If you have one or more unrecognized words, or if you want to change the destination language, consult [Googletrans docs](https://py-googletrans.readthedocs.io/en/latest/) for these.
 
If you want the code to work with other languages besides Chinese, the main thing to change would be the save_new_vocab_into_list function in Step 3.
