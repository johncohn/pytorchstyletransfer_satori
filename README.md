Ths is a simple pytorch style transfer example adapted from https://pytorch.org/tutorials/advanced/neural_style_tutorial.html
adapted to run on the MIT Satori PowerAI Cluster

## To deploy on Satori do the following:
1. Get access to Satori following  instructions in the [Satori Documentation](https://mit-satori.github.io/satori-basics.html)
2. Point your broswer to the [Satori Open On-Demand portal](https://satori-portal.mit.edu/pun/sys/dashboard)
< more to come afeter we test>


## to add your own pictures
you can change  borth the 'style' isource mage and the 'content' target image to use your own. Note the images need to be the same size. THe images here are all 444 x 444 pixels at 72 pixel/inch resultion and are of .jpg fomrat 

e.g.
style_img = image_loader("./hippy.jpg")
content_img = image_loader("./jcheadshot2.jpg")
