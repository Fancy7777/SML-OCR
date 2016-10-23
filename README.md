# SML-OCR
A project that reads historical books character and make classification. The formal competition is in Kaggle.

Optical Character Recognition (OCR) is an important machine learning application which converts an image of a printed document into text. This is a useful tool for digitising vast collections of books such as in libraries, meaning that text can be used efficiently for efficient searching and other applications. While OCR for modern documents is largely a solved problem, it remains very challenging case for historical documents. Early printing presses required manual selection and placement of each of the characters by the printer, and features wandering baselines,1 ink splodges, use of odd fonts and caligraphic capitals, and the use of characters that are no longer in use in modern texts. See the figure below for an example. Added to this scanning artefacts such as ghosting of the reverse page and the curvature of the page towards the spine are often a problem. Together these issues mean that off the shelf application of modern OCR technologies produce mostly gibberish, and consequently is of little practical use.
In this project you will develop character classifiers for several historical documents, each produced shortly after the advent of the printing press. Note that these documents are in different languages, use different fonts, and have other idiosyncrasies specific to their author and printer. Your job is to identify for a given bitmap image of a character the identity of that character.

# Solution
1. After preprocessing, we centered the images and reduce some noise
2. we use cosine KNN to get around 80% accuracy
3. We use random forest to get around 80% accuracy
4. We use Convolutional Neural Network to get around 81% accuracy
5. Use ensemble method to combine above 4 methods to get our final classifier

A better method was the other group's that can improve the accuray further, which is that after CNN, they use SVM to classify CNN's result.

Another groups method also generates good accuracy, however, they put more effort in preprocessing images. The specific method is in the ppt.
