## Project 5 : Image Segmentation with SLIC Pixels.


## Project Description

### Usage : 

``cd build && cmake ..``, then `make`

---
**Command Line Argument**
```./slic [-h] [--algorithm=a] [--ruler=r] input_image```

**Here is the information for each arguments :**

- slic 			 : Name of executable
- algorithm     : Name of `SLIC` algorithm variant
  - `SLIC` segments image using a desired region size
  - `SLICO` optimizes using an adaptive compactness factor
  - `MSLIC` optimizes using manifold methods giving more context-sensitive super-pixels
- size             : Chooses an average super-pixel size measured in pixels [default: 10]
- ruler            : Chooses the enforcement of super-pixel smoothness [default: 10.0]

### Input Image
<p align="center">
  <img src="./img/korea.jpg" width="270" height="334" >
</p>

### Output Image
`left to right algorithm SLIC, SLICO and MSLIC. (Constant Size = 25)`
<p float="center">
  <img src="./img/korea_slic_-a=0_-s=25.jpg" width="270" />
  <img src="./img/korea_slic_-a=1_-s=25.jpg" width="270" /> 
  <img src="./img/korea_slic_-a=2_-s=25.jpg" width="270" />
</p>

`left to right algorithm SLIC, SLICO and MSLIC. (Constant Size = 50)`
<p float="center">
  <img src="./img/korea_slic_-a=0_-s=50.jpg" width="270" />
  <img src="./img/korea_slic_-a=1_-s=50.jpg" width="270" /> 
  <img src="./img/korea_slic_-a=2_-s=50.jpg" width="270" />
</p>

