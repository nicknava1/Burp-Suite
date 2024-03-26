<h1>Burp Suite - Vulnerability Scan</h1>

<h2>Project Description</h2>
<p> <b>Burp Suite</b> is a powerful web application vulnerability scanner created by PortSwigger. In this project, I'm going to show you how to use this tool to identify common website vulnerabilities. The crawl function is used to map the website by navigating the website like a real user. Then, the audit function will identify exposures and other issues. Let's get started. </p>

<h2>Tools/Websites used</h2>

- <b>Burp Suite Professional</b>

- <b>[ginandjuice.shop](https://ginandjuice.shop/)</b>

- <b>Windows 10</b>

- <b>MITRE CWE</b>

<h2>Creating a new project</h2>
<p>First, we will begin by opening Burp Suite and creating a new project. Select new project on disk and enter a name for the project. For the purposes of this tutorial, I will be naming it Test Scan.</p>

![Step 1](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/1.png)

<p>From here, you will be asked to select the configuration you would like to load for this project. Let's use the Burp default option and click Start Burp on the bottom right of the window.</p>

![Step 2](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/2.png)

<p>Now you should see the Burp Suite dashboard. This is where the magic happens. Right now, we are going to focus on the upper left corner. You should see a button that says new scan, which I have highlighted yellow in the accompanying image. Let's go ahead and click      that so that we can move onto the next sextion of this tutorial.</p>

![Step 3](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/3.png)
  
<h2>Configuring your first scan</h2>
<p>Now there should be a new window called "New scan". You should be on the first left-hand tab called scan details. For this scan we are going to perform both a crawl and audit, so make sure it is selected. In the next field we will designate the target url we want to perform our vunlnerability scan on. We will be using the website https://ginandjuice.shop/.</p>

<p><b>Note: It is important to have permission from the website owner before performing a scan like this. "ginandjuice.shop" is provided by PortSwigger for testing purposes.</b></p>

![Step 4](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/4.png)

<p>Next, select the scan configuration tab on the left side of the window. On this screen we are given options for different types of scans we can perform. For this test, we want to get a top-level summary of the targeted website in a short amount of time. The best option for this is the Lightweight preset scan mode. Make sure the lightweight scan is selected then click OK to begin your scan.</p>

![Step 5](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/5.png)

<p>Your scan should now be underway, and in the mean time you should get yourself a cup of coffee. You earned it! While there are still more options for customization available, they are beyond the scope of this demonstration. The application login tab would allow you to establish a credentialed vs non-credentialed scan. This could be useful for identifying vulnerabilities to potential insider threats like disgruntled employees.</p>

<h2>Analyzing Results</h2>
<p>It's fifteen minutes later, so now our scan is complete. Let's take a look at the results. Wow, look at these serious vulnerabilities that our scan has uncovered! You can see them under the Summary tab. They are ordered here from top to bottom by most severe to least severe.</p>

![Step 6](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/6.png)

<p>Let's go ahead and inspect one of these vulnerabilities further. Click the first one on the list, which should be a Cross-Site Scripting vulnerability.</p>

![Step 7](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/7.png)

<p>Here you can see details about the issue. This screen even explains how it discovered the exposure point, including the payload it used to take advantage of the vulnerability. Remember, this tool should only be used for ethical purposes on websites you have permission to test on!</p>

<p>If you were performing this scan for a real company, it would be critical to analyze each vulnerability and create a remediation plan to make this website safe for its customers. Thankfully, the Burp Suite scanner includes valuable information like the relevant CWE associated with each detection. You can find more information about this from MITRE at https://cwe.mitre.org/. Thank you for joining me on this project, and I hope you learned something about vulnerability scanning! </p>
