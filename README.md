# MSE-2202-Lab-5-
Code for Lab 5, exercise 1, 2 and 3

Exercise 1:
In my exercise 1 video, the robot hits the beacon but then slightly slips past it as it is coasting to a stop. Since I did this exercise early into reading week, I used a time-based approach which correlated the encoder distance to a travel time. The travel time was multiplied by a "distanceCorrection" factor which was used to ensure that the time did not prematurely stop the robot before the encoder distance was reached. I found most of my troubles in getting the robot to consistently drive straight. In order to get it to go as straight as possible, I adjusted the left wheel speed per case and used a guess-and-check method until the speeds were aligned and allowed the robot to go straight. 

Exercise 2:
My exercise 2 was ultimately unsuccessful in reaching the ultimate goal as the robot just missed the beacon, to the right. However, it still reversed back, did a 180 degree turn and raised a flag. I also used a time-based approach for this exercise with the distance-correction term. While doing this exercise I encountered the largest problem that my robot had; the wheels did not reset to the correct position after each turn. For example, after a 90 degree turn, the right wheel would need to slip a certain before the bot actually starts moving. This amount of requried slip was different for the left wheel. To solve this issue, I'd have to overrotate the wheels past 90 degrees to accomodate for this difference in slip. When over-rotating the bot, it would straighten out once it started moving.

Exercise 3:
Exercise 3 was definetly my favourite to program, although it may be the most tedious. I changed to an encoder distance approach where the bot would stop only when the encoder distance was reached. This played out much more favourable for me. As for the localization of the beacon, I had the bot doing ~10 degree rotations until the IR signal was sensed by the TSOP. Once sensed, it would do one more rotation, then make a quick dash towards the beacon. If the dash did not make the bot touch the beacon exactly, I had the bot do 1 tick increments until the limit switch was hit and the new character was displayed. Once the new signal is received the led turns purple, and the bot does the reverse-180 turn-raise flag sequence.

Overall, this lab was not so much challenging but just tedious due to the limitations of our parts. I do believe it was a good learning experience though.
