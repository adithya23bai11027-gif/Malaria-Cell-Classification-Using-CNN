PROJECT REPORT

Project Title: Malaria Cell Classifier CNN

Author: adithya23bai11027  
Date: 2026-03-04 


1. Introduction

Malaria is one of the major global health burdens which causes a million deaths annually, early detection is survival in this case. Currently, a specialist needs to utilize a microscope to conduct a thorough examination for diagnosis purposes. Let's admit it, this task can be time-consuming, and no one has perfect vision constantly. This is not just about people and labs getting exhausted, but also about mistakes slipping through unnoticed.
I am taking on this project to experiment with training a Convolutional Neural Network (CNN) solely on blood cell images to see if it can independently detect malaria. For me, it is also a question of finding an assistive tool to give health workers a second opinion at this time of need.

2. Objectives

Develop a robust CNN model that can detect malaria-infected cells with high precision.
Learn from my experiences of actually implementing all of this using TensorFlow and Keras, since this is what I learned about.

3. Dataset

This is a famous publicly available dataset frequently used in research. There are thousands of blood images, every one annotated positive or not. The need to go and gather my own data itself was quite time and effort-consuming for me.

4. Methodology

Data Preprocessing

Before I could even think about feeding the images to the model, I had to clean them up a bit. The first thing I did was make sure every image was the same size. I then standardized the pixel values to prevent extremely high numbers. I incorporated data augmentation techniques, which involve randomly adjusting images by rotating, flipping, and zooming (making slight scale modifications). Such tricks (variations of the input data augmentation, i.e., very similar, near the original image) help it generalize better because it is trained on subtly modified versions of the picture seen during training.

Model Architecture

I designed a fairly simple CNN without any overly complex components. The model consists of several convolutional layers for pattern detection, multiple max-pooling layers to decrease dimensions, and ultimately a few fully connected layers for making classification choices.I kept the architecture simple on purpose so I could test how well a basic model would do before layering on more advanced features.

Training

For training, I picked Adam because it usually performs well without much fiddling. I used categorical cross-entropy as my loss function—it's a good fit for this kind of problem. Then I let things run while watching the validation loss like a hawk. My main concern was avoiding overfitting. I wanted the model to learn, not just memorize.

5. Results

To be honest, I was really happy with how it turned out. The model hit over 95% accuracy on the validation set. That means for every 100 new images I threw at it, it got at least 95 of them right. For a project like this, I think that's a pretty solid result. It showed me that the model actually learned something useful—it wasn't just guessing or taking lucky shots.

6. Conclusion

Looking back, this project reinforced my belief that CNNs have real potential in medical image analysis. You don't necessarily require a highly intricate arrangement - a well-built model combined with good quality data can achieve significant results. It feels rewarding to know that something I built could one day contribute to solving real-world problems like malaria detection.

7. Future Work

I'm eager to experiment with transfer learning next.I've come across quite a few discussions where people mentioned that using pre-trained models—like VGG or ResNet—often leads to better accuracy and takes way less training time.One thing I'd love to explore is whether this approach could be applied beyond malaria. Imagine using it to identify different types of blood disorders or even other parasitic infections. That would be pretty exciting.

8. References

Before I started building, I looked through quite a few research papers to see how other people had designed their CNNs. That gave me some solid ideas. And during the actual coding, I probably had a dozen tutorial tabs open at all times. Every time something broke or I didn't understand an error message, those online guides came to the rescue.

9. Acknowledgments

I genuinely want to thank everyone who makes their datasets and code available to the public. This project wouldn't have existed without people willing to share their work so openly. And a huge shoutout to the online developer community—you all answered so many of my random questions along the way, and I really appreciate the patience.

I also used data augmentation—things like rotating, flipping, or zooming images just a bit. This forces the model to learn from slightly different versions of the same picture, which helps it generalize better and perform well on new data.

