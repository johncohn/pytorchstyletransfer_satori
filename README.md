Ths is a simple pytorch style transfer example adapted from https://pytorch.org/tutorials/advanced/neural_style_tutorial.html
adapted to run on the MIT Satori PowerAI Cluster

## To deploy on Satori do the following:
1. Get access to Satori following  instructions in the [Satori Documentation](https://mit-satori.github.io/satori-basics.html)
2. Point your browse to the [Satori Open On-Demand (OOD)  portal](https://satori-portal.mit.edu/pun/sys/dashboard)
3. On the top menu bar got to **Clusters -> Satori Shell Access** 
4. In the  shell get the test repo by typing  **git clone https://github.com/johncohn/pytorchstyletransfer_satori**
5. Once the git clone is done, go back to the OOD Dashboad window (labeld **My Interactive Sessions**) and go to menu option **Interactive Apps -> Jupyter Notebook**
6. Click the **Launch** button to fire off a Jupyterlab session
7. CLick the **Connect to Jupyter** button when it appears in a few moments


## to add your own pictures
you can change  borth the 'style' isource mage and the 'content' target image to use your own. Note the images need to be the same size. THe images here are all 444 x 444 pixels at 72 pixel/inch resultion and are of .jpg format 

*e.g.*

style_img = image_loader("./hippy.jpg")

content_img = image_loader("./jcheadshot2.jpg")
