Colorectal polyps are benign lesions that develop in the colon and can progress to cancer if left untreated. Clinical observations from medical images are often preferred over computational results due to the lack of trust in the machine learning models, thereby posing serious challenge for the explainability of the results. In order to computationally diagnose colorectal polyps from cancerous images and explain the results, we propose a Layer-wise eXplainable ResUNet++ (LeXNet++) framework for segmentation of the cancerous images, followed by layer-wise explanation of the results. We utilize a publicly accessible dataset that contains of 612 raw images with a resolution of 256x256x3 and an additional 612 clinically annotated and labeled images with are solution of 256x256x1, which includes the infected region.The LeXNet++ framework comprises of three components—encoder, decoder and the bridge. The encoder and the decoder components each comprise of four layers. Each of the four layers in the encoder and the decoder comprises of14and11internal sub-layers, respectively. Among the sub-layers of the encoder andthe decoder, there are three 3x3 convolutional layers with an additional 3x3 convolution transpose layer in the decoder. The output of each of the sub-layers has been explained through heatmap generation after each iteration which have been further explained.The encoder and the decoder are connected by the bridge which comprises of three sub-layers. The results obtained from these three sub-layers have also been explained to inculcate trust in the findings. In this study, we have used three models to segment the images, namely UNet, ResUNet, and proposed LeXNet++. LeXNet++ exhibited the best result among the three models in terms of performance; hence, only LeXNet++ was explained layer-wise. Apart from explanation of the results fetched in this study, the performance of the proposed explainable model has been observed to be 2% greater than the existing polyp segmentation proposals, both with and without explanations. 
![Fig](https://github.com/user-attachments/assets/775eda73-b4fc-46de-b5e8-af241f27f10b)
The proposed LeXNet++ framework.

![fig3](https://github.com/user-attachments/assets/d3664fd9-d377-4fad-b9e0-856d314cfceb)
The proposed LexNet++ architecture with layer-wise Heatmap Generation.

![fig4](https://github.com/user-attachments/assets/52ef0444-ac07-4b8f-9d02-475478e6d648)
Layerwise heatmap generation of the proposed LeXNet++ framework
