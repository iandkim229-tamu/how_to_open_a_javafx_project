# How to open a JavaFX project
## Opening a JavaFX project in Eclipse
1. Click on `File` -> `Open Projects from File System` -> `Directory`.

   Select the project folder.
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/eclipse_step1.gif" width=50% height=50%>
###
###
2. Click on `Window` -> `Preferences`.

   `Java` -> `Build Path` -> `User Libraries` on the left tab of the Preferences window
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/eclipse_step2.gif" width=50% height=50%>
###
###
3. Click on `New` and type name of library in `User library name` (`JavaFX` in this case).
   
   Go to `{directory to JavaFX SDK}/bin` and select all `.jar` files, click on open.
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/eclipse_step3.gif" width=50% height=50%>
###
###
4. Right click on `wordle_final_project` in the package explorer and go to `Build Path` -> `Configure Build Path`.
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/eclipse_step4.gif" width=50% height=50%>
###
###
5. Click on the `Libraries` tab and click on `Classpath` -> `Add Library`.

   Select `User Library` and click on `Next`.

   Select the added libarary (`JavaFX` in this case) and click on `Finish` -> `Apply and Close`.
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/eclipse_step5.gif" width=50% height=50%>
###
###
6. Select the Java file containing the main method, which is `wordle_final_project/src/(default package)/App.java`.
   
   Click on the arrow on the right of the `Run App` button and click on `Run Configurations` on the dropdown.
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/eclipse_step6.gif" width=50% height=50%>
###
###
7. Double click on the `Java Application` on the left.
   
   Click on the `Arguments` tab and type `--module-path "{Path to JavaFX SDK}/lib" --add-modules javafx.controls,javafx.fxml` in the VM arguments text box. Do remember to replace the curly brackets and the contents within with your own path to the JavaFX SDK.

   Click on `Run` and you should be able to see the project window. You should be able to run the project through the `Run App` button now.
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/eclipse_step7.gif" width=50% height=50%>

## Opening a JavaFX project in Visual Studio Code
1. `launch.json` has been set up for the project. However, you may need to change the JavaFX run directory.
  
   Go to `.vscode`/`launch.json` and change `C:/sdk/javafx-sdk-18.0.1/lib` to `{Path to JavaFX SDK}/lib`. Do remember to replace the curly brackets and the contents within with your own path to the JavaFX SDK.
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/vscode_step1.gif" width=50% height=50%>
###
###
2. You may have to add Jar files to `Referenced Libraries`.

   Open the `Java Projects` -> `wordle_final_project` dropdown on the bottom left.

   Hover over `Referenced Libraries` and click on the plus icon beside it.

   Go to `{directory to JavaFX SDK}/bin` and select all `.jar` files, click on `Select Jar Libraries`.
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/vscode_step2.gif" width=50% height=50%>
###
###
3. Click on `Run` -> `Run Without Debugging`. You should be able to see the project window.
<img src="https://github.com/iandkim229-tamu/how_to_open_a_javafx_project/blob/main/Resources/vscode_step3.gif" width=50% height=50%>
