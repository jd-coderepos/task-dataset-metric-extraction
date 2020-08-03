# Task Dataset Metric Software Extraction

This program produces the test data for classification over a set of predefined task#dataset#metrics#software labels.

Given input a pdf file, it scrapes the text from the filw using the Grobid parser, subsequently generating the test data file for input to the neural network classifier.

### Steps to run the program


1. Clone this repository (https://github.com/jenlindadsouza/task-dataset-metric-extraction)
2. The program jar file can be found at https://github.com/jenlindadsouza/task-dataset-metric-extraction/tree/master/build/libs <br>
&nbsp;&nbsp;&nbsp;&nbsp; - It is called `tdm-1.0.jar`
3. `Usage: java -jar tdm-1.0.jar <pdf-file-path> <resources-dir>`
Where the `pdf-file-path` is the input pdf article to extract task, dataset, metric, software elements from and `resources-dir` should point to the directory at https://github.com/jenlindadsouza/task-dataset-metric-extraction/tree/master/src/main/resources
4. To run directly from the source code, the build file will have to be updated for the local dependencies for jar files. See here: https://github.com/jenlindadsouza/task-dataset-metric-extraction/blob/master/build.gradle
5. Either the jars can be obtained from source. For convenience, they are also made available here https://drive.google.com/drive/folders/1ax7ah8AInoD-_7amx27VKaSrFV73ggEk?usp=sharing


Acknowledgement: This program reuses code modules from IBM's science-result-extractor (https://github.com/IBM/science-result-extractor). A reference url to their paper on the ACL anthology is https://www.aclweb.org/anthology/P19-1513
