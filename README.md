# opencv-kf-pose-estimation
Tracks human joints (e.g., hands, elbows, knees, etc.) using Pose Estimation and applies a Kalman Filter to reduce noise and smooth movements.

Explanation
--
MediaPipe Pose Estimation
- Detects keypoints (left and right wrist).
- Converts normalized coordinates to pixel coordinates.

Kalman Filter Application
- Each wrist has its own Kalman Filter.
- The filter predicts and then corrects its estimates.

Visualization
- Red Circles → Noisy wrist detections.
- Green Circles → Smoothed Kalman-filtered wrist positions.
