# PyTorch-ML

**PyTorch model building essentials**
- PyTorch has four (give or take) essential modules you can use to create almost any kind of neural network you can imagine.
They are torch.nn, torch.optim, torch.utils.data.Dataset and torch.utils.data.DataLoader. For now, we'll focus on the first two and get to the other two later (though you may be able to guess what they do).

| PyTorch module | What does it do? |
| ----- | -----|
|  torch.nn | Contains all of the building blocks for computational graphs (essentially a series of computations executed in a particular way).|
| torch.nn.Parameter | Stores tensors that can be used with nn.Module. If requires_grad=True gradients (used for updating model parameters via gradient descent) are calculated automatically, this is often referred to as "autograd".|
| torch.nn.Module | The base class for all neural network modules, all the building blocks for neural networks are subclasses. If you're building a neural network in PyTorch, your models should subclass nn.Module. Requires a forward() method be implemented.|
| torch.optim | Contains various optimization algorithms (these tell the model parameters stored in nn.Parameter how to best change to improve gradient descent and in turn reduce the loss).|
| def forward() | All nn.Module subclasses require a forward() method, this defines the computation that will take place on the data passed to the particular nn.Module (e.g. the linear regression formula above).|

If the above sounds complex, think of like this, almost everything in a PyTorch neural network comes from torch.nn,
- nn.Module contains the larger building blocks (layers)
- nn.Parameter contains the smaller parameters like weights and biases (put these together to make nn.Module(s))
- forward() tells the larger blocks how to make calculations on inputs (tensors full of data) within nn.Module(s)
- torch.optim contains optimization methods on how to improve the parameters within nn.Parameter to better represent input data

![Image](https://github.com/andysingal/PyTorch-ML/blob/main/Images/Screen%20Shot%202023-04-08%20at%206.59.59%20PM.png)

Books:
- Deep Learning with PyTorch Thomas Viehmann, Eli Stevens, Luca Pietro Giovanni Antiga https://learning.oreilly.com/library/view/deep-learning-with/9781617295263/Text/10.xhtml#sigil_toc_id_193
- Inside Deep Learning Edward Raff https://learning.oreilly.com/library/view/inside-deep-learning/9781617298639/
- Awesome-Deep-Camera-Calibration https://github.com/KangLiao929/Awesome-Deep-Camera-Calibration
- The ultimate guide on installing PyTorch with CUDA https://medium.com/decodingml/the-step-by-step-guide-on-how-to-install-pytorch-with-cuda-support-in-all-possible-ways-147b3f34085c

[huggingface-pytorch](https://github.com/huggingface/transformers/tree/main/examples/pytorch)
