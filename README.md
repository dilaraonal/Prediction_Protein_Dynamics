# Deep learning model for protein dynamic structure prediction

## Introduction

Proteins are macromolecules that help the regularization of our biological system. They affect several pathways in our body and generate many diseases protein problems.
Because of this understanding of protein structure and functions is important for creating treatments. Proteins have specific 3D structures and they are dynamic.
Experimental methods such as NMR (Nuclear Magnetic Resonance) and SAXS (Small-Angle X-ray Scattering) were first used to analyze the structures of proteins.
NMR provides information about protein structure by examining the resonance behavior of atomic nuclei under magnetic fields.
In general, the magnetic properties of nuclei such as hydrogen, carbon, and nitrogen in proteins are used. SAXS provides information about the general shape and size of proteins in solution. When the protein is exposed to X-rays, the intensity of the scattered rays at small angles is measured. These methods have certain limitations and disadvantages such as high cost, difficulty in data analysis in large-sized proteins, and technical complexities.

Simulations were used for the dynamic properties of the obtained 3D structures (Molecular Dynamics simulations), these simulations calculated the new positions of the atoms by taking the distances and movements of each other as reference with physical calculations and created the movements of the protein as a result of these calculations. However, this method also had disadvantages in terms of cost and time. In recent years, the developing field of artificial intelligence has produced developments that are solutions to these problems. The artificial intelligence system alphafold developed by DeepMind has made a great impact in the scientific world by managing to predict the three-dimensional structure of proteins from the amino acid sequence. With alphafold, a deep learning model, specific 3D structures of proteins could be created without using costly techniques. With these developments, current studies have accelerated research to predict the dynamic structures of proteins using artificial intelligence. In the few studies conducted in this field, the coordinate data obtained with md simulations were selected as the data source required for the training of the deep learning model. As a solution to the cost of working and long-term formations of MD simulations, it would be sufficient for the simulation to produce data short enough for the training of the model. This field is quite new in the literature and there are methods that are produced quite quickly. In this study, an variational autoencoder (VAE) model training was performed with the obtained md simulation data and the results were analyzed to examine how successful it was for dynamic structure estimation.

## Requirements
**Biobox**

**Tensorflow**

**Keras**


## References

1. Zhu, J. J., Zhang, N. J., Wei, T., & Chen, H. F. (2023). Enhancing conformational sampling for intrinsically disordered and ordered proteins by Variational autoencoder. International Journal of Molecular Sciences, 24(8), 6896.
2. Gupta, A., Dey, S., Hicks, A., & Zhou, H. X. (2022). Artificial intelligence guided conformational mining of intrinsically disordered proteins. Communications biology, 5(1), 610.
3. Janson, G., Valdes-Garcia, G., Heo, L., & Feig, M. (2023). Direct generation of protein conformational ensembles via machine learning. Nature Communications, 14(1), 774.
