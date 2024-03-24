<h1>Scanning for website vulnerabilities using Burp Suite</h1>

<h2>Introduction</h2>
  <p>Burp Suite is a powerful vulnerability scanner created by PortSwigger. In this project, I'm going to show you how to use this tool to identify a spectrum of vulnerabilities by performing a crawl and audit of a target website. Then, we'll analyze the results together     and explore the different issues discovered during the audit. Finally, I'll show you how to create a report in Burp Suite and present a remediation strategy to tackle the exposures we discovered. Let's get started!</p>

  <p>Note: In order to perform this scan, you will need to have a copy of Burp Suite Professional.</p>

<h2>Creating a new project</h2>
  <p>First, we will begin by opening Burp Suite and creating a new project. Select new project on disk and enter a name for the project. For the purposes of this tutorial, I will be naming it Test Scan.</p>

  ![Step 1](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/1.png)

  <p>From here, you will be asked to select the configuration you would like to load for this project. Let's use the Burp default option and click Start Burp on the bottom right of the window.</p>

  ![Step 2](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/2.png)

  <p>Now you should see the Burp Suite dashboard. This is where the magic happens. Right now, we are going to focus on the upper left corner. You should see a button that says new scan, which I have highlighted yellow in the accompanying image. Let's go ahead and click      that so that we can move onto the next sextion of this tutorial.</p>

  ![Step 3](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/3.png)
  
<h2>Configuring your first scan</h2>
  <p>Now there should be a new window called "New scan". Here we will designate the target url we want to perform our vunlnerability scan on. </p>

  ![Step 4](https://github.com/nicknava1/Burp-Suite/blob/main/Burp%20Suite%20Scan/4.png)
