---
title: "Deep Fake Detection based on Physical or Physiological Models"
excerpt: "Use modelling to determine if a video is a fake or not"
collection: portfolio
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/iyiOVUbsPcM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Description


Deep fakes are everywhere and the next few years are going to be a big issue all around the world.  This is an arms race that requires to produce tools that are able to deal with the problem, to move the post ahead.  One way in which this can be done, is by using physiological valid or physically valid models derived from the videos, to see if the information that is obtained from the video is indeed valid or not.

For instance, it is possible to infer a signal similar to PPG from the analysis of the red spectrum of face pixels from a human being.  They shuld represent the blood filling the vascular regions of the face, and the red light emitted from those pixels fluctuates following a similar pattern derived from the flow circulation (https://www.sciencedirect.com/science/article/abs/pii/S1746809417301362).  A similar situation can also be applied with deep fakes from people, where for instance, the respiration must be met, if the person is running or moving, there must be some change in the way the person breath and this can eventually be detected.

Another application is for physical videos. Physics require certain restrictions to be met in terms of possible masses, how they move, energy constraints and so on.  A video can be analyzed trying to understand if these constrainst are fulfilled and if not, flag the video as likely false.  This is exactly what we do when we see a video and we apply our understanding of how things work in the world to see if what is happening in the video is plausible or not.

<iframe width="560" height="315" src="https://x.com/Rainmaker1973/status/1703720519995134023" title="Twitter" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Methodology

EdgeAI, or ASIC technology specifically designed for video or image processing https://blog.inten.to/hardware-for-deep-learning-part-4-asic-96a542fe6a81 can be used to implement the video processing.

## Scope

It is possible and quite straightforward to start detection the physiological response and start to iterate from there.
