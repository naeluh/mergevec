mergevec
========

Mergevec.py is used to merge .vec files for use in training a cascade with openCV's opencv_traincascade. This code was made as replacement for mergevec.cpp (created by Naotoshi Seo. See: http://note.sonots.com/SciSoftware/haartraining/mergevec.cpp.html) in order to avoid recompiling opencv with mergevec.cpp. 

#To use the function:

	(1) Place all .vec files to be merged in a single directory ("vec_directory").
	(2) Download mergevec.py
	(3) Go to the bottom of mergevec.py and enter the vec_directory name along with an output filename.
	(4) Navigate to mergevec.py in your CLI (terminal or cmd) and type "python mergevec.py".

#To test the output of the function:

	(1) Install openCV.
	(2) Navigate to the output file in you CLI (terminal or cmd).
	(2) Type "opencv_createsample -w img_width -h img_height -vec output_filename". This should show the .vec files in sequence.

The aggregate .vec output from megevec.py has successfully been used to train a cascade. See the below for resources on training cascade classifiers.

#opencv_traincascade Resources

OpenCV:
http://docs.opencv.org/doc/user_guide/ug_traincascade.html

Naotoshi Seo:
http://note.sonots.com/SciSoftware/haartraining.html

Coding Robin:
http://coding-robin.de/2013/07/22/train-your-own-opencv-haar-classifier.html

StackOverflow:
http://stackoverflow.com/questions/16058080/how-to-train-cascade-properly
