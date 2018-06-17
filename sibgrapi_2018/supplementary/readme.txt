% Part of Supplementary Materials
% Online Submission 
ID: 0356
High-Quality Fast non-Blind Deconvolution Using Adaptive Sparse Priors

See supplementary material in files:
index.html (image examples)

Note: The acompanying scripts are intended to facilitate the avaliation of 
our algorithm by the reviewers, please do not re-distribute this material.

%--------------------------------------------------------------------------
'./scripts/demo_our_method.m':

The script 'demo_our_method.m' compares various deconvolution methods with 
our proposed method. The original image is convolved with the 19 x 19 blur 
kernel of Krishnan and Fergus(2009) and 1% of Gaussian noise is added. 

It calls the following scripts that implement the deconvolution algorithms:

%--------------------------------------------------------------------------
Lucy-Richardson: 

uses MATLAB implementation  

%--------------------------------------------------------------------------
Zhou et al method:

./zhou/zhou.m

zhou calls code downloaded from: 
http://www1.cs.columbia.edu/~changyin/SharedCode/ICCP2009/zDemo.html (27/09/2012)
Wiener Deconvolution Using 1/f Law - Changyin Zhou @ Columbia U, 2009'

%--------------------------------------------------------------------------
Levin et al Gaussian prior:

./levin/deconvL2_frequency.m

% script deconvL2_frequency.m downloded from: 
% http://groups.csail.mit.edu/graphics/CodedAperture/DeconvolutionCode.html
% Image and Depth from a Conventional Camera with a Coded Aperture
% Anat Levin, Rob Fergus, Fredo Durand, Bill Freeman

%--------------------------------------------------------------------------
Levin et al Sparse prior:

./levin/deconvSps.m

% script deconvSps.m downloded from: 
% http://groups.csail.mit.edu/graphics/CodedAperture/DeconvolutionCode.html
% Image and Depth from a Conventional Camera with a Coded Aperture
% Anat Levin, Rob Fergus, Fredo Durand, Bill Freeman

%--------------------------------------------------------------------------
Shan et al. method:

./robust_deconv.exe

% program robust_deconv.exe downloded from:
% http://www.cse.cuhk.edu.hk/~leojia/projects/motion_deblurring/index.html
% High-quality Motion Deblurring from a Single Image
% Qi Shan, Jiaya Jia, Aseem Agarwala

%--------------------------------------------------------------------------
Junfeng Yang et al. method:

% FTVd_v4 solves TV models (TV/L2, TV/L1 and their color variants)
% by Alternating Direction Method (ADM).
%
% Copyright (c), May, 2009
%       Junfeng Yang, Dept. Math., Nanjing Univiversity
%       Wotao Yin,    Dept. CAAM, Rice University
%       Yin Zhang,    Dept. CAAM, Rice University
%--------------------------------------------------------------------------
D. Krishnan and R. Fergus method:

% fast_deconv solves the deconvolution problem in the paper (see Equation (1))
% D. Krishnan, R. Fergus: "Fast Image Deconvolution using Hyper-Laplacian
% Priors", Proceedings of NIPS 2009.
%
% This paper and the code are related to the work and code of Wang
% et. al.:
%
% Y. Wang, J. Yang, W. Yin and Y. Zhang, "A New Alternating Minimization
% Algorithm for Total Variation Image Reconstruction", SIAM Journal on
% Imaging Sciences, 1(3): 248:272, 2008.
% and their FTVd code.

%--------------------------------------------------------------------------
Our method:

./our_method/our_method.m

%--------------------------------------------------------------------------
