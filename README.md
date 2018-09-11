# Recognition of handwritten digits from the mnist data-set, as well as recognition of the custom data-set drawn in Photoshop



НС для классификации картинок с одним цветовым каналом (градации серого) размером 28 x 28 пикселей. Классифицируются 10 различных объектов / классов  с 10 нейронами и функцией активации softmax.

softmax возвращает вероятность принадлежности картинки к каждому классу. Т.е. на выходе получается матрица с 10-ю столбцами (один столбец на каждый класс) с вероятностями.

Слой Dense - это простой полносвязный слой, когда каждый нейрон предыдущего слоя связан с каждым нейроном данного. Обычно во всех сверточных сетях в последних слоях используют 2-3 полносвязных слоя, которые следуют за слоями свертки, пулинга и "выпрямления" (слой: Flatten).

слой Flatten - "выпрямляет" 2+-мерные матрицы в одномерные вектора. Например из матрицы размерности (64, 32, 32) получится одномерный вектор с 64 * 32 * 32 = 65536 элементов.

Dropout - один из методов регуляризации (используется для борьбы с переобучением).

relu - одна из самых популярных нелинейных функций активации нейронов:

f(x) = max(0, x)

MaxPooling2D(pool_size=(2, 2)) проплывает окошком размером (2, 2) по матрице и для каждого окошка выбирает максимальное значение, уменьшая размер исходной матрицы

# Eng
Neural network for classification of images with one color channel (grayscale) with a size of 28 x 28 pixels. 10 different objects / classes with 10 neurons and softmax inclusion functions are classified.

softmax returns the probability of the picture number to each class. Those. the output is a matrix with 10 columns (one column per class) with probabilities.

The Dense layer is a simple, fully connected layer when each of them is connected to each of them. Usually in all convolutional networks in the last layers 2-3 layers are used, which follow the layers of convolution, pulling and "straightening" (layer: smooth).

The Flatten layer "straightens" 2 + -dimensional matrices into one-dimensional vectors. For example, from a matrix of dimension (64, 32, 32) we obtain a one-dimensional vector with 64 * 32 * 32 = 65536 elements.

Dropout - one of the methods of regularization (used to combat re-training).

relu is one of the most popular nonlinear activation functions of neurons:

f (x) = max (0, x)

MaxPooling2D (pool_size = (2, 2)) swims by a window (2, 2) in the matrix and for each window selects the maximum value, reducing the size of the original matrix

![alt text](https://github.com/poteminr/PoteminMnistPrediction/blob/master/logo.jpg)
