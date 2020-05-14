# Important-Selenium-Interview-Questions
Selenium Interview Questions &amp; Answers

What is Automation Testing ?

Automation testing is a way of automating the browser application by performing or executing the test cases. Using automation test, we can perform parallel execution, which we can't do with manual process. Manual process requires more man-power and more efforts to execute the test case. Rather, we can do it using various Automation tools, like Selenium, CodedUI ,QTP, which require less time. Using automation testing, we can execute various scenarios multiple times, but in case of using manual processes or manual testing, there may be chances of leaving such scenarios.The results are more accurate with automation testing and save a lot of time.

Different Automation Testing Tools in IT Industry

Nowadays, everyone prefers various Automation Tools like QTP, CodedUI, Selenium etc. Using these tools, we can get very accurate results compared to that of manual processes. Selenium is open source whereas CodedUI and QTP both are licensed tools. Selenium is easy and fast in execution compared to QTP and CodedUI.

Usage of Automation Testing

Using Selenium or any other Automation Tool, we can perform various tasks, like execution of test cases with accurate results, and navigating through various scenarios and screens multiple times. Executing the test cases on remote machines by launching various browsers remotely reduces the time and effort.

What is Selenium and its components?

Selenium is an open source automation tool which is used to execute the test cases on web applications. Selenium supports various programming languages which include C#.Net , Java , Perl , PHP, Javascript etc. It supports various platforms to perform execution; some of the platforms are Windows , Linux , Mac OS, windows -10(For Edge browser) etc. It supports various browsers to execute the test cases such as Chrome browser , Internet Explorer, Firefox , Safari ,Edge etc.

The various components of Selenium are

Selenium Core
Selenium RC
Selenium IDE
Selenium Grid
Selenium webdriver.
Among these, Selenium core and Selenium RC (Remote Control) are part of Selenium version 1.0. Selenium IDE (Integrated Development Environment ), Grid and webdriver are part of Selenium 2.0. The popular ones in Selenium are Selenium Grid and Selenium webdriver, as most of the top organizations are preferring these in their project development.

Why should I prefer Selenium over other Automation tools ?

As I mentioned in my above answers,Selenium is an open source Automation tool ,whereas CodedUI,QTP or other tools are Licensed Versions. Selenium is very fast in execution compared to other tools. It supports execution on web applications as well as mobile applications like Android, IOS, etc.

What are the advantages of using Selenium ?


You can refer to the above answers.

Using Selenium we can perform parallel execution with the help of hub and node configuration and it also supports execution of the test cases in remote machines which saves time and human effort.

How to find a control or element in Selenium ?

We can have various elements or controls on a page like Textbox,radiobutton, dropdown , Button , Hyperlink etc.

In Selenium after launching the browser we can perform various operations like clicking of a button or selecting dropdown , selecting checkbox or entering the value in a textbox, checking the radio button etc based on our requirements.

For identifying the controls or elements , each element will have a unique property like Id, Name, Classname, Xpath, Tagname, css Selector, partial link text etc.

Code for identifying the control
Iwebdriver driver;  
IwebElement element = driver.Navigate().GoToUrl("http://www.google.com");  
element.findElement(By.Id("Inputname"));  
element.findElement(By.Name("Inputname"));  
element.findElement(By.CssSeletor("Inputname"));  
element.findElement(By.TagName("Inputname"));  
element.findElement(By.Xpath("//Inputname"));  
element.findElement(By.LinText("Inputname"));  
These are a few examples for finding a control based on their unique properties.

Different versions of Selenium 

As I have explained in my earlier questions above, there are three different versions of Selenium. 
Selenium 1.0 was the very starting version of Selenium which was released in 2004 . In this version we have Selenium Core and Selenium RC.

Selenium 2.0 is the second version which was released in July 2011, which consists of Selenium IDE, Selenium Grid and Selenium Webdriver. Most of the companies prefer to work on Selenium Grid and Selenium Web driver. For more information, you can follow the official website(https://seleniumhq.wordpress.com/2011/07/08/selenium-2-0/)

Selenium 3.0 is the latest version which was released in June 2016 and it has the following advantages or features:
Firefox Browser version is supported by 47+. If we want to work with the older versions; i.e., less than 47 version, there is no need to install Gecko driver but working with more than 47+ either in Selenium 2.0 or Selenium 3.0 requires Gecko driver to be installed and configured.

In this version, we also have support for Microsoft’s Edge Browser, which is Microsoft’s own browser.

Following are the prerequisites to work with Edge Browser .

The client machine should be installed with Windows 10 Operating system.

It supports Java greater than 8 version to run Java code (hub).

Support for Safari (Apple OS) Browser is provided by Safari drivers (10.0 version+).

More than 9+ versions of IE are supported in Selenium 3.0.

Now Selenium 3.0 has became a W3C (World Wide Web consortium) standard.

Selenium 3.0 removed Selenium Core but supports Selenium RC indirectly through back-end Webdriver.

For more information you can refer to the Selenium Official website (http://www.seleniumhq.org/about/news.jsp) and you can refer to my previous articles (http://www.c-sharpcorner.com/article/introduction-to-selenium-3-0/).

What is the usage of Xpath in Selenium?

If the control or the element is not identified by its unique properties like id , name , class, tagname etc then in this situation we need to use Xpath. For some element there will be no unique properties or there may be properties with the same name for multiple controls like id=inputname for textbox and button. In this case we need to use xpath for identifying the control.Xpath will be unique for each control. Once we inspect the webpage by clicking on F12 , we can highlight on the element and right click ---> And click on Copy Xpath.

What is absolute & relative path in Selenium ?

In Xpath Absolute path can be created by using single forward Slash like ('/').If we want to take xpath of a control then it takes it from the beginning of the element:

/html/body/table/tr/td[2]

Relative path can be created by using two forward slashes like ('//').If we want to take xpath of a control, relative path starts in the middle from any element.

//table/tr/td[2]

What is the benefit of using Selenium Grid ?

Using Selenium Grid we will be able to execute the test cases in parallel and remotely in another machines by configuring hub and a node.

We can configure single hub and multiple nodes from other machines which are connected in LAN Network.

Hub will act as a Server and distributes the test cases to different nodes which are configured to a particular hub.

What is a webdriver and its types ?

Selenium webdriver is an object oriented tool which consists of various classes and namespaces with which we can perform various actions on the web elements or controls.

To Execute the test cases , each browser has their own drivers to execute.

If we want to execute test case in Chrome, we have a Chrome driver.

If we want to execute test case in Internet Explorer, we have an Internet Explorer driver.

If we want to execute test case in Safari, we have a Safari driver.

If we want to execute test case in Firefox, we have a Gecko driver.(Supported only for version 47+)

If we want to execute test case in Edge, we have an Edge driver.

Selenium even supports execution in mobile applications like IOS/Android drivers which can be downloaded from (http://www.seleniumhq.org/download/).

How to launch a browser in Selenium ?

Using Selenium Automation Tool we can launch the browser in various browsers like Chrome, Firefox, Edge, Safari, Internet Explorer etc. If we want to execute it first we need to download their respective driver from the official website.(http://www.seleniumhq.org/download/) and unzip them and place it in some folder.

Example 1

To launch the browser in Internet Explorer, Chrome and Firefox drivers.
Using OpenQA.Selenium;  
Using openQA.Selenium.FireFox;  
Using openQA.Selenium.Chrome;  
Using openQA.Selenium.IE;  
[TestMethod]  
Public void IELaunch() {  
    Iwebdriver driver = new InternetExplorerDriver("path of the driver");  
    IWebElement element = driver.Navigate().GoToURl("http://www.google.com");  
  
    Iwebdriver driver = new Firefox("path of the driver");  
    IWebElement element = driver.Navigate().GoToURl("http://www.google.com");  
    Iwebdriver driver = new ChromeDriver("path of the driver");  
    IWebElement element = driver.Navigate().GoToURl("http://www.google.com");  
}  
}  
}  
Different operations on an element in Selenium

We can perform various operations or actions to a control like enter the value or clicking the button or double click etc.
IwebDriver driver = new Firefox();  
IwebElement element = driver.Navigate().GoToUrl("http://www.google.com");  
element.FindElement(By.Id("cvcv")).SendKeys("Hello This is Selenium Interview QA"); //for performing sendkeys to a textbox.  
element.FindElement(By.Name("cvcv")).Click();  
element.FindElement(By.ClassName("cvcv")).DoubleClick(); <  
face = "Roboto, sans-serif" >  
What is the difference between findElement() and FindElements() in Selenium?

If we want to find particular element; i.e., a single button or textbox or dropdown or any other control then we find it by FindElement() method like below
IwebDriver driver = new ChromeDriver("path of the driver");  
Iwebelement element = driver.Navigate.gotoUrl("http://www.google.com");  
element.FindElement(by.Xpath("//html/body/input[2]")); // If it single we find using FindElemet()  
List < IwebElement > elements = driver.Navigate().GotoUrl("http://www.google.com");  
elements.FindElements(By.Xpath("//html/body/a")));  
If it is collection then we have to use FindElements()  
What is the difference between Quit() and Close() ?

Both are the methods of a IwebDriver interface.

driver.close() is used when we want to close the particular windows or current window in which we perform the execution of test cases.

driver.quit() is used when we want to close all the browser windows which were launched or opened by the current webdriver.

Which programmings are supported in Selenium?

JAVA, C#, PHP, Perl, JavaScript etc.

What are the platforms supported in Selenium ?

Windows(including Windows-10 for Edge browser), Linux , MacOS etc.

What is Assertion and different types of Assertions are used in Selenium ?

Assertion is used to verify or to check whether the given value is present on the webpage or not , we have various type of Assertions like
Assert Text
Assert text is used to Assert the value Available in the textbox.

AssertElementPresent
Assert Elementpresent is used to verify whether element is displayed on the webpage or hidden state.

AssertBodyText
It is used to verify whether the given input exists on the webpage.

AssertId
It is used to verify / Assert the id of an element.

Assert Title
It is used to verify the title of the webpage.
What is a hub and node ?

As we discussed earlier, Hub acts as a Server or middle point. We can configure multiple nodes to a hub. Hub distributes the test cases we want to execute on various nodes.


What is jar file and how do we configure hub and node?

Jar file is a Java Execute file which is used for creating the hub .

The following is the process for configuring hub and Node.

Before configuring hub, we need to have Java runtime installed in our machine. Without Java runtime, we cannot configure the hub.

Once Java runtime is installed into your machine, you can download the Jar file from the official website.

Java -jar "Name of the jar file" - role hub , this command will configure hub.

Java - jar "name of the jar file" -role hub - node http://192.168.1.1:4444 -bowser:browsername="chrome" Version=ANY -DwebDriver.chrome.driver="path of the chrome driver"

The above command will configure the node.

Different types of exceptions thrown in Selenium

NoSuchElementException
StaleElementReferenceException
ElementNotVisibleException
TimeoutException
ElementNotSelectableException

For more Exceptions in selenium you can go here.

How do we perform sample unit tests in Selenium ?
 

Using openQA.Selenium;  
[TestMethod]  
public void LaunchBrowser() {  
    IwebDriver driver = new FirefoxDriver / ChromeDriver / IEExplorerDriver("path of the driver file");  
    IwebElement element = driver.Navigate().GotoUrl("http://www.google.com");  
    element.FindElement(By.Id("input"));  
    element.click();  
}  
To execute the above unit test, right click on the above method, launch browser, and either you can debug the test or Run.

What is the latest version of Selenium and what are its features ?

Selenium 3.0 is the latest version available in the market which was released in June 2016. Please refer to my previous article which is on Selenium 3.0.

What are the parameters or arguments in Selenium ?
Host
Host is the IP address of the node/client machine where we want to execute the test case.

Port Number
The default port number is 4444 , if we don't assign any port number it takes by default 4444 or we can set other port numbers like 5555 , 5556 etc.

Browser
It defines where we need to execute the test case on which browser (example Chrome ,Firefox , IE , edge ) etc.

URL
It defines the URL of the webpage.
How to specify wait time for a control?

WebDriver driver = new FirefoxDriver();  
driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);  
[OR]  
Thread.sleep(2000 seconds);  
Does Selenium support testing on mobile-based applications?

Selenium supports mobile application testing, like iOS , Android etc.

Can we handle Windows based pop-ups using Selenium ?

Yes, Selenium supports both Windows and Web pop-ups.

driver.switchTo().alert();

What is the use of the GetAttribute() method in Selenium?

If we want to access the properties of a control or element such as id, name , class , Tagname etc, we use GetAttribute() method.
element.getAttribute("id")  
element.getattribute("class")  
How to click on Login button using selenium ?

webelement.click() or webelement.submit()

How to maximize window in Selenium ?

After launching the browser, if we want to maximize the page we use the below code.

driver.manage().window().maximize();

By default IE and Firefox are maximized, but for Chrome, we need to maximize that using the above code.
 
 You can enhance your knowledge more, by reading the following articles.
 
How To Select A Test Automation Tool 
The Postman Always Tests Your Web APIs, Twice
Introduction To Selenium 3.0
Software Testing: The Essential Guide To Bug Reports
Top 10 Website Security Testing Tools
Top 10 Website Functional/Regression Testing Tools
Software Testing: Software Verification & Validation
Creating Script Using Selenium WebDriver
Basics of Automation Testing
Best Practices of Software Testing
