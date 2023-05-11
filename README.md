First aproach was creating a simple CNN with a single convolution and pooling layer that was then flattened.
0.5130 - accuracy: 0.0318
333/333 - 1s - loss: 0.6743 - accuracy: 0.0548 - 1s/epoch - 4ms/step

With tree form of convolutional and pooling layers followed by a two dense layers flattened.
2s 25ms/step - loss: 0.0346 - accuracy: 0.9921
40/40 - 1s - loss: 0.0733 - accuracy: 0.9794 - 503ms/epoch - 13ms/step
"my_model.h5"

The same as above with dropout 0.5.
2s 28ms/step - loss: nan - accuracy: 0.2148
40/40 - 1s - loss: nan - accuracy: 0.0413 - 639ms/epoch - 16ms/step
"my_model.h6"

2s 28ms/step - loss: 0.0337 -accuracy: 0.9947
40/40 - 1s - loss: 0.1546 - accuracy: 0.9627 - 509ms/epoch - 13ms/step
"tree_ConvPoolDense.h5"

2s 29ms/step - loss: nan - accuracy: 0.2069
40/40 - 0s - loss: nan - accuracy: 0.0540 - 439ms/epoch - 11ms/step
"tree_ConvPoolDenseDropout05_nn.h5"

1s 14ms/step - loss: 0.0306 - accuracy: 0.9884
40/40 - 0s - loss: 0.3405 - accuracy: 0.9365 - 430ms/epoch - 11ms/step
"tree_1LConvPoolDense.h5"
