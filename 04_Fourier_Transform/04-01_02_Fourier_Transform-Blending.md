# 04 Fourier Transform

## 1. Fourier Transform
  * Using sines and cosines to reconstruct a signal
    * Target singal can be reconstructed by adding cosines
	* ![Target Signal](./Figures/TargetSignal.png)
	* ![Adding Cosines Graph](./Figures/AddingCosinesGraph.png)
	* ![Adding Cosines Formula](./Figures/AddingCosinesFormula.png)		
  * The Fourier Transform
    * Periodic function: An weighted sum of sines and cosines of diffent frequencies
	* Transform f(t) ==> F(w)
	* A reversible operation
	* ![Model Equation](./Figures/ModelEquation.png)	
  * Frequency Domian for a signal
    * View into frequency / time domain
	* ![View into frequency / time domain](./Figures/ViewIntoFreqTimeDomain.png)	
	* ![Time, Frequency, and Frequency Spectra](./Figures/TimeFreqSpectra.png)		
  * 3 properties of convolution relating to Fourier Transfrom
    * Fourier transfrom of a convolution of two function = product of their Fourier transforms
	* ![Property1](./Figures/Property1.png)
	* Inverse Fourier transform of the product of two Fourier transforms = convolution of the two inverse Fourier transforms
	* ![Property2](./Figures/Property2.png)
	* Convolution in spatial domain is equivalent to multiplication in frequency domain
  * Fourier Transforms: Example
    * ![Example1](./Figures/Example1.png)
	* ![Example2](./Figures/Example2.png)
	* ![Example3](./Figures/Example3.png)
	
## 2. Blending
  * Merging two images
    * Cross-Fading
	* ![Cross-Fading1](./Figures/CrossFading1.png)
    * ![Cross-Fading2](./Figures/CrossFading2.png)
	* ![Cross-Fading3](./Figures/CrossFading3.png)
	* ![Cross-Fading_total](./Figures/CrossFadingTotal.png)
  * Window sizes used for merging images
    * To avoid seam: Window = size of <u>largest prominent</u> "feature"
	* To avoid ghosting: Window <= 2x size of <u>smallest prominent</u> "feature"
  * Advantages of a using the Fourier Domain
    * Could be hepful for the right window size ... Largest frequency <= 2x size of smallest frequency
	* Image frequency content should occupy one "octave"
	* Feather: merge the right kinds of things from two different images ... "Blur" the edges before applying the blend operations
	* ![Blur](./Figures/Blur.png)

