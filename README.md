# 🍽 Food Classification Model Predict
<img src="https://t1.rg.ltmcdn.com/es/posts/7/4/1/ceviche_peruano_18147_orig.jpg" />

# Overview
This model is trained to recognize 2023 food dishes from images. It is based on MobileNet V1.

# Input
This model takes images as input.

Inputs are expected to be 3-channel RGB color images of size 224 x 224, scaled to [0, 1].

# Output
This model outputs to image_classifier.

image_classifier: A probability vector of dimension 2024, corresponding to a background class and one of 2023 food dishes in the labelmap.

# Model architecture
For details of the model architecture, see MobileNet V1.

# Suitable usecases
This model is trained to recognize 2023 food dishes. The training set includes entrees, side dishes, desserts, snacks, etc.

# Unsuitable usecases
Do not use this model to determine whether an object is edible or not. This model is not suitable for predicting the ingredients of a food dish. Do not use this model to predict allergen or nutrition information.

# Known limitations
This model assumes that its input image contains a well-cropped food dish. If a non-food image is input to the model or if the dish is not well-cropped, the output of the model may be meaningless. This model was trained on a dataset skewed toward North American foods.

# The Code
<a href="https://github.com/thecodemancer/Model-for-Food-Classification/blob/bc11bfe804eda06d68dd6efa2835c52dd45e3612/Model_for_Food_Classification.ipynb" title="The Code">The code is here</a>
