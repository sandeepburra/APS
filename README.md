The system in focus is the Air Pressure system (APS) which generates pressurized air that are utilized in various functions in a truck,
such as braking and gear changes. The datasets positive class corresponds to component failures for a specific component of the
APS system. The negative class corresponds to trucks with failures for components not related to the APS system.
The prbolem is to reduce the cost due to unecessary repairs. So it is required to minimize the false predictions.


Predicted class | True class | | pos | neg |
pos | | cost_1 |
neg | cost_2 | |
Cost_1 = 10 and cost_2 = 500


The total cost of a prediction model the sum of "Cost_1" multiplied by the number of Instances with type 1 failure and "Cost_2" with
the number of instances with type 2 failure, resulting in a "Total_cost". In this case Cost_1 refers to the cost that an unnessecary
check needs to be done by an mechanic at an workshop, while Cost_2 refer to the cost of missing a faulty truck, which may cause a
breakdown. Total_cost = Cost_1 * No_Instances + Cost_2 * No_Instances
