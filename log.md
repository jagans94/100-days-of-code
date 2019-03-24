# 100 Days Of Code - Log

## List of Projects:
- [P1](https://github.com/jagans94/Coloring-greyscale-images): Learning Pytorch by porting the following [implementation]( https://github.com/emilwallner/Coloring-greyscale-images) from Keras.
- To be added...

### Day 0: March 9th, 2019

**Today's Progress**: Set up a GCP account to do some deep learning. 

**Thoughts:** Done this before, but it seems there were some problems with permissions, authorizations etc. with my gcloud SDK client. It was horribly out of date. So fixed it up and got an instance up and running.`

### Day 1: March 10th, 2019

**Today's Progress**: Coded up an implementation in pytorch.  

**Thoughts:** 
- Looks like you need to initialize all the layers with trainable parameters inside `__init__` function. Otherwise, network doesn't automatically identify it's parameters. The functional implementation doesn't seem to be of much use in such a case. 
- Reworked the implementation; got it executing, but it's giving a weird output. Will need to fix it.

### Day 2: March 11th, 2019

**Today's Progress**: Debugging the weird output.

**Thoughts:** 
- Gives partitioned `orange` and `black` output. Gradient explosion, or `tanh` saturation. I don't see where the problem is. 

### Day 3: March 12th, 2019

**Today's Progress**: Changed network weights.

**Thoughts:** 
- Tried changing the network weights. No use. The output has slightly changed, but still `orange` and `black`. :(

### Day 4: March 15th, 2019

**Today's Progress**: Finished Alpha-notebook implementation in PyTorch.

**Thoughts:** 
- Ran the network today, and it started working. No clue why though! But the weird error stopped. 
- Added some reproducibility code, just in case.

### Day 5: March 24th, 2019

**Today's Progress**: Finished Beta-notebook implementation in PyTorch.
**Thoughts:** 
- Finished the Beta-notebook implementation in PyTorch, even though a bit of correction is left :(
- Some plotting and cleaning up of code is left. 
- `ImageDataGenerator` in Keras generates batches of random affine transformed images from a single input sample. A quasi-similar implementation can be done in PyTorch as well, by Composing the relevant `transforms` together. On the TODO list.
