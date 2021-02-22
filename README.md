# Amazon Vine Analysis
## Overview

Here is an analysis of an Amazon dataset of Vine and non-Vine client's reviews on musical instruments, to understand if there is any bias (positive or negative) towards the Vine reviewers.

A data set of reviews about musical intruments was analyzed, and the 5-star reviews were compared between regular clients' reviews and Vine program participants' reviews.

## Code

ETL (Extract,Transform and Load) was performed in an Amazon Dataset using PySpark on Google COLAB.

After runing a series of trasnformations (filters, joins), results were obtained to better understand the bias on reviews by Vine participants.

<img width="1385" alt="Screen Shot 2021-02-21 at 10 21 19 PM" src="https://user-images.githubusercontent.com/72593264/108662081-21bd4a00-7493-11eb-8b5c-0145afce954b.png">
<img width="1330" alt="Screen Shot 2021-02-21 at 10 22 02 PM" src="https://user-images.githubusercontent.com/72593264/108662127-3b5e9180-7493-11eb-861b-6f18c0f0d42d.png">
<img width="1371" alt="Screen Shot 2021-02-21 at 10 22 35 PM" src="https://user-images.githubusercontent.com/72593264/108662156-4f09f800-7493-11eb-9546-416e1a2cb2d9.png">
<img width="1208" alt="Screen Shot 2021-02-21 at 10 23 13 PM" src="https://user-images.githubusercontent.com/72593264/108662182-6517b880-7493-11eb-8fb7-408cd5aae1af.png">
<img width="1325" alt="Screen Shot 2021-02-21 at 10 23 45 PM" src="https://user-images.githubusercontent.com/72593264/108662214-782a8880-7493-11eb-9b20-4503e2c2a902.png">
<img width="1248" alt="Screen Shot 2021-02-21 at 10 24 10 PM" src="https://user-images.githubusercontent.com/72593264/108662238-87113b00-7493-11eb-9dfc-25c74e086014.png">
<img width="1371" alt="Screen Shot 2021-02-21 at 10 24 44 PM" src="https://user-images.githubusercontent.com/72593264/108662270-9b553800-7493-11eb-9555-fc52f318725e.png">
<img width="1288" alt="Screen Shot 2021-02-21 at 10 25 14 PM" src="https://user-images.githubusercontent.com/72593264/108662316-ad36db00-7493-11eb-9318-0fa0b10347a1.png">


## Results

The reviews were split into two categories:
- Vine participants and,
- non-Vine participants. 

Here are the results for each category:

### Vine Participants
- In this data set, the number of Vine participants was of: **60**

    <img width="278" alt="Screen Shot 2021-02-21 at 10 13 04 PM" src="https://user-images.githubusercontent.com/72593264/108661668-fd14a280-7491-11eb-9a84-e371707a8332.png">

- The number of 5-star reviews, among Vine participants was of: **34**

    <img width="340" alt="Screen Shot 2021-02-21 at 10 13 40 PM" src="https://user-images.githubusercontent.com/72593264/108661689-10277280-7492-11eb-88d7-5465d13f8b27.png">

- Conversely, the percentage of Vine participants 5-Star reviews was of: **56.7%**

    <img width="736" alt="Screen Shot 2021-02-21 at 10 16 03 PM" src="https://user-images.githubusercontent.com/72593264/108661806-64caed80-7492-11eb-909b-4d18d945aaba.png">

### Non-Vine Participants
- In this data set, as expected, the number of non-Vine participants was much higher: **14477**

    <img width="319" alt="Screen Shot 2021-02-21 at 10 17 36 PM" src="https://user-images.githubusercontent.com/72593264/108661891-9c399a00-7492-11eb-8285-c16f640ca808.png">

- The number of 5-star reviews, among Vine participants was of: **8212**

    <img width="400" alt="Screen Shot 2021-02-21 at 10 25 52 PM" src="https://user-images.githubusercontent.com/72593264/108662360-c3dd3200-7493-11eb-8919-0c8eb7e10a4d.png">

- Conversely, the percentage of Vine participants 5-Star reviews was of: **56.7%**

    <img width="840" alt="Screen Shot 2021-02-21 at 10 26 26 PM" src="https://user-images.githubusercontent.com/72593264/108662396-d8212f00-7493-11eb-8114-c9820562679e.png">

## Summary

Interestingly enough, the rounded percentage of both categories (Vine and non-Vine participants) was exactely the same: **56.7%**
That means that, at least reagarding musical intruments reviews, according to this dataset, **no bias can be found among reviews by Vine Program participants.**

As a recommendation to support this result, other datasets on Vine reviews should be analysed, and their result should be crossed to this one to understand if this result is really reflective of the reality.
