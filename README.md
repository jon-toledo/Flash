![GitHub Logo](https://github.com/jon-toledo/Flash/blob/master/images/FLASH.png)

# FLASH: A neural network for climbing route recognition.

Flash is a convolutional neural network which takes a picture of rock climbing route as input, and as output gives the name and grade of the route.  The network is trained using about 200 images of each route taken from various positions during a small time period.  The challenge is then to classify new images taken from arbirary positions and under arbitrary conditions (weather, time of day, season).

Standard practice among climbers is to use a guidebook or 'topo' in order to identify specific outdoor climbing routes. This turns out to be much harder than one may naively expect. Determining 'which route is which' using the (often sparse) information of the guides is a hard problem! When exploring a new area, a great deal of valuable climbing time is lost on this task.

The eventual goal of this project is to develop a point-and-shoot mobile app which climbers can use to identify climing routes so they can spend less time staring at guide books and more time climbing!  

<!## Current status

This is an ongoing project. As I have already mentioned, the eventual goal is to develop a mobile app which takes data from your phones camera as input, feeds this data into a pre-trained neural network, and produces route data as output (e.g. the name and difficulty grade of the route). 

The current status of the project is much more humble and is only a proof of concept. I choose 4 different climbing routes in a popular sector of the local climbing area Mount Nemo. Lets call them route 1, ...., route 4. I took 200 pictures of each route from various angles -- this constituted the training set. My wife then took around 50 pictures of each route from various positions of her own choosing -- this constituted the test set. The goal was to train a neural network that would correctly classify the images in the test set.  

The first step is just to concentrate on training data and testing data collected on the same day, but independently by different people. This is a fairly simple problem of image recognition, and excellent results of > 99% can be achieved with simple versions of standard architecture.

Of course one will eventually need to ensure generalization to different conditions, mainly various weather conditions, time of day, season. It is not practical to collect training data under all possible conditions, so we need to design a neural network which focuses on the qualities of the route which are invariant under these changes.  >


