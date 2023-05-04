Download Link: https://assignmentchef.com/product/solved-cs6375-assignment-5-k-means-clustering-on-images
<br>
In this problem, you will use K-means clustering for image compression. Two image files provided in the elearning. The assignment task is to display the images after data compression using K-means clustering for different values of K (2, 5, 10, 15, 20).

Is there a tradeoff between image quality and degree of compression? What would be a good value of K for each of the two images?

<table width="642">

 <tbody>

  <tr>

   <td width="642">from matplotlib import pyplot as io import numpy as np from PIL import Image # Image to arrayimg1 = io.imread(imagefilename)  #image is saved as rows * columns * 3 array  print (img1)#Array to image filearray = np.zeros([10,20,3], dtype = np.uint8) array[:,:10] = [255, 128, 0]    # Orange left side array[:,10:]  = [0,0,255]   # Blue right side</td>

  </tr>

 </tbody>

</table>

Note that your program must compile and we should be able to replicate your results.

Otherwise no credit will be given.

What to turn in:

<ol>

 <li>Your code and datasets</li>

 <li>A README for your compiling/using your code</li>

 <li>A report (pdf or doc file) containing answers to the questions posed.</li>

</ol>




<strong><em>The following code is for reading and writing Image Files: Image to RGB array or RGB array to image: </em></strong>




print(array) img2 = Image.fromarray(array) img2.save(‘testrg.png’)


