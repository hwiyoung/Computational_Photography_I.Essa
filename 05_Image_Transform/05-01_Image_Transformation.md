# 05-01 Image Transformation

## Transform the image
  * Image filtering: Change range of image ==> g(x) = T(f(x))
  * Image warping: Change domain of image ==> g(x) = f(T(x))
  * Parametric Global Warping: Translation, Rotation, Aspect, Scale, Perspective, Affine
    * Transformation T is as a matrix transform
	* p' = T p <=> p' = M p
    * ![Parametric Warping](./Figures/ParametricWarping.png)

## Rigid Transformations: Translation, Rotations
  * 2D Rotation
  * ![2D Rotation](./Figures/2DRotation.png)
  * Linear transformation are combinations of (1) Scale, (2) Roation, (3) Shear and (4) Mirror
  * Properties of linear transformations
    * Origin maps to origin
	* Lines map to lines
	* Parallel lines remain parallel
  * 2D Translation
	* ![2D Translation](./Figures/2DTranslation.png)
  * Homogeneous Coordinates
    * Reperesent coordinates in 2D with a 3-vector
	* Add a 3rd coordinate to every 2D point - (x, y, w) => (x/w, y/w)
	* ![Homogeneous Coordinates](./Figures/HomogeneousCoordinates.png)
  * Basic 2D Transformation
    * ![2D Transformation](./Figures/2DTransformation.png)
	* The transformation matrix M can have only **<u>8 parameters</u>**
	* Homogeneous coordinates is independent to scale, **<u>the parameter i can be 1 by dividing by i</u>**

## Affine/Projective Transformation

## Degrees of Freedom for different transformation
