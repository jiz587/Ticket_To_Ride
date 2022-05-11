# Ticket_To_Ride

This project is for Assignment 4 IS545. I have constructred a map with the cities in the game "Ticket-To-Ride". When each player places their train on route, the route
and points would be added to data. All graphs would display  with four colors where each color represents a player. The lines on the map shows which route the players
claimed. The bar graph shows the current score board of the gamestate, and the line chart shows the progression of the points by rounds.


## Advantages and Shortcomings of the current design
The biggest advantage of this design is having a map representation. Having a map representation of the routes claimed by each user is very clear for the audience to see the current game state. It makes the current design more interesting to view as well. The bar graph shows the current points of each player, which is also very clear for the audience to see the points summary. The line graph shows the change of points for each round which gives a history of the points progression.

Some disadvantages of the current design is I don't have the length of the route represented anywhere on the visualization. I initially wanted to add the length of each route on the map, but I wan't able to achieve this. Another disadvantage is the color code. The colors on the all graphs were chosen by vega-lite. Even though the colors are matched across all visualizations, this choice of color doesn't match the true train color in the game. This might confuse the audience

## Responsivity and interactivity
Unfortunately I wan't able to create any interactive features becuase debugging the line path on the map took to much time.  If I were to create any interactive features, I would create a text table with a drop down menu, listing the specific action of each round, where the users could select which round they would like to see. In this table, I could also show the route length in this table.

## What would I try differently next time
Like I mentioned in the previous section, I would definitely add more interactive features like showing the detail info for each round. I would also try to color code according to the train color of the true gamestate instead of having vega-lite assign the colors. I would also want to add "insert data" feature(adding the data in runtime). However, I know this cannot be easily accomplished in vega-lite. Therefore I would probably try a different platform next time just for this feature. I think this feature is rather important becuase we would want to record the game as we go

## Experience of building visualization feedback into prototyping phase
I think the hardest part of this experience is to decide which part of game we want to save and which part we would drop. It is always hard to drop some information such as which cards are open to draw, which cards do each players have, what are the two target routes of each player(the routes to gain extra points), how many cards are open to draw, and many more. The second part is choosing the right platform. I wanted to set up a map, therefore I chose vega-lite because the map features seem simple to implement. After the platform is decided, other design choices need to be decided as well. For example, I debated whether to use a horizontal bar graph or a vertical bar graph for the current points. After this experience, I am much more familiar with prototyping and I think I would do better next time.
