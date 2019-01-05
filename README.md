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
      1) a trip end O-D matrix
      2) a comparison of traffic volume and transport capacity
      3) financial cost, revenue and income.


## instances of input scenarios and corresponding output
![scenario 01](https://user-images.githubusercontent.com/46351057/50719570-1226ef80-10d9-11e9-8a9f-a95c40b06f00.jpg)
![scenario 02](https://user-images.githubusercontent.com/46351057/50719571-16eba380-10d9-11e9-8d36-19309103fd55.jpg)
![scenario 03](https://user-images.githubusercontent.com/46351057/50719573-19e69400-10d9-11e9-9c7d-b31f1bfc6c98.jpg)
![scenario 04](https://user-images.githubusercontent.com/46351057/50695640-36061900-1078-11e9-8710-de0d4a9cc896.jpg)
