---
layout: project
title: Music-Circles
caption: An interactive visualization of billboard song clusters
description: >
  Music-Circles links audio feature data offered by Spotify to popular songs to create unique vectors for each song,
  and calculate similarities between these vectors to cluster them.
date: '2020-12-11'
image: 
  path: /assets/img/projects/music-circles-analysis.jpg
  # srcset: 
  #   1920w: /assets/img/projects/qwtel.jpg
  #   960w:  /assets/img/projects/qwtel@0,5x.jpg
  #   480w:  /assets/img/projects/qwtel@0,25x.jpg
links:
  - title: Link
    url: https://musiccircles.netlify.app/result/bubbleradar
# accent_color: '#4fb1ba'
# accent_image:
#   background: '#193747'
# theme_color: '#193747'
sitemap: true
---

In my second semester at SNU GSDS, there was a group project in a data visualization lecture. We were free to choose from
any topic of interest and form a team. Hence, since I was interested in music, I reached out to different students who may be interested in music as well, and formed a team.
After our team was formed, we decided to use music from the billboard and audio features data from Spotify to create an interactive visualization system.

## Motivation
1. Find novel ways of clustering music.
  - Depart from traditional artist/genre, and use audio features
2. Create an interactive visualization system, Music-Circles, to target music enthusiasts.
  - Offer exploration of patterns in hit songs

<p align="center">
  <img src="../../assets/img/projects/music-circles-circular.jpg" alt="circular" width="800">
</p>
Front page of Music-Circles with a circular bar chart.
{:.figure}

## Project Outline
- Data Collection: Collected data from Spotify and Billboard.
- Data Combination: Match audio features from Spotify to Billboard songs to serve our interest.
- Data Transformation: Choose 6 audio features, and megahit songs only for visualizations.
- System Development: Write code using web development skills to create an interactive visualization.
  1. Circular Bar Chart: Offer information about different audio features
  2. Survey: Survey page that allows users to find their personal music cluster
  3. Lined bubble, radar, and table chart: Information on the music cluster output from the survey
- Deployment: Deploy the system online.

<p align="center">
  <img src="../../assets/img/projects/music-circles-survey.jpg" alt="survey" width="600">
</p>
Survey page of Music-Circles. Colors change interactively with the user's choice.
{:.figure}

## Result
- Successfully coded and deployed the interactive visualization system.
- Grabbed media attention from TechExplore. ([**Music-Circles on TechExplore!**](../../blog/media/2021-03-16-music-circles))

## Personal Contributions | Skill Development
1. **System Development**: I wrote extensive HTML, CSS and Javascript code for the interactive visualization to happen.
4. **Presentation**: I held a talk about this project using powerpoint slides.

## Obstacles
Here are a few important obstacles I faced during this project.
- **No prior experience with Web Development**
  - I only had experience with machine learning projects using Python and C.
  - **Solution**: Took and fully completed online courses on [CodeIt](https://www.codeit.kr/event){:.heading.flip-title} and Coursera that covered HTML, CSS, JavaScript and D3.
  Extensively utilized stackoverflow as well :)
- **No experience on a project focused on Data Visualization**
  - Data Visualization in its true form had many non-programming aspects to it, like psychological elements on attention and visual aesthetics.
  - **Solution**: Reached out to the professor ([Hwajung Hong](http://communication.metapresso.net/snu__professor/%ED%99%8D%ED%99%94%EC%A0%95/){:.heading.flip-title}) who was an expert in journalism for great advice.

## Languages & Tools
Here are the languages and tools used for this project.
- HTML, CSS, JavaScript, D3, Python
- Jupyter Notebook
- Microsoft Powerpoint
- Git

## Links
*  **Github**: <a href="https://github.com/kev94yo/snuDxd" target="_blank">https://github.com/kev94yo/snuDxd</a>
*  **Media**: <a href="https://techxplore.com/news/2021-03-music-circles-interactive-visualization-tool.html" target="_blank">https://techxplore.com/news/2021-03-music-circles-interactive-visualization-tool.html</a>
*  **Website**: <a href="https://musiccircles.netlify.app/" target="_blank">https://musiccircles.netlify.app/</a>
*  **Paper**: <a href="https://arxiv.org/abs/2102.13350" target="_blank">https://arxiv.org/abs/2102.13350</a>