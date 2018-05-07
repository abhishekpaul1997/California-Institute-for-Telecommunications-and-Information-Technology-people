# California-Institute-for-Telecommunications-and-Information-Technology-people

1. Title: CalIt2 building people counts         GMYMN8705


2. Creator and Maintainer:
	     Jon Hutchins
             UCI
	     johutchi@uci.edu
   Donor: CalIt2
   Date:  December, 2006


3. Past Usage.
   Reference: "Adaptive event detection with time-varying Poisson processes"
	   A. Ihler, J. Hutchins, and P. Smyth
	   Proceedings of the 12th ACM SIGKDD Conference (KDD-06), August 2006.


   Predicted Attribute: Presence of an event such as a conference in the building 
	that is reflected by unusually high people counts for that day/time period. 


4. Number of Observations:  10080.  2 data streams (people flow in and out of the building), 
	15 weeks, 48 time slices per day (half hour count aggregates).  
	file: CalIt2.data


5. Validation data (Number of known events during this time period): 30
	Note: this is an incomplete set, other unscheduled events likely occured
        file: CalIt2.events

	     
6. CalIt2.data file format:
 (column)
  1.  Flow ID: 7 is out flow, 9 is in flow
  2.  Date: MM/DD/YY
  3.  Time: HH:MM:SS
  4.  Count: Number of counts reported for the previous half hour
  Rows: Each half hour time slice is represented by 2 rows: one row for
  the out flow during that time period (ID=7) and one row for the in flow 
  during that time period (ID=9)

7. CalIt2.events format:
 (column)
  1.  Date: MM/DD/YY
  2.  Begin event time: HH:MM:SS (military) 
  3.  End event time: HH:MM:SS (military)
  4.  Event name (anonymized)

8. Missing Attribute Values: None.

9. Other information:  This data comes from the main door of the CalIt2 building
   at UCI.  There are seven other entrances to the building, but the main door 
   gets approximately half of the traffic. 
