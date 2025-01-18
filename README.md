HUMAN POSE ESTIMATION

MediaPipe Pose Detection - Video and Image Processing
This project uses Google Colab along with the MediaPipe library to process video and image files. It performs pose detection on the input video or image and overlays the detected pose landmarks. The code handles both video and image files and provides processed outputs with landmarks drawn on them.

Features:
Pose Detection for Videos: The code processes video files, detects human pose landmarks, and overlays the landmarks on each frame. The processed video is saved with the landmarks visible.
Pose Detection for Images: The code can process individual image files and display the pose landmarks on the image.
Video Re-encoding: Processed video is re-encoded into MP4 format for easy download.
Requirements:
Google Colab: This code is designed to run on Google Colab for easy integration with uploaded files.
MediaPipe: Used for real-time pose detection.
OpenCV: For video and image processing.
FFmpeg: For video re-encoding (only applicable to videos).
Setup:
Install Dependencies:

Ensure that the following libraries are installed in your Colab environment:
mediapipe
opencv-python
ffmpeg
Upload Files:

The code supports both video (.mp4, .mov) and image formats.
Upload the file using the upload widget (only available in Colab after executing the code cell).
How It Works:
File Upload: The user uploads a file (image or video) to the system.
Processing:
If the file is a video, the code processes each frame, applies pose detection using MediaPipe, and writes the frame with detected landmarks to a new video file.
If the file is an image, the code applies pose detection and shows the processed image with landmarks.
Output:
For video, the processed video is saved and re-encoded in MP4 format for download.
For images, the processed image is displayed directly in the notebook.
Code Workflow:
Upload File: The file is uploaded from the user's local machine.
Check File Type:
If the file is a video (either .mp4 or .mov), the code processes each frame and applies pose detection.
If the file is an image, the code directly applies pose detection to the image.
Pose Detection:
The MediaPipe Pose model detects human pose landmarks (key points on the body like head, shoulders, knees, etc.).
Save or Display Output:
For videos, the output is written to a temporary file and re-encoded into MP4 format.
For images, the processed image with landmarks is displayed inline in the notebook.
Download Processed Video or Image:
The processed video is available for download in MP4 format.
The processed image is displayed directly in the notebook for review.
Example Usage:
Video Input:
Upload a .mp4 or .mov file. The code processes each frame and outputs a video with landmarks.
Image Input:
Upload an image file (JPEG, PNG, etc.), and the code will display the image with pose landmarks.
Output:
Video Output: The video with landmarks is saved as output_video_with_landmarks.mp4.
Image Output: The processed image is displayed inline in the notebook.
Troubleshooting:
If you encounter errors, check if the file is in the correct format (video or image).
Ensure that MediaPipe, OpenCV, and FFmpeg are correctly installed in the Colab environment.
