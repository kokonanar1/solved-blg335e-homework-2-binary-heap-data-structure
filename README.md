Download Link: https://assignmentchef.com/product/solved-blg335e-homework-2-binary-heap-data-structure
<br>
Part 1. Implementation

In this homework, you are expected to build a priority queue (PQ) for a taxi application simulation using the binary heap data structure. In the simulation scenario, a hotel desk clerk uses an application to see available taxis in the city with their distance to the hotel location. When a customer is leaving the hotel, the hotel desk clerk calls the nearest taxi for the customer. Your implementation should simulate the taxi application, i.e., showing the nearest taxis to the hotel using the provided coordinates of taxis.

You are given a dataset named “locations.txt”. In the dataset, the locations of the taxis are provided as longitude and latitude. You will use the longitude and latitude information of a taxi to calculate its distance to the hotel by using the Euclidian distance. The location of the hotel is 33.40819 (longitude) and 39.19001 (latitude).

You need to implement a PQ using binary heap data structure that supports the following operations (30 points):

<ul>

 <li>A new taxi can become available in the city (in other words, a new distance can be added to the heap)</li>

 <li>Some taxis’ distances to the hotel location can be updated (only decrease is allowed for this simulation)</li>

 <li>The hotel desk clerk may call the current nearest taxi (its information should be removed from the heap)</li>

</ul>

You need to develop a simulation for the taxi application with the following features (20 points):

<ul>

 <li>The closest taxi to the hotel location will be removed after every <strong>100</strong></li>

 <li>Each operation is an update with a probability of <strong>p</strong> or an addition of a new taxi with a probability of <strong>1 – p</strong>.

  <ul>

   <li>If an operation is an update, a random taxi’s distance value will be decreased by <strong>0,01</strong>.</li>

   <li>If an is an addition, new information will be read from the provided file, and the distance value of the new taxi will be added to the PQ.</li>

  </ul></li>

 <li>Simulation stops after <strong>m</strong> operations (new taxi addition, updating taxi distance, or calling nearest taxi).</li>

</ul>

Your program should run from the command line with the following format:

./a.out m p

The output must contain the following:

<ul>

 <li>The distance of the called taxis</li>

 <li>The number of taxi additions and distance updates</li>

 <li>Total running time in milliseconds</li>

</ul>

<h1>Part 2. Report</h1>

<ol>

 <li>Please explain your implementation on the PQ operations and the simulation features with their theoretical running times. It is better you support your explanations with comments on your source code file.</li>

 <li> Demonstrate (using a graph or a table) of the effect of the <strong>m</strong> choice on the running time. You should run the simulation for different values of <strong>m</strong> between 1000 and 100000 for a constant p (0.2). Also, discuss the demonstration by answering following questions: Is the graph as what you have expected? Does it match to the theoretical running times?</li>

 <li> Demonstrate (using a graph or a table) the effect of the <strong>p</strong> choice on the running time. You should run the simulation for different values of p {0.1, 0.2, …, 0.9} for a constant <strong>m</strong> (you should choose an appropriate value for <strong>m</strong>). Also, discuss the demonstration by answering following questions: Is the running time affected by <strong>p</strong>?</li>

</ol>

Why do you think it is affected or not effected?