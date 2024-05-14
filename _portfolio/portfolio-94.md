---
title: "Faces generation for Memory Research"
excerpt: "Use GANs to generate artificial faces that can be used for memory research"
collection: portfolio
---

![Descriptor](/images/fakeface.jpeg){:height="450px" width="300px"}

## Description

We are working on a super interesting project.  Innocent Project (https://innocenceproject.org/) is an international organization that deals worldwide with wrongfully convicted cases.  In several of those cases there is always a line up witness trial procedure that it is either purposely manipulated or it is based on a very wrong procedure in terms of how human memory works.  The "Lab Sueño y Memoria" at ITBA University, Buenos Aires, Argentina (https://www.labsuenoymemoria.com/) works closely with Innocent Project to provide research evidence that is used by this organization to present legal cases.

What are we doing:  The Lab needs to create realistic faces and needs to be able to manipulate them.  Hence, we are working on a modified version of StyleGAN2 from NVIDIA to do three things: (1) we created an app that connects to StyleGAN2 and that can be used by researchers and the legal team to create and manipulate realistic faces. (2) we are modifying certain aspects of StyleGAN to be able to have more concept vector directions on the latent space to be able to manipulate the faces in several ways (for instance, keeping the face frame, the hairline, intact between images). (3) StyleGAN has been trained with FFHQ which is very biased towards European and American faces, and we need to retrain it to be able to generate faces more similar to South Americans.  

This is a Bachellor's Dissertation that explains in details the first iteration of this project: https://catalogo.itba.edu.ar/cgi-bin/koha/opac-detail.pl?biblionumber=17919
This is a video on how to use the currently version of the app:https://www.youtube.com/watch?v=KcqwrXCWKF0

Currently this project involves the manipulation of real faces to force them to have a very specific emotional expression, like given someone's picture, get the same picture but with a person showing affection, an angry face, sadness and so on.  It is the opposite of what a lot of computer vision do, that recognize the affection given a picture.

## Bachellor's Thesis

* Title: Use of Generative Adversarial Networks for the creation and manipulation of facial images in the context of studying false memories and its effects on wrongful conviction cases.
  * Link: https://ri.itba.edu.ar/entities/proyecto%20final%20de%20grado/5cbc8418-8b08-4f4f-a9d2-8d0ee94112ae
  * Students: Jimena Lozano, Maite Herrán
  * Director: Rodrigo Ramele

* Title: Controlling Face's Frame generation in StyleGAN's latent space operations, Modifying faces to deceive our memory
  * Link: https://ri.itba.edu.ar/entities/proyecto%20final%20de%20grado/0ceaaf22-f870-402f-a905-994cd5e2a612
  * Student: Agustín roca, Nicolás Britos
  * Director: Rodrigo Ramele

* Título: Face Generator: A Web-based Platform for Interactive Facial Image Generation and Manipulation, Unveiling StyleGAN in a Web-based Interface for Face Generation.
  * Students: Octavio Serpe, Agustín Jerusalinksy, Francisco Quesada
  * Director: Rodrigo Ramele

## Talks

* University of Essex, Computer Vision Seminars, organized by Dr. Alba Garcia Seco:  https://albagarciaseco.blogspot.com/p/seminars.html
* *Bachellor's Thesis*: https://ri.itba.edu.ar/handle/123456789/3800
* https://www.youtube.com/watch?v=KcqwrXCWKF0

* ITBA Students: 
 * Maite Herran, Jimena Lozano
 * Agustín Roca, Nicolás Britos
 * Octavio Serpe, Agustín Jerusalinksy, Francisco Quesada








