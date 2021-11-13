# Multi-headed vertical federated neural network

Prerequisites
-----
    Python 3.8
    Torch 1.8.0 or Tensorflow 2.3.0
Models&Data
-----
    Learning models: neural networks
    Datasets: Adult
Main Parameters
-----
    parser.add_argument('--dname', default='ADULT', help='dataset name')
    parser.add_argument('--epochs', type=int, default=10, help='number of training epochs')    
    parser.add_argument('--batch_size', type=int, default=128)
    parser.add_argument('--data_type', default='original', help='define the data options: original or one-hot encoded')
    parser.add_argument('--model_type', default='vertical', help='define the learning methods: vrtical or centralized')    
    parser.add_argument('--organization_num', type=int, default='3', help='number of origanizations, if we use vertical FL')
Get Started
-----
    python tf_vertical_FL_train.py --epochs 100 --model_type 'vertical'
    python torch_vertical_FL_train.py --epochs 100 --model_type 'vertical'
    
