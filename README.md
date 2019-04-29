## Project to predict initally the results of upcomming bouldering or lead competitions, and eventually the OL 2020 climbing results

I enjoy climbing in my spare time, and in the upcomming Olympic Games, climbing will be introduced as a new disciplin. 
The rules of the scoring is a little different from what I would have expected. 

The format of the games are explain [here](https://www.youtube.com/watch?v=aLKavMRf0do) bu athlete 
Adam Ondra.

Basically, 20 men and 20 women will compete, and the format consist of three disciplines:
* Lead Climbing
* Speed Climbing
* Bouldering

How the climbers will be chosen is described [here](https://www.climbing.com/competition/how-climbers-will-be-chosen-for-the-2020-olympics/) - but to sum up:

Of these 20 men/women (maximum of 2 of the same gender pr. country), the selection is as follows:
* one will be from Japan (the host country)
* one will be selected by the Tripartite Commission. 
* seven  invitations to the OL will be given at the IFSC Combined World Championships on August 20-21, 2019, in Hachioji (Tokyo). If for example there are 5 American women among the top 7, only the 2 with the best results will be invited - the "unused" invitations will be given to representatives further down the ranks. 
* 6 spots will be occupied after the Olympic Qualifying Event on November 28-December 1, 2019, in Toulouse
* the remaining 5 will be divvied accrose five separate Continental Championships in spring 2020. **The last competition is in Japan on May 18th-24th 2020**. 

### The Challenge - part 1
Since the athletes that will participate in the OL games have not yet been qualified, prediction of the main event is still dificult. 
Instead, my plan is to initially predict the results of upcoming bouldering, lead or speed climbing competitions based on the results from previous competitions. 

### The Challenge - part 2
Once all athletes have been chosen (May 24th 2020), based on the learning done for the individual competitions, I will try and predict the result of each athelete for each disciplin - as a classification of position 1-20, and based on these three predicted results, find the totalt score and predict a total winner for men and women. 


#### Initial Thoughts
I will try to focus first on a single disciplin, bouldering, since this is the discipline where I already have the best understanding of the scoring system.
The results of multiple bouldering competitions can be found on the [International Federation of Sport Climbing Homepage](https://www.ifsc-climbing.org/), using the calendar results from previous years (prior to 2018) can also be found. 

#### Work Flow
* Collect data from 2015-today of all men and women bouldering competitions - should there be some sort of penalty for older data?
* Use pandas to clean the data - maybe some synthetic features taking into account the age of the athlete etc.?
* Use tenforflow + keras to construct a neural network to predictic the results of a future set of bouldering competitions
