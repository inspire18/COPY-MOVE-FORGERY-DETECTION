# COPY-MOVE-FORGERY-DETECTION
𝙄𝙣𝙩𝙧𝙤𝙙𝙪𝙘𝙩𝙞𝙤𝙣
With the increasing importance of image information, image forgery seriously threatens the
security of image content. Copy-move forgery detection (CMFD) is a greater challenge
because its abnormality is smaller than other forgeries.

𝑷𝒓𝒐𝒃𝒍𝒆𝒎 𝑺𝒕𝒂𝒕𝒆𝒎𝒆𝒏𝒕
As image editing softwares like Adobe Photoshop and ACDSee Photo Editor are becoming
more prevalent, there is an ever increasing need for developing a solution for accessing the
authenticity of the image in question. This solution is very important in places like judiciary
and politics where determining the authenticity of image data is of utmost importance.
Therefore, the image forensics technique, aiming at detecting and locating the forgery, has
important research value. Copy-move forgery detection (CMFD) is one of the passive
forensics techniques for copy-move forgery. It is a common and easy image forgery
manner, which copies and pastes a region from an image to the same image.

𝑷𝒓𝒐𝒑𝒐𝒔𝒆𝒅 𝑺𝒐𝒍𝒖𝒕𝒊𝒐𝒏

We propose a binary classification method based on Local Binary Patterns and Discrete
Cosine Transform. We have used a support vector machine for classification. The
MICC-F220 dataset is used for training and testing the model.
In order to extract deep features with minimal training effort, the proposed copy move
detection employed a pre-trained AlexNet model. The Logistics classification method was
used. As training such a CNN model is time consuming and resource internstive, we have
employed a pre-trained AlexNet model for the purpose of feature extraction.
The entire workflow can be divided into 4 distinct phases which are as follows:
1. Pre - Parsing and Image Processing
○ According to the AlexNet model's first input layer, the images were then
resized to 227 227 pixels. After that, the images were transformed to
grayscale images.
2. Feature Extraction
○ The feature extraction is performed with the assistance of a pre-trained
AlexNet model. It can be seen that the network's original weights are
preserved, while the original layers are employed in the feature extraction
step. Finally, a total of 4096 dimensional feature vectors were extracted from
the fully connected fc7 layers. The feature selection procedure is applied to
the feature vector, which is subsequently input into a classifier.
3. Feature Selection
○ Feature selection approaches focus on eliminating duplicated and irrelevant
features. Furthermore, by avoiding overfitting, Feature selection is utilized to
minimize training time and enhance generalization capacities. An algorithm
known as ReliefF is used for feature selection. In order to achieve an optimal
and relevant set of features, a total of 4096 dimensional feature vectors were
subjected to the ReliefF algorithm.
4. Classification
○ In order to implement the detection task, The distinguishing features are
supplied to the classifiers. The classifier's job is to determine whether or not
the image is genuine. Ordinary regression is the foundation for logistic
regression, often known as statistical regression.

