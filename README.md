# Caffe for MSG-Net (Multi-scale guidance network)

This repository is the release of <strong>MSG-Net</strong> for our paper <a href="http://personal.ie.cuhk.edu.hk/~ccloy/files/eccv_2016_depth.pdf"><strong>Depth Map Super-Resolution by Deep Multi-Scale Guidance </strong></a> in ECCV16. It comes with 4 trained networks (x2, x4, x8, and x16) and 3 hole-filled testing sets (A, B, and C).

To the best of our knowledge, MSG-Net is the <strong>FIRST convolution neural network</strong> which attempts to <strong>1) upsamples depth images</strong> and <strong>2) uses the multi-scale guidance from the corresponding high-resolution RGB images</strong>.

Another <a href="https://github.com/twhui/MS-Net">repository </a> for <strong>MS-Net</strong> (without multi-scale guidance) is also available.

For more details, please visit the <a href="http://mmlab.ie.cuhk.edu.hk/projects/guidance_SR_depth.html">project page </a>.

# Dependency
We train our models using <a href="https://github.com/BVLC/caffe">caffe</a> and evaluate the results on Matlab.

# Installation and Running
You need to install <a href="https://github.com/BVLC/caffe">caffe</a> and remeber to complie matcaffe. You can put the folder <code>MSGNet-release</code> in <code>caffe/examples</code>. Finally, you need to get into the the directory of <code>examples/MSGNet-release</code>, and run <code>MSGNet.m</code>. </li>

# Training data
Our <a href="https://www.dropbox.com/sh/p45abqvpzv66m2p/AACwDh0iIu67Us3IPLusfPXXa?dl=0e">RGBD training set</a> consists of 58 RGBD images from <a href="http://sintel.is.tue.mpg.de/depth">MPI Sintel depth dataset</a>, and 34 RGBD images from <a href="http://vision.middlebury.edu/stereo/data/">Middlebury dataset</a>. 82 images are used for training and 10 images (frames 1, 20, 28, 58, 64, 66, 69, 73, 75 and 79) are used for validation.

# License and Citation
All code is provided for research purposes only and without any warranty. Any commercial use requires our consent. When using the code and/or training data in your research work, please cite the following paper:

"T.-W. Hui, C. C. Loy and X. Tang, Depth Map Super-Resolution by Deep Multi-Scale Guidance, pp. 353–369, ECCV16".
