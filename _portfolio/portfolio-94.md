---
title: "Faces generation for Memory Research"
excerpt: "Use GANs to generate artificial faces that can be used for memory research"
collection: portfolio
---

![Descriptor](/images/fakeface.jpeg){:height="450px" width="300px"}

## Description

We are working on a super interesting project.  Innocent Project (https://innocenceproject.org/) is an international organization that deals worldwide with wrongfully convicted cases.  In several of those cases there is always a line up witness trial procedure that it is either purposely manipulated or it is based on a very wrong procedure in terms of how human memory works.  The "Lab Sueño y Memoria" at ITBA University, Buenos Aires, Argentina (https://www.labsuenoymemoria.com/) works closely with Innocent Project to provide research evidence that is used by this organization to present legal cases.

What are we doing:  The Lab needs to create realistic faces and needs to be able to manipulate them.  Hence, we are working on a modified version of StyleGAN2 from NVIDIA to do three things: (1) we created an app that connects to StyleGAN2 and that can be used by researchers and the legal team to create and manipulate realistic faces. (2) we are modifying certain aspects of StyleGAN to be able to have more concept vector directions on the latent space to be able to manipulate the faces in several ways (for instance, keeping the face frame, the hairline, intact between images). (3) StyleGAN has been trained with FFHQ which is very biased towards European and American faces, and we need to retrain it to be able to generate faces more similar to South Americans.  

We need the GPU for this project.

This is a Bachellor's Dissertation that explains in details the first iteration of this project: https://catalogo.itba.edu.ar/cgi-bin/koha/opac-detail.pl?biblionumber=17919
This is a video on how to use the currently version of the app:https://www.youtube.com/watch?v=KcqwrXCWKF0

## Scope

Implement the program that can generate the faces offline.

* *Bachellor's Thesis*: https://ri.itba.edu.ar/handle/123456789/3800

https://www.youtube.com/watch?v=KcqwrXCWKF0

* ITBA Students: 
 * Maite Herran mherran@itba.edu.ar
 * Jimena Lozano jilozano@itba.edu.ar
 * Nicolás Britos
 * Agustín Roca








