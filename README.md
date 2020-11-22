                                                   Breakout-A3C
A3C : Asynchronous Advantage Actor-critic

• Asynchronous: There are several agents, each one having their own copy of the environment, and all
asynchronised (playing the game at different times).

• Advantage: The advantage is the difference between the prediction of the actor, Q(s, a), and the
prediction of the critic, V (s):
A = Q(s, a) − V (s) 

• Actor-Critic: Of course we can see the actor and the critic, that therefore generate two different
losses: the policy loss and the value loss. The policy loss is the loss related to the predictions of
the actor. The value loss is the loss related to the predictions of the critic. Over many epochs of
the training, these two losses will be backpropagated into the neural network, then reduced with an
optimizer through stochastic gradient descent.

    Repository contains the test folder which has video samples of how AI try to make Breakout Game work by reinforcement learning.
