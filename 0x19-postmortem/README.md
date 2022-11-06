<img src=./image.jpeg width=50%>

# Wajakoya Inc requests failure report
Last week, it was reported that our platform was returning 402 Error on all requests made on the platform routes, all the services were down.  Nearly all of the users were affected. The root cause was due to an overload on our servers due to an influx on users due to the release of a new feature. 

## Timeline
The error was realized on Saturday 20th March 04:20 pm (East Africa Time) when our Backend Engineer, saw the master server receiving several requests. There was an emergency meeting called for clearance from several departments to purchase and manage the influx of use and solve the inaccessibility of the site. The problem was solved by Sunday 20th March 2004 hours (East Africa Time).

## Root cause and resolution
The root cause was due to the site not having sufficient resources to handle the increase of several requests from several users. We had not anticipate to get such a huge response to the new feature that had clients logging in at the same time to access our site.


The issue was fixed when we increased the number of servers temporarily to enable the requests be managed properly. After to check the user number gradually and make the necessary servers to manage the requests.

## Measures against such problem in future
- A team to be always on hold during a feature release.
- Always keep an eye on number of users during feature release to ensure current servers available don't get highly stressed.
- Have back-up servers to prevent your program from completely going offline during an issue
