#  Exercise 2 - Generate an SAP Fiori app from an image

In this exercise, we will create a number of SAP Fiori apps, but instead of using a text document as input, we will use images of the applications that we want to create.

## Exercise 2.1 Downloading the sample images into SAP Business Application Studio

Copy the repository link below:

```
https://github.com/ianquigley-sap/ai-image-samples
```

From the menu select **View -> Command Palette**.

![image](ex2img1.png)

Search for command **git clone** and select it.

![image](ex2img2.png)

Paste the repository link into the input field and hit enter.

Choose the projects folder for the repository location and click **Select as Repository Destination**.

![image](ex2img3.png)

Click **Cancel** to see the repository added under **projects** in the current workspace.

![image](ex2img4.png)

## Exercise 2.2 Launching the SAP Fiori tools AI Project Accelerator with image input

Click the **SAP Fiori** icon in the left hand side panel.\
Similar to exercise 1, click **Launch Project Accelerator** (you can close the **Application Modeler** and **Information** sections):

![image](ex2img5.png)

Click the **Choose file** link.

![image](ex2img6.png)

Select the **countries.jpg** file from the **ai-image-samples** folder.

![image](ex2img7.png)

A thumbnail of the image should appear in the input box. Click **Generate** to start generating the application directly from the image.

![image](ex2img8.png)

The application will start generating, give it some time.

![image](ex2img9.png)

## Exercise 2.3 Previewing the generated application

After generation, the **Application Info** page should open automatically. Click the **Preview Application** button to launch a preview of the application.

![image](ex2img10.png)

Select the watch script from the Preview Options dropdown when prompted.

![image](ex2img11.png)

You may see a message in the terminal stating that the port is already in use (from previewing our application from exercise 1), click **Return/Enter** to use any other port for preview.

![image](ex2img12.png)

The application should launch in a new browser tab. Click **Go** to see the sample data that the AI has created.

![image](ex2img13.png)

## Summary

You've now successfully generated a SAP Fiori app using a sketch of the application you'd like to generate.

Continue to - [Exercise 3 -  Generate and enhance an app](../ex3/README.md)
