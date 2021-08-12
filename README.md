## Parameter

--model : path to an existing model for testing
--selection : number from 0-6 that represents the sampling selection method
 * 0 = Random Offline Pair
 * 1 = Hard Negative Online Par 
 * 2 = All Positive Online Pair 
 * 3 = Random Offline Triplet 
 * 4 = All Positive Online Triplet 
 * 5 = Random Negative Online Triplet 
 * 6 = Semi-hard Negative Online Triplet

--dataset : number from 0-2 that represents the dataset
 * 0 = MNIST
 * 1 = KMNIST
 * 2 = FashionMNIST

--out : output path to save the results

## Train model 

example to train Random Offline Pair Selection on KMNIST dataset
```bash
python main.py --dataset 1 --selection 0
```

## Test model 
example to test Hard Negative Online Pair Selection on KMNIST dataset  
all trained models can be found in the models folder

```bash
python main.py --model ./models/KMNIST/HardOnlinePairSelection_model.pt --dataset KMNIST --selection 1
```
