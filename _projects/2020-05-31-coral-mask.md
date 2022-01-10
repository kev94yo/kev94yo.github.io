---
layout: project
title: Real-time Mask Detection on Google Edge TPU
caption: Lightweight mask detection model on Google Coral Dev Board.
description: >
  This lightweight model has been built based on MobileNetV2, with full integer quantization applied.
date: '2020-05-31'
image: 
  path: /assets/img/projects/coral-mask-model.jpg
  # srcset: 
  #   1920w: /assets/img/projects/hydejack-site.jpg
  #   960w:  /assets/img/projects/hydejack-site@0,5x.jpg
  #   480w:  /assets/img/projects/hydejack-site@0,25x.jpg
links:
  - title: Link
    url: https://arxiv.org/abs/2010.04427
sitemap: true
---

In my first semester at SNU GSDS, there was a group project in a machine learning lecture. We were free to choose from
any topic of interest, and chose a topic related with the COVID pandemic, since it was only a few months after the outbreak.
To apply the machine learning knowledge in class, our group decided to develop a lightweight mask detection model, specifically to be
deployed on to an edge TPU device, to differ from other mask detection projects. 

## Motivation
1. To contribute to 'social distancing and public mask wearing' as data scientists.
2. Utilize transfer learning and Edge TPU to align with the 'Ambient AI' project by the school.
  - Ambient AI: AI everywhere, accelerated by AI chips embedded in numberous small edge devices

<p align="center">
  <img src="../../assets/img/projects/coral-mask-ambient-ai.jpg" alt="Ambient AI" width="400">
</p>
SNU Ambient AI project outline.
{:.figure}

## Project Outline
- Literature Review: Reviewed multiple papers on classification, object detection and quantization.
- Data Collection: Collected data with masked faces.
- Model Development: Combined MobileNetV2 our classification model to detect faces and classify masks.
- Train, Evaluate: Trained the model for high accuracy.
- Quantization: Performed full integer quantization on the model.
- Deployment: Deploy the quantized model on to Coral Dev Board.

<p align="center">
  <img src="../../assets/img/projects/coral-mask-pipeline.jpg" alt="pipeline" width="500">
</p>
Coral deployment pipeline.
{:.figure}

## Result
- Successfully trained our model to detect masks with great accuracy.
- Well quantized the model and held successful demonstrations on Coral Dev Board.
- Grabbed media attention from Maeil Newspaper. ([**Coral Mask Detection on the media!**](../../blog/media/2020-06-30-coral-mask))

## Personal Contributions | Skill Development
1. **Literature Review**: I reviewed the FaceNet paper.
2. **Data Collection, Augmentation**: I collected data from peers and augmented original face data to wear masks by using xml editing tools.
3. **Research Pipeline Development**: I wrote pipeline code to insert data into the mask detection model for training and evaluation.
4. **Presentation**: I presented this project using powerpoint slides. Here's the video on [youtube](https://www.youtube.com/watch?v=MdS2j5mPYmk&ab_channel=WooLEE) of the presentation.

## Obstacles
Here are a few important obstacles I faced during this project.
- **Low resources on quantization**
  - Since quantization was not an old topic, online resources on quantization and quantized TF Lite models were scarce.
  Therefore, troubleshooting errors was a big challenge.
  - **Solution**: Reached out to one of the professors ([Hyungshin Kim](https://sites.google.com/site/hskiminthebody){:.heading.flip-title}) who was an expert in IoT and Edge TPUs for help.
  Also met with people from the Google Coral Dev Board team to ask questions. And of course, extensively utilized stackoverflow :)
- **Low amount of data**
  - There were lots of freely available pictures on the internet, but most of them were without masks.
  - **Solution**: Performed data augmentation on face images to create faces with masks. Also collected masked face data through crowdsourcing.

## Languages & Tools
Here are the languages and tools used for this project.
- Python, Tensorflow
- Jupyter Notebook
- Microsoft Powerpoint
- Git

## Links
*  **Github**: <a href="https://github.com/kev94yo/coral_mask" target="_blank">https://github.com/kev94yo/coral_mask</a>
*  **Media**: <a href="https://n.news.naver.com/article/009/0004605829" target="_blank">https://n.news.naver.com/article/009/0004605829</a>
*  **Talk**: <a href="https://www.youtube.com/watch?v=MdS2j5mPYmk&ab_channel=WooLEE" target="_blank">https://www.youtube.com/watch?v=MdS2j5mPYmk&ab_channel=WooLEE</a>
*  **Paper**: <a href="https://arxiv.org/abs/2010.04427" target="_blank">https://arxiv.org/abs/2010.04427</a>