# mercury-lunar-mapper
Mapping the element composition of Mercury and the albedo of the Moon with machine learning applied to Messenger and Lunar Orbiter datasets. Based on the ML4Sci MLMAPPER project proposal.

For the Moon, a multi-input nonlinear regression neural network is coded using Tensorflow/Keras, taking in several element datasets and creating a regression model for lunar albedo. This model is then tested on the element data for the left side of the Moon, to plot the albedo of the right side. The model is evaluated to find its accuracy.

Similarly, for the Mercury program, a multi-output nonlinear regression neural network is used to predict the chemical composition of the bottom half of the planet, from the albedo data of the top half. As there are gaps in the Messenger chemical/albedo data for the top half, further neural networks are used to fill in the gaps, with this "filled in" data put into the bottom half prediction neural network.

Written in: Python
