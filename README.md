# the best metro route scenario
## Objective:
      to find the best metro route scenario which is
            the most profitable for a metro company 
            and satisfies the travel demand of consumers. 
      (by using the Four-Step Travel Demand Model and Dijkstra algorithm)
      
## Topic:
      Development of an application (in Python) for educational purposes where students can define Public Transport systems in a schematic situation in order to optimize the service (in terms of travel time for the passengers, passenger trips, exploitation costs, etc.).

## Inputs:
      1) the location of metro stations
      2) the lines that connect stations
      3) the frequency of vehicles
      4) capacity of vehicles

## case data:
The application is based on a certain defined case. In this case, an area is divided into a 5 rows*5 columns grid network. Each grid cell is a zone. The total number of zones is 25. It can be seen in the picture below. 
      ![casegrid](https://user-images.githubusercontent.com/46351057/50719932-e575d680-10de-11e9-885b-8a1421423111.jpg)
1) Social Economic Factors: These data are used for calculating trip generation. It contains number of inhabitants in a zone, number of jobs in a zone, average income of the inhabitants in a zone, average car ownership of inhabitants in a zone, average household structure of in habitants in a zone, average family size of in habitants in a zone 
      ![1](https://user-images.githubusercontent.com/46351057/50719928-e444a980-10de-11e9-94e7-5c85a58e6886.png)
2) Coefficients of Social Economic Factors: These data are used for calculating trip generation.
      ![2](https://user-images.githubusercontent.com/46351057/50719929-e4dd4000-10de-11e9-8aba-c8c7be118c3f.PNG)
3) Impedance Calculation Factors: There data are used for calculating impedance from a zone to another zone. 
      ![3](https://user-images.githubusercontent.com/46351057/50719930-e4dd4000-10de-11e9-9bb9-3411baf4c16f.png)
4) Budget Data: These data are used for calculating financial cost, revenue and income. 
      ![4](https://user-images.githubusercontent.com/46351057/50719931-e575d680-10de-11e9-86f4-130189f9e7eb.png)

      
## Methodology: 
      The theory underneath the application is the Four-Step Travel Demand Model which contains: 
      1) trip generation
      2) trip distribution
      3) mode choice: Dijkstra algorithm is applied
      4) traffic assignment
      
## Outputs:
1) a trip end Origin-Destination matrix
      
      ![output1](https://user-images.githubusercontent.com/46351057/50720093-97ae9d80-10e1-11e9-9eb6-78ad0ddf32b5.png)
      
2) a comparison of traffic volume and transport capacity
      This is a result of traffic assignment. It has two purposes. The first purpose is to show that how many trips go from each metro station to another metro station. This is called traffic volume. It can be seen in the pink part of the table below. It clearly presents which edges of which line has more than traffic volume than the other edges. So the user can make some improvement if needed. The second purpose is to show whether or not the transport capacity is able to bear the traffic volume. If the calculation result is a positive number which means the transport capacity is large enough, then the result shows “Succeed”. Otherwise, the result shows “Fail”. The calculation and result can be seen in the blue part of the table below. 
      ![output2](https://user-images.githubusercontent.com/46351057/50720094-97ae9d80-10e1-11e9-93dd-5c74b05c6080.png)
      
3) financial cost, revenue and income
      ![output3](https://user-images.githubusercontent.com/46351057/50720095-98473400-10e1-11e9-845b-05a35f69a6cb.png)
      Financial cost contains two parts: establishment cost and operation cost
      Establishment cost of the whole metro system (euros) = Station build-up cost + Road build-up cost + Vehicle purchasing cost
      Operation cost of a line (euros/day) = Station maintenance cost + Road maintenance cost + Vehicle maintenance Cost + Labor cost 
      Revenue of a line (euros/day) = sum of (price per unit of distance * distance of an edge * traffic volume of an edge)
      Income of a line (euros/day) = Revenue- Operation cost. The establishment cost is not taken into account when calculating income because establishment cost is not related to time. 

## instances of input scenarios and corresponding output
![scenario 01](https://user-images.githubusercontent.com/46351057/50719570-1226ef80-10d9-11e9-8a9f-a95c40b06f00.jpg)
![scenario 02](https://user-images.githubusercontent.com/46351057/50719571-16eba380-10d9-11e9-8d36-19309103fd55.jpg)
![scenario 03](https://user-images.githubusercontent.com/46351057/50719573-19e69400-10d9-11e9-9c7d-b31f1bfc6c98.jpg)
![scenario 04](https://user-images.githubusercontent.com/46351057/50695640-36061900-1078-11e9-8710-de0d4a9cc896.jpg)
