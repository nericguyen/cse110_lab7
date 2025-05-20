Eric Nguyen.

1) Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.

Answer: "Within a Github action that runs whenever code is pushed."  We want automated tests to run whenever a certain event occurs to test both pre-existing code and newly developed code.  If we are automating tests that validate code, it logically follows that the event we would want to track is whenever we push new code.  Thus, we would run the tests within a Github action that runs when code is pushed.  Not to sound redundant, but again, code is usually pushed when new code is written.

2) Would you use an end to end test to check if a function is returning the correct output? (yes/no)

Answer: Probably not...? End to end tests are for user actions, and user actions aren't usually tied to specific functions.

3) What is the difference between navigation and snapshot mode?

Answer: The difference between navigation and snapshot mode is the time in which the page is analyzed.  According to what was in the write up, navigation mode analyzes a page on start up and snapshot mode analyzes a page in its current state.

4) Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.

Answer: One, the user experience is not optimized for mobile screen sizes because it does not have a <meta name="viewport"> tag with width or initial-scale.  Two, the <html> element does not have a [lang] attribute, so the screen reader assumes that the page is in the default language that the user chose when setting up the screen reader. If the page isn't actually in the default language, then the screen reader might not announce the page's text correctly.  Three, the images are not properly sized and is missing out on saving hundreds of KiB.  Lighthouse says that image formats like WebP and AVIF provide better compression than PNG or JPEG, which means faster downloads and less data consumption.