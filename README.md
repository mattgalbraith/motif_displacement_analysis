# Analysis of the co-occurrence between TF DNA Binding Motifs and ehancer RNA origins
Hello! This github rep contains two things:

  1) A jupyter notebook that takes you step by step through methods and capabilities in the package directory

  2) And of course the actual python package
  
The jupyter notebook along with this code is in large part meant to complement the Azofeifa et al. 2016 Paper "Enhaner RNA profiling predicts transcription factor activity." Below are some images  hat can be easily generated by this package. 

The python dependencies are minimal
  
  1) Numpy  2) Scipy 3) Matplotlib
  
To download the jupyter / ipython notebook software please go to: http://jupyter.org

Please feel free to contact me with errors, bugs or  additional features at joseph[dot]azofeifa[at]colorado[dot]edu



![alt tag](https://github.com/azofeifa/motif_displacement_analysis/blob/master/images/pic2.png)

Above: Analyzing the co-occurrence between two genomic features is a common problem in genomics research. Specifically, we are interested in the relationship between TF-DNA binding motifs and sites of non-promoter associated bidirectional transcription. The above histogram shows the frequency of observe a TF-DNA binding motif at any eRNA within a 1.5 KB window. This figure can be generated by invoking the show_motif_displacement function within the load module.


![alt tag](https://github.com/azofeifa/motif_displacement_analysis/blob/master/images/pic1.png)

Above: Analyzing changes in the co-occurrence between two genomic features is also of interest genomics researcher. Here, we are interested in changes in the co-localization of TF-DNA binding motifs and sites of non-promoter associated bidirectional transcription following experimental perturbation. For this we developed, the motif displacement score which quantifies the propotion of displaced motifs with 150 base pairs of any bidirectional origin. Significance can be easily calculated by Z-test. This figure can be generated by invoking the differential_single method part of the mds_frame frame found within differential_MD module.



![alt tag](https://github.com/azofeifa/motif_displacement_analysis/blob/master/images/pic3.png)

Above: Analyzing changes in MD scores across multiple datasets. This method allows users to perform spline interpolation, filter insignificant changing profiles and compute changes relative to any start dataset (might be interpreted as velocity) and between adjacent pairwise datasets (acceleration)


