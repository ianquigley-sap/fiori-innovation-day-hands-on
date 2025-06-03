#  Exercise 3 - Generate and enhance an app 


In this exercise we will put your learning from the other exercises to the test! You will re-use your skills of generating a Fiori app from a picture, but this time we will create ai generated mock data and enhance the app with the flexible programming model.

Please be aware that you need to complete: [Exercise 0 - Getting Started - Setting up your Development Environment
](../ex0/README.md) and [Exercise 2.1 - Generate an SAP Fiori app from an image](../ex2/README.md)  before you can start Exercise 3.

## Exercise 3.1 Generate your app

Navigate to you explorer in the business application studio and look for the **TravelScenario.png** picture. Double click on the picture to see the preview.
  
![image](ex3img1.png)

The Preview should look like this:

![image](ex3img2_2.png)

1. Next, navigate to **SAP Fiori** in your Business Application Studio menu on the left side.
2. Click on **Choose file (md, txt, jpg)**
3. Select the **TravelScenario.png** from the drop down.

![image](ex3img3.png)

If **Project folder path** appears in **Project Accelerator**, please ensure that the path `/home/user/projects/ai-image-samples/` is inputted

![image](ex3img3-1.png)

Click **Generate**

![image](ex3img4.png)

Once the app has been successfully generated
1. A page should open named **Application Information**
2. Click **Preview Application**.

![image](ex3img5.png)

Select the **watch** option when prompted

![image](ex3img5-2.png)

The preview of the newly generated app should look like the following picture.

![image](ex3img6.png)

## Exercise 3.2 Enhance your app

As a next step we want to enhance our AI generated app. To do this switch back from your **Preview** tab in your browser to your **Business Application Studio** tab again. 

1. Go to the **Application Information** page
2. Click on **Open Page Map**

![image](ex3img7.png)

Now you can see the page map for our AI generated Travel app. Please check if you can see the **Advanced Features Are Enabled** sign up top. If this is the case, press the edit button on the list report.

![image](ex3img8.png)

As the next step, we want to add an additional column that indicates wether it is a business flight, and another one showing the flight destination.\
Please find the columns section and press the **Add column** button.

![image](ex3img9.png)

Now we want to select *Add Basic Columns** from the drop down menu.

![image](ex3img10.png)

Please open up the dropdown.

![image](ex3img11.png)

In the input field, type in **Business** and set the checkmark on the left hand side radio box.

![image](ex3img12.png)

1. Now click on **String** on the right hand side.
2. Select **Boolean** 

![image](ex3img13.png)

Click Add.

![image](ex3img14.png)

Now we want to add a second column. Please repeat pressing the **add column** button the right hand side again.

![image](ex3img15.png)

Open up the dropdown again.

![image](ex3img16.png)

1. In the input field, type in **Destination** and set the checkmark on the left hand side radio box. This time we want to leave the selection on the right hand side on **String**. 
2. Click on **Add**

![image](ex3img17.png)

In the Columns section you now can see our newly added column (Business & Destination). Now we want to move to the middle on the list. To do so click on the up arrow shown in the picture. 

![image](ex3img18.png)

Once this is done, we want to preview the app again to see the newly created columns in action. Switch to your **preview** tab in your browser and reload the tab with CTRL+R (Windows) or COMMAND+R (Mac). This will reload the app and reveal the new columns Business and Destination.

![image](ex3img19.png)

## Exercise 3.3 Use Ai to refine Test Data 

 If you successfully previewed the two new columns (Business and Destination). We can now press the **Use Ai to refine Test Data** Button. 

 ![image](ex3img21.png)

 Click on **Generate**

 ![image](ex3img22.png)


To reload the app with our generated Ai Mock Data we have to go to our Terminal at the bottom of the page. <br>
Click inside of the terminal field and press:<br>
**control + c (on Mac)**<br>
**CTRL + c (on Windows)**<br>

You should now see<br>**(CDS) - my watch has ended<br>
user: fiori-tools-ai $**

![image](ex3img191.png)

Repeat the steps to preview the application from earlier.

![image](ex3img5.png)
![image](ex3img5-2.png)


You may see a message in the terminal stating that the port is already in use (from previewing our application from exercise 1), click **Return/Enter** to use any other port for preview

![image](ex3img20.png)

You can now see your Ai Mock Data in the preview.

![image](ex3img201.png)

## Exercise 3.4 Flexible column layout

As the next step we want to switch the layout of the app to the flexible column layout. <br>
1. To have more room in the business application studio we can now close the preview.<br>
2. Now click on **Page View**

![image](ex3img24.png)

Navigate to the Felxible Column Layout on the right side. Switch from the **Standard Layout** to the **Flexible Column Layout**. For the 2 column layout select **Mid-Expanded**.

![image](ex3img25.png)

As a next step switch to you **Preview** tab again to reload your app with: <br>
**CTRL + R (Windows)**<br>
**Command + R (Mac)** <br> 
After this step click on the first item in the list to experience the flexible column layout.

![image](ex3img26.png)

Now click on the first line on the object page

![image](ex3img27.png)

## Exercise 3.5 Using the Flexible Programming Model

The available [SAP Fiori elements floorplans](https://help.sap.com/docs/SAP_FIORI_tools/17d50220bcd848aa854c9c182d65b699/2b2b12e708944d85a40d087194cc1edd.html) for OData V4 cover most business scenarios that customers encounter with SAP. In fact, SAP uses these SAP Fiori elements floorplans to create roughly 80% of new SAP S/4HANA apps.\
If these floorplans do not meet your needs, the [flexible programming model](https://ui5.sap.com/test-resources/sap/fe/core/fpmExplorer/index.html#/overview/introduction) provided by SAP Fiori elements allows to assemble your custom design by combining the available building blocks with SAPUI5 controls,\
and leverage controller extensions in order to fine-tune the behaviour of your app.\
For our scenario we want to combine building blocks filter bar and table in a custom section, enabling the user to set a filter on the bookings of a selected travel.

Please click one the **SAP Fiori** button in the left hand navigation![](image2.png)


![](image1.png)

Now open the **Open Application Info** on your most recently created app. Depending if you accomplished all exercises this should be ai-created-cap 5.  ![](image4.png).

![](image3.png)

Click on **Open Page Map**.

![](image5.png)

Click on **Configure page** for the object page. ![](image8.png).

![](image7.png)

Press the **Delete** button ![](image10.png) to delete section **Bookings**.

![](image9.png)

If you run into the following Error, please reload BAS: <br>
**CTRL + R (Windows)**<br>
**Command + R (Mac)** <br> 

![](image92.png)

Next click on the **Add Sections** ![](image14.png) menu item.



![](image13.png)

Click **Actions** and select ![](image16.png).

![](image15.png)

1. Type in **Bookings** as a title.
   
2. Click ![](image18.png) to generate a translatable text key.

3. Click  ![](image19.png).

![](image17.png)

Please fill in the fields as shown below and make sure everything is entered correctly. Then click on **ADD**.

![](image20.png)

We have now successfully created a new custom section extending the app based on an XMLfragment. **Please make sure it shows (Custom Section) after Bookings. If this is not the case please reload your tab.**  
We need to make sure that the browser view cache is deactivated during testing our development, so that changes applied to the xml fragment get properly updated when refreshing the UI.\
For this, we will use the watch script that has been added to file **package.json** by the app generator. The script contains additional parameter **sap-ui-xx-viewCache=false** added to the app start Url.

In the Application Modeller pane, click **Preview Application** ![](image22.png).

![](image21.png)

Choose the second entry ->  **cds watch \--openmyapplication/webapp/index.html?sap-ui-xx-viewCache=false** 

![](image23.png)

1. Switch to your preview tab in your Browser. 
2. Click on the first entry of your list report to find our newly created custom section on our object page.

![](image241.png)


![](image25.png)

Switch back from your preview tab to the page editor in your Business application studio and expand custom section **Bookings**.

![](image26.png)


Now we want to add building block filter to our custom section.\
Click button **Add** ![](image29.png).

![](image28.png)

Select ![](image31.png).


![](image30.png)


1. Click ![](image33.png) to reveal the dropdown for **Aggregation Path**.

2. Select ![](image34.png).\
   This ensures that the filter building block will be added at the corresponding position in the XML fragment.

![](image32.png)

Click **Add**.

![](image35.png)

We will now define a filter field to be shown in the filter bar.\
Click **Add Filter Fields** ![](image14.png).

![](image36.png)

1. Click ![](image38.png) to reveal the dropdown.

2. Check the radiobox for ![](image39.png).
3. Click Add.

![](image37.png)

1. Open the filter bar properties panel by clicking entry ![](image41.png).

2. Search for property **Live Mode** and seleset it to **True**.

![](image40.png)

1. Search for property **Show Clear Button** and set it to **True**.

![](image44.png)

In the page editor, click **Edit in source code** ![](image48.png) for filter field **Flight Date** to navigate to the corresponding annotation.

![](image47.png)

For the filter field, we will now enable the usage of semantic date values, such as **Today** or **Last Week**, by applying annotation ****FilterRestrictions.AllowedExpressions** as described in [the documentation](https://ui5.sap.com/#/topic/fef65d03d01a4b2baca28983a5449cf7).\
Please copy the Code snippet below and paste it on the exact position that is shown in the picture:

```
    Capabilities : {
      FilterRestrictions : {
        FilterExpressionRestrictions :
          [{
              Property : 'flightDate',
              AllowedExpressions : 'SingleRange'
          }]
      }
    }
```

![](image49.png)

Switch to your preview tab to see the latest changes to your app. If you cant see the latest changes please reload your browser window.

![](image50.png)

Switch back to your Business application studio. We will now use **Guided Development** to add a table building block.\
Guided development allows the user to walk through the steps required to implement a specific functionality in the Fiori element application.\
Click on the **SAP Fiori** icon in the left hand side panel.

![](image5321.png)

Click on **Open Application Info** on your latest app.

![](image3.png)

Click on **Open Guided Development**.

![](image531.png)

Close the **Application Info** tab to free up more space in the editor.

![](image532.png)

1. Now use the search on the top right hand of the screen and type in **"Table Building Block"**
2. Click on **"Add a table building block"**

![](image533.png)

**Start the guide**

![](image534.png)

1. In the first step of the guide, fill in fields **CDS File / Service / Entity** as depicted below.
2. Click Next.

![](image535.png)

In the second step of the guide, fill in the required fields as depicted below.

![](image536.png)

**Scroll down** and click **Insert Snippet**.

![](image537.png)

1. File **Bookings.fragment.xml** is opened, showing the table building block added to the defined aggregation path position. It should look like this:
```
<macros:Table id="Table" metaPath="/Travels/bookings/@com.sap.vocabularies.UI.v1.LineItem" filterBar="FilterBar" headerVisible="true" isSearchable="true" selectionMode="Single" type="ResponsiveTable" variantManagement="None"/>
```
2. Click on **Exit Guide**



![](image538.png)

Switch to your preview tab to see the result. You can now specify a range in the newly added filter bar.
1. Select a travel entry in the List Report to open the travel details in the object page.
2. In the **Bookings** section, open filter field **Flight Date** and select a date range.
3. Click **Apply**.

![](image56.png)

The filter is applied to the bookings table.

![](image58.png)


## Summary

You now have completed the Hands-on. Thank you very much for participating.


