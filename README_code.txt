Most of the code is taken from here:
http://modelai.gettysburg.edu/2013/tdgammon/index.html
http://modelai.gettysburg.edu/2013/tdgammon/pa2.pdf
http://modelai.gettysburg.edu/2013/tdgammon/pa4.pdf

But the following classes have been added:
To package player - BackPropPlayer2,Utility
To package driver - SimulationDriver,TestStrengthDriver

BackPropPlayer: A NN player, that implements TD learning, takes parameters Lambda(TD-lambda), Alpha(NN learning-rate), trainingmode(true/false)
Utility: Implements primarily "BoardtoVec" to change a board to a NN representation
SimulationDriver: To run simulations
TestStrengthDriver: To test any two players against each other (the first one is always black)

Useful things to know:
1. SavedNN is a trained NN, the one provided with the code was generated after 1000000 games
of selfplay (specified in the while loop of SimulationDriver) and took 886 minutes to train on a very fast laptop
2. NeuralNetworkVisualizer class can be used to visualize the Neural Nets thus generated


In other repertory :

You find our SavedNN with different number of training games (k) : 1000, 10.000, 100.000, 300.000, 1000.000
If you don't have a powerfull machine to reproduce the results, just use these files. 
You can use them to get the figure and table showed in the report


