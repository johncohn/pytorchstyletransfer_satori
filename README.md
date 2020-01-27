Ths is a simple pytorch style transfer example adapted from https://pytorch.org/tutorials/advanced/neural_style_tutorial.html
adapted to run on the MIT Satori PowerAI Cluster

## To deploy on Satori do the following:
1. Get access to Satori following  instructions in the [Satori Documentation](https://mit-satori.github.io/satori-basics.html)
2. Point your browse to the [Satori Open On-Demand (OOD)  portal](https://satori-portal.mit.edu/pun/sys/dashboard)
3. On the top menu bar got to **Clusters -> Satori Shell Access** 
4. In the  shell get the test repo by typing  **git clone https://github.com/johncohn/pytorchstyletransfer_satori**
5. Once the git clone is done, go back to the OOD Dashboad window (labeld **My Interactive Sessions**) and go to menu option **Interactive Apps -> Jupyter Notebook**
6. Click the **Launch** button to fire off a Jupyterlab session
7. Click the **Connect to Jupyter** button when it appears in a few moments
8. When Jupyter comes up for the first time, you may be prompted to select a kernel, If so, choose the default **Python 3 PowerAI**
9. Use the left navigation pane to find the git repo directory (**pytorchstyletransfer_satori**) you downloaded in step 4. . click into it and dopuble click on the Jupyter notebook **TorchTransfer.ipynb**
10. before you start running the code select **File -> New -> Terminal** in the Jupyterlab menu bar. 
11. In the terminal that is started paste the command ``watch -n0.1 nvidia-smi``. You should see a continually updating text showing GPU temperature and power.
12. Now switch back to the tab for the **TorchTransfer.ipynb** notebook
13. run the Jupyter frames one by one  using the 'play' arrow button to test.. or go to the menu option **Run -> Run all cells**
14. intermediate  results will appear at the bottom as the program runs. 
15. while the program is running (especially cell 15 in the notebook i.e. ``output = run_style_transfer(cnn, cnn_normalization_mean, cnn_normalization_std, ``...) switch
    to the Terminal tab you created earlier. You should see that the GPU temperature and rate of energy use increase to around 70C and 200W respectively.
16. **Enjoy !!!** -- but also think about the energy you are using and how you might reduce it


## to add your own pictures
you can change  borh the 'style' isource mage and the 'content' target image to use your own. Note the images need to be the same size. THe images here are all 444 x 444 pixels at 72 pixel/inch resultion and are of .jpg format 

*e.g.*

style_img = image_loader("./hippy.jpg")

content_img = image_loader("./jcheadshot2.jpg")
