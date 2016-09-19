# Selenium
To get the Selenium package to work there are a few things you need to do first:
-	1) Download java JDK downloaded --  This is different than the run-time environment used for simple surfing of the web. http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.htmlFollow the step-by-step instructions
-	2) Down load the the WebDriver extension for safari @ http://www.seleniumhq.org/download/   It was under SafariDriver section; version I downloaded was 2.48.0When you double click on the downloaded file.If all is right it should have brought up the Extension section of Safari's preference menu option.
-	3) Next download Selenium Standalone server from same webpage  http://www.seleniumhq.org/download/Some on the web helpsites suggested you need to do this because of Mac's security settings. Download the file under the Selenium Standalone Server section
-	4) When downloaded I had a selenium-server-standalone-3.0.0-beta3.jar  in my download directory.  Put that file in R's working directory.
-	5) Next open Terminal (you'll find that in your LaunchPad under Other)I navigated to my R working directory using cd and ls commands
-	6) One in the working directory type:java -jar  selenium-server-standalone-3.0.0-beta3.jar
-	7) Everything should be ready for you to execute your code:
**	library(RSelenium)
*
*	RSelenium::checkForServer()
*	remDr = remoteDriver(browserName = "safari")
*	remDr$open()
* ...
