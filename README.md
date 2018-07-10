# junit-tag-surefire-problem

The native maven surefire plugin doesn't recognize the excludeTags/includeTags properties. This project should only execute a single test by default, but currently executes all three. 

Correct behavior would be:
* executing a single test if nothing is commented out
* executing two tests if "includeTags" is commented out
* executing a single test if "excludeTags" is commented out
* executing three tests if both "includeTags" and "excludeTags" is commented out
