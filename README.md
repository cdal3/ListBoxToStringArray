# Opening the Project
The following sample project can be opened with or without FacotoryTalk Optix Studio Pro
## With FactoryTalk Optix Studio Pro
1. Select the green **Code** dropdown
2. Copy the repository URL to the clipboard
3. Open FactoryTalk Optix Studio and sign in to obtain the FactoryTalk Optix Studio Pro Entitlement
4. Select **Open** > **Remote**, paste the repository URL in the **Remote URL** field, set the **Location**, and Select **Open**
## Without FactoryTalk Optix Studio Pro
1. Select the green **Code** dropdown
2. Select **Download ZIP**
3. Unzip the downloaded Repository to the desired location
4. Open the **.optix** file

# Introduction
The following sample project demonstrates how to visualize a PLC Array in a FactoryTalk Optix ListBox, and write the selected value down to a string in the controller.
![ProjectGif](https://github.com/cdal3/ListBoxToStringArray/blob/main/ProjectFiles/Screenshots/ListBoxToStringArray.gif)

# Project Files
The sample controller ACD file can be found here:

# Implementation
1. Configure the Array update mode for 'Array' in the Station tags. ![Step1](https://github.com/cdal3/ListBoxToStringArray/blob/main/ProjectFiles/Screenshots/Step1.png)
2. Add a ListBox to the project.
3. Add an array of the same size as the controller array to the ListBox Properties, and tie its dynamic link to the controller array. ![Step3](https://github.com/cdal3/ListBoxToStringArray/blob/main/ProjectFiles/Screenshots/Step3.png)
4. Tie the ListBox's Model property to the Variable created in the previous step. ![Step4](https://github.com/cdal3/ListBoxToStringArray/blob/main/ProjectFiles/Screenshots/Step4.png)
5. Set the ListBox's **Display value path** property to *{Item}@Value* ![Step5](https://github.com/cdal3/ListBoxToStringArray/blob/main/ProjectFiles/Screenshots/Step5.png)
6. Set the ListBox's **Selected value** property to the controller tag of which to write the selected value back to. ![Step6](https://github.com/cdal3/ListBoxToStringArray/blob/main/ProjectFiles/Screenshots/Step6.png)
