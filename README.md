# -Video-Stabilisation-using-Matrix-Transformation

## 1.0 INTRODUCTION
This project focuses on stabilizing videos captured on mobile devices using matrix transformation techniques. Shaky footage caused by hand tremors or device movements is corrected by aligning frames through translation, rotation, and scaling. The system applies linear algebra methods, including affine transformations, optical flow, and least squares optimization, to reduce shakiness and improve video quality. Trajectory smoothing ensures gradual adjustments, preserving the visual coherence of the video.
Key features of this project:
- Video frame stabilization using matrix transformations
- Motion estimation using optical flow
- Frame alignment using affine transformations
- Trajectory smoothing with moving average filters
- Evaluation using structural similarity (SSIM)

## 2.0 OBJECTIVES
- Improve stability and clarity of videos captured on mobile devices
- Reduce shakiness and maintain consistent frame alignment
- Evaluate matrix transformation techniques on various video types
- Demonstrate practical applications of linear algebra in video stabilization

## 3.0 DATA SOURCES
The project uses multiple video sources for stabilization:
- **Youtube-8M Dataset:** Diverse videos with varying motion and lighting
- **UCF101 Action Recognition Dataset:** 13,320 action videos from 101 categories
- **Optical Flow Data:** Lucas-Kanade or Frameback methods for pixel motion estimation
- **Sample Videos:** Personal handheld recordings and publicly available clips from Vimeo/Pexels

## 4.0 RUNNING THE SCRIPT
To stabilize a video, run:
python src/video_stabilization.py --input videos/input/sample_video.mp4 --output videos/output/stabilized_video.mp4

The program will:
- Load the input video
- Track pixel movements using optical flow
- Apply affine transformations and frame alignment
- Smooth trajectories and generate stabilized video
- Save output in the specified folder

## 5.0 EVALUATION
The output video is evaluated visually and quantitatively using:
- Structural Similarity Index (SSIM)
- Comparison between original and stabilized frames
- Reduction in abrupt camera movements and improved visual smoothness

## 6.0 REQUIREMENTS
- OpenCV (`opencv-python`), NumPy, SciPy, Matplotlib

## 7.0 LICENSE
This project is for educational purposes.

## 8.0 AUTHORS & CREDITS
Iman A., Fatin A.K., Fitrah M.R., Zullaikha Z.
Created as part of Maths for Computing 3 group project.

- Roberto, M. e. et al., Survey on Digital Video Stabilization, ACM CS, 2023

