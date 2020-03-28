# Convolutional-neural-network


Execution Result :
Using TensorFlow backend.
Found 16 images belonging to 2 classes.
Found 16 images belonging to 2 classes.
Epoch 1/1
5000/5000 [==============================] - 43070s 9s/step - loss: 0.0033 - accuracy: 0.9990 - val_loss: 1.3871e-07 - val_accuracy: 1.0000


Validation and prediction results :
import numpy as np
from keras.preprocessing import image
test_image = image.load_img(r'C:\Users\vinodhkumarb\Desktop\Ineuron-DL\Image classification task\758.jpg', target_size = (64, 64))
test_image = image.img_to_array(test_image)
test_image = np.expand_dims(test_image, axis = 0)
result = classifier.predict(test_image)
training_set.class_indices
if result[0][0] == 1:
    prediction = 'Vino'
    print(prediction)
else:
    prediction = 'Mithu'
    print(prediction)
    
Vino ==> output
