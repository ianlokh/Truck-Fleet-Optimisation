### Cheaper & Greener - Transportation Multi-Objective Optimisation

I will be sharing how we approached a "real world like" problem of optimising a fleet of mixed sized trucks for a supplier of automotive parts delivering into manufacturing assembly lines. The actual supplier and assembly line locations were masked but the volumes are scaled based on the actual volume received.

Because the tool we used for this exercise is a trial software, hence there were limitations to the size and complexity of the problem we could model. So to simplify the problem, the following assumptions were taken:

* There are 4 (01 Ð 04) assembly lines the supplier needs to deliver the parts to
* The supplier has a fleet of 3 different trucks types which they used to transport the auto parts to each of the four assembly lines. The parts can be loaded into a 5 Tonne (5T), 8 Tonne (8T) and 10 Tonne (10T) truck type based on the volume of the truck.
* Each truck has a different rental cost and once a truck is used, regardless of the number of orders on the truck, the cost of the truck is expensed.
* The cost of the truck would include driver hourly rate and fuel surcharge by distance per delivery trip.
* The distance and time matrix between the supplier and the plant is given
* Dimensional modelling was not considered and only pure volume was used
* The supplier is looking at optimising the use of their fleet of trucks to meet the contracted demand of the car manufacturer to each assembly line. In addition, the supplierÕs customer has a commitment to ensure CO2 is minimised because of the environmental policy of the customer.

Hence the objectives are to minimise the cost of the truck and trip assignments as well as to minimise the CO2 emission. The key decision variables to this problem is:

* The optimal no. of trucks of each type (e.g. 2 x 5T)
* The optimal no. of trips each of the trucks need to make (e.g. 2 x 5T trucks with 3 trips each, resulting in 6 deliveries using 5T trucks)

And the result needs to consider the least no. of trucks and the lowest CO2 emission as a result of delivering all the orders.

### Pre-Requisites

* Download and install Lingo from [Lindo Systems](http://www.lindo.com) - you need to download the Windows version to be able to use OLE to link to the Excel spreadsheet to read the data tables
