## Neural Dependency Parser
A Neural Dependency Parser using TensorFlow based on [A Fast and Accurate Dependency Parser using Neural Networks](https://cs.stanford.edu/~danqi/papers/emnlp2014.pdf).

#### How to run
```
python3 model.py --optimizer=adam --lr=0.001 --activation=relu --hidden=4 --hidden_size=500 -l2_beta=10e-8
```

#### Hyper-parameters Options
- learning rate `--lr`
- number of hidden layers `--hidden`
- hidden layer size `--hidden_size`
- number of epochs `--epochs`
- l2 regularization beta `-l2_beta`
- activation `--activation` can be `relu` or `cube`
- optimizer `--optimizer`, can be `adam` or `adagrad`

#### Result
|| Original Result | Adam ReLU 4 layers |
|---|---|---|
|LAS| 92.0 | 90.1 |
|UAS| 90.7 | 91.3 |
