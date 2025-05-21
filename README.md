Victoria Timofeev

1) Where would you fit your automated tests in your Recipe project development pipeline? 
Within a Github action that runs whenever code is pushed. This is because the tests run automatically whenever a change is pushed. You do not have to worry about manually running them, which is easy to forget and wastes a lot of time. You also do not want to run them after development is complete so that you can catch bugs early. 

2) Would you use an end to end test to check if a function is returning the correct output? (yes/no)
No. End-to-end tests automate test cases with user actions from start to finish. As a result, it does not test functions but complete user workflows. Unit tests are better for testing functions.

3) What is the difference between navigation and snapshot mode?
Navigation mode tests a page load from the start, useful for understanding the performance of a page when it is first accessed by a user. Snapshot mode, on the other hand, analyzes the page in the current state without reloading. It tests the page after human interactions with the page, like filled in forms for example. It does not measure load performance however.

4) Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.
- Improve accessibility by adding a `[lang]` attribute to the `<html\` element. A screen reader may not announce the text of the page correctly since it will assume that the page is in the default language the user has set up. 
- Add meta description. Adding a `<meta name="viewport">` tag with width or initial-scale optimizes the site for mobile screen sizes. Lighthouse also mentioned that it prevents a 300 millisecond delay to user input.
- Properly size images since they are larger than necessary and can slow load time. Potentially save 718 KiB. 