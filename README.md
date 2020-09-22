# 2048C-Mod1-Demo1-Lesson1

# Lesson 1: Overview of HTML

### Demonstration: Creating a Simple Contact Form

#### Preparation Steps 

1. Ensure that you have cloned the 20480C directory from GitHub **(https://github.com/MicrosoftLearning/20480-Programming-in-HTML5-with-JavaScript-and-CSS3/tree/master/Allfiles)**. It contains the code segments for the labs and demos in this course.
2. Browse to **[Repository Root]/Allfiles/Mod01/Democode**, and then open the **DemoWebSite - Complete.sln** file.
3. Run the **DemoWebSite - Complete.sln** application.
4. In Microsoft Edge, on the address bar, note the port number that appears after **http://localhost:**. You will use this port number during this demonstration.
5. Close Microsoft Edge.


### Demonstration Steps

#### Create an HTML page

1. Open Notepad.

2. To the blank text file, add the following basic HTML structure:

   ```html
       <!DOCTYPE HTML>
        <html lang="en">
            <head>
              <meta charset="UTF-8" />
              <title>Contact Us</title>
            </head>
            <body>
   
            </body>
        </html>
   ```

3. Save the file as **[Repository Root]\Allfiles\Mod01\Democode\ContactUs.html**.

#### Add content to the page

1. In the **&lt;body&gt;** element, add a level 1 page heading:

   ```html
    <h1>Contact Contoso Conferencing</h1>
   ```

2. Add the company address by using two paragraphs and a line break element:

   ```html
   <p>Contoso Conferencing Ltd.</p>
   <p>
       123 South Street<br />
       Somewhere<br />
       Over There<br />
       <em>USA</em>
   </p>
   ```

3. For the company's contact email address, add a hyperlink. Note the use of the **mailto** protocol rather than the more common http.

   ```html
    <p>
        <a href="mailto:contact@contoso.com">
        contact@contoso.com</a>
    </p>
   ```

4. To invite users to use the contact form, add the following text:

   ```html
    <p>
        If you would like to contact Contoso Conferencing, whether you're interested in our services or in a conference we're currently organizing, don't hesitate to contact us by using our enquiry form. (<strong>Bold fields</strong> are required.)
    </p>
   ```

5. Save the file.

#### Add a form with input controls

1. In the page, below the previously added text, add the following **form** element:

   ```html
    <form method="Post" action="support.aspx">
    </form>
   ```

2. Between the **&lt;form …&gt;** tag and the **&lt;/form&gt;** tag, add a **fieldset** element and a **submit** button.

   ```html
    <fieldset>
        <legend>
            Your Details and Enquiry
        </legend>
    </fieldset>
    <input type="submit" value="Send" />
   ```

3. In the **&lt;fieldset&gt;** element, below the **&lt;/legend&gt;** tag, add the unordered list in the following code sample.  This list contains input elements for the user's name, telephone number, email address, and a message.

   ```html
    <ol>
        <li>
          <label>
            <strong>Name</strong><br />
            <input type="text" 
                   name="UserName" />
          </label>
        </li>
        <li>
          <label>
            Telephone<br />
            <input type="text" 
                   name="Phone" />
          </label>
        </li>
        <li>
          <label>
            Email Address<br />
            <input type="text" 
                   name="Email" />
          </label>
        </li>
        <li>
          <label>
            <strong>Message</strong><br />
            <textarea name="Message" 
              cols="30" rows="10">Add your message here
            </textarea>
          </label>
        </li>
    </ol>
   ```

4. Save the file, and then close Notepad.

### View the page

1.	Open File Explorer.
2.	Browse to **[Repository Root]\Allfiles\Mod01\Democode**.
3.	To display the page in Microsoft Edge, double-click **ContactUs.html**.
4.	If the **How do you want to open this type of file (.html)?** dialog box appears, select **Microsoft Edge**.

![alt text](D:/610 - Curso Desarrollo Web/Practicas/JavaScript/2048C/Instructions/Images/20480B_1_ContactUs.png "About page")