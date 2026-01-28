#  Pablo Strunz - Data Science Portfolio

Machine Learner in the making.

---

##  Skills & Technologies

- **Languages**: Python
- **Libraries**: Pytorch, Pandas, NumPy, Scikit-learn, Tensorflow, Matplotlib, Seaborn
- **Tools**: Jupyter Notebook, Git
- **Concepts**: Deep Learning, Regression, Classification, Time Series Forecasting

---

## 🤖 Machine Learning Projects:

### 1. Neural Style Transfer

Neural Style Transfer (NST) refers to a class of software algorithms that manipulate digital images, or videos, in order to adopt the appearance or visual style of another image.
NST takes two images as input (content image & style image) and creates a new image representing the content from the content image blended with the artistic style from the style image.

**Goal**: Build, train and deploy a Neural Network that stylizes Images on the fly.  
**Tech Stack**: Pytorch, Gradio, Generative AI
- First I learned about basic vs fast NST:
Both methods rely on a pre-trained VGG network extracting features from input images as well as a loss function adding the differnece in content representation between the content image and the new image (content loss) to the differnece in style representation between style image and the new image (style loss).
Basic NST updates the generated image itself during training.
Fast NST on the other hand trains a neural network to apply a certain style to any input image in a single pass through the network. (ergo: that's what I need)
- Next I built a feedforward Network and trained it on 4 different style images.
For training data I used images from the COCO 2014 dataset.
I trained each model for a couple hours on between 2000 to 3500 samples of the COCO dataset.
In terms of experimentation I set the style weight (style loss needs to be weighted heavily) as a hyperparameter that I could tweek to influence the model's results.
One could probably generate more accurate results by training for longer and on more data.
- Finally I deployed the project:
I used gradio to create a simple web interface for my model
and deployed it on huggingface spaces.

[🔗 Huggingface Space](https://huggingface.co/spaces/cian-ps/image_stylization)  
[🔗 Source Code](https://github.com/cian-ps/neural_style_transfer)

---

### 2. Dog Breed Detection
**Goal**: Determine a dog's breed from a photo  
**Tech Stack**: Computer Vision, Tensorflow, Transfer Learning
- Trained a multi class image classifier model on ~10000 labeled images.
- The model achieved a Multi Class Log Loss of 0.87 on the test data.
 
[🔗 View Project](https://github.com/cian-ps/dog-breed-detection)

---

### 3. Bulldozer Sale Price Predictiion
**Goal**: Predict the sale price of a bulldozer based on previous sales data.  
**Tech Stack**: Scikit-Learn, Catboost, Random Forest, Time Series Data 
- Compared Random Forest Regressor vs Catboost Regressor.
- Improved the model's hyperparameters using RandomizedSearchCV & GridSearchCV
- Achieved a root mean squared log error of 0.36

[🔗 View Project](https://github.com/cian-ps/ml_lab_bluebook-bulldozers)

---

## 🏅 Certifications

[🔗 Python (Basic) Certificate](https://www.hackerrank.com/certificates/60e73997f090)

