# junit-tag-surefire-problem

The Native maven surefire plugin doesn't recognize the excludeTags/includeTags. This project should only execute a single test, but executes all three. 

Correct behavior would be:
* executing a single test if nothing is commented out
* executing two tests in "includeTags" is commented out
* executing a single test if "excludeTags" is commented out.
* executing three tests if both "includeTags" and "excludeTags" is commented out
