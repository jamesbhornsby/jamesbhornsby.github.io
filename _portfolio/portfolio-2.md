---
title: "Media Digitizer"
excerpt: "Combining Convolution Neural Networks and OCRs. <br/><img src='/images/mediaDigProcess.png' width='650'>"
collection: portfolio
---
The ideation of this project began with me seeking rare, out of print essay collections on the Internet Archive. I discovered that the workflow used to convert photographed pages into friendlier formats was less than satisfy in consistency. 

I devised a plan to gather enough data such that the solution would not only copy the information, but understand the relationship between the page's elements. If this was done, then it was possible to reliably reconstruct the a given page into flowed text formats with some simple scripting.

When asked at the beginning of the fall '25 semester whether I would be willing to lead a CodeCoogs team project through the development process, I shared my idea to combine deep with OCRs, and, after interviews, I was among those selected to lead.

<br/><img src='/images/mediaDigitizer.png' width='650'>

By this time, my team had the done the majority of the work on the project's biggest hurdle: building a synthetic dataset generator from scratch. This process required writting scripts to generate pages while randomizing all aspects and performing various linear transformations. This was done to ensure that the model would have a diverse and representative collection of data to learn from.

<br/><img src='/images/mediaDigDataset.png' width='650'>

From there, it was a matter of training the convolutional neural network (CNN). With a database of over one thousand images, I performed incremental training and validation, monitering the improvements at each milestone. After a some fine tuning, I had the result that I was looking for: a page could be imaged and reliably transformed into flowed text.

<br/><img src='/images/mediaDigProcess.png' width='650'>

Though we did not get beyound a simply web app for interaction, we built our solution on a CNN known for its low compute overhead and real-time performance. Due to this, our application could be integrated into, say, a mobile app using the camera to rapidly copy printed material.