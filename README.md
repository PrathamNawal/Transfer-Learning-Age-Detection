<h1>Age Detection of Indian Actors</h1>
<hr />
<p>Indian Movie Face database (IMFDB) is a large unconstrained face database consisting of&nbsp;<strong>34512</strong>&nbsp;images of&nbsp;<strong>100</strong>&nbsp;Indian actors collected from more than 100 videos. All the images are&nbsp;<strong>manually</strong>&nbsp;selected and cropped from the video frames resulting in a high degree of variability interms of scale, pose, expression, illumination, age, resolution, occlusion, and makeup. IMFDB is the first face database that provides a detailed annotation of every image in terms of age, pose, gender, expression and type of occlusion that may help other face related applications. For more details about the data set</p>
<h1>Model Architecture</h1>
<hr />
<p>I have used a pretrained&nbsp;&nbsp;<a href="https://keras.io/applications/">VGG16</a> architecture with <a href="https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/SGD">SGD optimizer</a> in combination with weights of ImageNet data. We have freezed few layers and changed the last softmax layer according to out problem</p>
<p><img src="http://www.cs.toronto.edu/~frossard/post/vgg16/vgg16.png" alt="VGG 16 Architecture" width="470" height="276" /></p>
<h1>Data</h1>
<hr />
<p>The dataset is cleaned and formatted to give you a total of 26742 images with 19906 images in train and 6636 images in test.</p>
<p>The task is to predict the age of a person from his or her facial attributes. For simplicity, the problem has been converted to a multiclass problem with classes as Young, Middle and Old.</p>
<h1>Dependencies :</h1>
<hr />
<ul>
<li>Numpy</li>
<li>Pandas</li>
<li>Matplotlib</li>
<li>Sckit-Learn</li>
<li>Keras (Tensorflow Backend)</li>
</ul>
<h1><strong>Reference:</strong></h1>
<hr />
<p>https://datahack.analyticsvidhya.com/contest/practice-problem-age-detection/</p>
