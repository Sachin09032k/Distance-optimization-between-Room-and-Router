# Distance-optimization-between-Room-and-Router
A Digital Circuit is designed which generates the locations of the Room Router pair having minimum distance between them when an array of locations of room and router is provided.

In case of multiple room router pairs having minimum distance, the room should be selected such that its location from the reference point is minimum. 

The circuit contains a ROM (Read Only Memory) which is fed by a binary file containing sixteen 7-bit binary numbers out of which twelve numbers are the locations (distance from reference point) of the hostel rooms whose MSB is 1 and the rest four numbers are the locations of routers whose MSB is 0. 

### Note:
Only 6 bits are the location and rest 1 bit(MSB) is flag bit to differentiate between room and router. 

## Approach

The circuit is designed using Proteus EDA Software and 7400 ICs.
- The list is iterated to find the locaton of Router using a clock,counter and ROM. 
- The current address of the location of Router is stored in a register.
- Next, the list is iterated again and distance is calculated between the router and all the rooms and compared.
- Every time, when it gets a minmum distance or a distance equal to minimum and a room having less distance from refernce point, the location of Room and Router is updated.
- Again the list is iterated to find the location of router and its address is compared with the previously stored address so that we get the next router.
- And the cycle continues until all the routers are compared with all the rooms.
- The required loactions of Room and Router are dispalyed using 7 Segment Display.


#### P.S.

 A python file stores the list of locations and it creates a bin file when run. The Rom must be attached with the bin file.
 Both files are uploaded in the repository for reference.




