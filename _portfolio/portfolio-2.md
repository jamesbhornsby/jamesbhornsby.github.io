---
title: "Media Digitizer"
excerpt: "Combining Convolution Neural Networks and OCRs. <br/><img src='/images/mediaDigProcess.png' width='650'>"
collection: portfolio
---
The ideation of this project began while I was accessing rare, out of print essay collections on the Internet Archive. I discovered that the workflow used to convert photographed pages into easier to use formats was ineffective in rendering consistent results. 

Thus, I thought that if enough data could be gathered such that the solution not only copied the information, but understood the relationship between the page's elements, then it was possible to reliabley recronstruct the given page into a flowed text format.

When asked at the beginning of the Fall '25 semester whether I would be willing to lead a CodeCoogs team project through the development process, I shared my idea to combine deep learning neural with OCRs, and, after interviews, I was among those selected to lead.

<br/><img src='/images/mediaDigitizer.png' width='650'>

By this time, my team had the majority of the groundwork on the projects biggest hurdle: building a synthetic dataset generator from scratch. This process required writting scripts to generate pages while randomizing all aspects and performing various linear transformations.

<br/><img src='/images/mediaDigDataset.png' width='650'>

From there, it was a matter of training the convolutional neural network. With a database of over one thousand images, I performed incremental training and validation, monitering the improvement at each milestone. At last, the result we want: a page could be imaged and reliably transformed into flowed text.

<br/><img src='/images/mediaDigProcess.png' width='650'>