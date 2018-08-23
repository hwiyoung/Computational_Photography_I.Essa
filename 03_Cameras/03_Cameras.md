# 03 Cameras

## 1. Cameras
  * Rays to pixels  
    * [3D scene] -> Illumination -> Optics -> Sensor -> Processing -> Display -> [Image]
	* ![Single-Lens Reflex Camera](./SingleLensReflexCamera.png)
	* Geomtery(Perspective) / Light scattering
  * A camera without optics
    * 어떤 obstruction 없이 빛이 센서에 닿으면, 물체의 특정 부분이 센서의 특정 부분에 모이지 않아 상이 맺히지 않는다
	* 이 obstruction을 만들어 주는게, pinhole 카메라의 기본 원리!
  * Lens in the camera system
    * Pinhole size ... Light diffraction
	  * Large pinhole = geometric blur
	  * Small pinhole = diffraction blur
	  * Best pinhole = very little light
	* 핀홀을 렌즈로 대체 ... 렌즈가 ray를 모아줌
  * The lens equation
    * Geometric optics
	  * Parallel rays는 렌즈 반대편에서 렌즈로부터 f만큼 떨어진 지점에서 모두 만난다
	  * 렌즈의 중심을 지나는 rays는 굴절없이 지나간다
	* Lens equation
	  * focal length: 무한대에서 온 빛이 렌즈를 통과해 모인 지점과 렌즈 사이의 
	  * ![LensEquation](./LensEquation.png)
	  * 위의 식에서 카메라와 물체의 거리가 매우 멀면(o ≒ ∞), 초점거리와 이미지의 거리는 같아진다! (f = i)
## 2. Lenses
  * Focal length
    * Object distance가 길면 렌즈에 맺히는 상의 크기는 작아진다(Object distance ↑ => Image size ↓)
	* Focal length가 길어지면 맺히는 상의 크기 커진다(Focal length ↑ => Image size ↑)
	* Focusing: moving sensor back or forward w.r.t. to lens
  * Field of View(FOV)
    * Sensor size(h) ↓ => FOV ↓
	* Focal length(f) ↑ => FOV ↓
	* ![Field of View(FOV)](./FOV.png)
  * Sensor size
    * There are many kinds of sensor size: Full frame to iPhone
	* ![Sensor sizes](./SensorSizes.png)
	* 1.26, 1.5 등의 crop factor는 [풀프레임의 대각선 길이 / 해당 센서의 대각선 길이]로 계산
    * Crop factor(위 그림의 (1:1.26)에서 1.26과 같은 표시)를 통해 렌즈의 환산 focal length를 알 수 있다!
	* 센서 타입의 1/2'' 등은 해당 센서 대각선 길이를 인치로 표현한 것 ==> 진공관 길이 1/2'' = 센서 대각선 길이 8mm
	  * 진공관 vs. 센서 - https://blog.naver.com/jazz_mir/60038917792
  * Image Formation & Capture
    * Changing focal length allows us to move back and capture the scene
	* ![Changing focal length](./Changing_focal_length.png)
	* f가 18mm 일 때 보다 180mm 일 때 카메라와 객체 간의 실제 거리는 더 길지만, 화면상으로 큰 차이가 없게 느껴진다
	* 두 객체 간의 거리는 f가 18mm 일 때 보다 180mm 일 때, 더 가깝게 느껴진다
  * Perspective Projection
    * 기본적인 카메라 모델: Perspective projection model
	* ![Camera model](./CameraModel.png)
	* 영상이 inverted 되는 것을 고려해 영상의 투영면을 반대편에 가정
## 3. Exposure
## 4. Sensor