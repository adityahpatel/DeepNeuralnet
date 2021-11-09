I took a toy dataset of about 250 images of size 64 x 64 x 3. Some were inages of cats, others weren't. Then split into train-test. 

Built binary classifier to classify them as cats (1) or non-cats (0) <br>
Initially implemented logistic regression from scratch i.e. calculated linear sum--> relu--> linearmsum--->sigmoid, calculated total loss over 200 training images ---> calculated gradient of loss with respect to all weights and biases. <br> 
Trials:
(1) Built a 1 layer logistic regression predictor (Not uploaded in this repo)
<br> 
<br>
(2) Built a 2 layer neural network to do the same binary classification task <br>
<br>
<br>
(3) built a 4 layer neural network to do the same binary classification task>br>
<br>
<br>
Then built a L-layer neural network where user can specify any depth of neural net and any size of the neurons in each layer. layer_dims controls this parameter so suppose a 6 layer neural network would be layer_dims = [12288, 4,4,3,3,1] where 1st layer is flattened input layer of size 64 x 63 x 3 = 12288 neurons, 2nd layer has 4 neurons, 3rd layer has 4 neurons, 4th layer has 3 neurons, 5th layer has 3 neurons and final 6th outpout layer has 1 neuron.<br>
<br>
I have used RELU for all hidden neurons and sigmoid for output. Alternatively tanh can be used too. Avoided Sigmoid for all hidden layers except output layer. TanH mean-centers the data and Relu converges faster, so they're better than Sigmoid. 

Future Work: No dropout layers, early stopping etc is implemented. Therefore, neural network overfits which is pretty common
