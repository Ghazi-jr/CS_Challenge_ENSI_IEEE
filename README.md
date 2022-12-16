This work is the Reproducibility of the paper "Segmentation Convolutional Neural Networks for Automatic Crater Detection on Mars" .

------------------

The Folder Structure of the project : 

	* doc : Contains README File with instructions on How to execute the project.
	* Scripts :  Notebook Containing the Full implementation of the code.

------------------

Because of the capabilities and performance of the hardware provided by Google, we focused our efforts on implementing the solution in a collaborative environment. (Google Colab) also this enables the users to not manage Complex Dependencies.

To Run The Notebook : 

	* Simply Upload The Notebook To Google Colab.
	* Make Sure that the execution mode is set to GPU.

The Notebook is Devided into Sections : 

	* Data and Libraries Loading : The Target Data (Annotated Data) is Downloaded From Ieee Portal so Make sure always to copy the zip download url from this website : "https://ieee-dataport.org/open-access/mars-crater-segmentation-datasetand" .  The Original images are scraped from this website : "https://www.mars.asu.edu/data/thm_dir/large/v1.0/".
	* Execute Model Architecture (This Notebook uses Tensorflow.keras to create the U-Net Model).
	* Execute Training Utils.
	* Execute Model Creation.
	* Training Section : We Trained our models based on the test scenarios specified in the paper.
	* Crater Counting and Matching.
	* Last Section is About The optimization Part.

(New Paper is created after the optimization to showcase our method).
		
------------------
Constraints : 

*   Computing Power : somehow the colab and the laptops used arent able to process the same Data size in the input so we downsampled our Data and we got pretty much the same results. Also the crator Counting Part works only on one image (RAM Problems).
*   Results From Section IV-B : Since these section is all about changing data Size of the Train and that was a problem to implement we didn't Implement the same results so all the notebook and Code is About Testing and Inspecting the results of the Other Sections : IV-A and Crater Counting Algorithm.

------------------
Implementation : 

*   We Implemented and Tested all the Authors Test However we presented some chosen algorithms that showed the Best Results :

  	*   For Solid Target : We Implemented The Test Number 4 
  	*   For Thick Target : We Implemented the Test Number 3 
  	*   For Thin Target  : We Implemented the Test Number 6 
