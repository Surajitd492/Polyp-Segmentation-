Colorectalpolypsarebenignlesionsthatdevelopinthecolonandcanprogress tocancerifleftuntreated.Clinicalobservations
 from medical images are often preferred over computational results due to the lack of trust in the machine learning models,
 thereby posing serious challenge for the explainability of the results. In order to computationally diagnose colorectal polyps
 from cancerous images and explain the results, we propose a Layer-wise eXplainable ResUNet?? (LeXNet??) framework
 for segmentation of the cancerous images, followed by layer-wise explanation of the results. We utilize a publicly accessible
 dataset that contains of 612 raw images with a resolution of 256 256 3 and an additional 612 clinically annotated and
 labeledimageswitharesolutionof256 256 1, whichincludestheinfectedregion.TheLeXNet??frameworkcomprises
 of three components—encoder, decoder and the bridge. The encoder and the decoder components each comprise of four
 layers. Each of the four layers in the encoder and the decoder comprises of14and11internal sub-layers, respectively. Among
 the sub-layers of the encoder andthe decoder, there are three 3 3convolutionallayerswithanadditional3 3convolution
transpose layer in the decoder. The output of each of the sub-layers has been explained through heatmap generation after each
 iteration whichhavebeenfurtherexplained.Theencoderandthedecoderareconnectedbythebridgewhichcomprisesofthree
 sub-layers. The results obtained from these three sub-layers have also been explained to inculcate trust in the findings. In this
 study, we have used three models to segment the images, namely UNet, ResUNet, and proposed LeXNet??. LeXNet??
 exhibited the best result among the three models in terms of performance; hence, only LeXNet?? was explained layer-wise.
 Apart from explanation of the results fetched in this study, the performance of the proposed explainable model has been
 observed to be 2% greater than the existing polyp segmentation proposals, both with and without explanations. 
