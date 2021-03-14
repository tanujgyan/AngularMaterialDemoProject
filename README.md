This is a demo project aimed at integrating Angular Material in Angular 11 project. This is a simple CRUD app \
It can be used as a start project 

**Basic test setup to check if integration is successful**
Step 1: Create a new angular app using command ng new AngularMaterialDemo \
Step 2: Install Angular Material. The best way to install it is using CLI. Run the following command ng add @angular/material \
You can choose a theme or add your own custom theme however be careful with dark themes like pink-bluegrey.css or purple-green.css as the structure input won’t be noticeable \
Read about it here https://rdineshkumar88.medium.com/input-field-not-visible-in-angular-material-dark-themes-solved-11329553e1ac \
Step 3: Import the stylesheet to style.css 
```css @import '~@angular/material/prebuilt-themes/indigo-pink.css'; ``` \
Step 4: The controls that you want to use have to be imported in app module ts file. also add them to import array \
```import {MatInputModule} from '@angular/material/input'; ``` \
```import {MatButtonModule} from '@angular/material/button'; ```

Step 5: In your app.component.cs file add the css 
```css
:host { 
    display: flex; 
    flex-direction: column; 
    align-items: flex-start; 
  } 
  ```
 Step 6: Add the following code to your app.component.html file. This will just create two textboxes and a button to make sure everything is working fine and imported correctly 
 ```html
   <mat-form-field  appearance="outline">
    <mat-label>Name:</mat-label>
    <input matInput >
  </mat-form-field>
  
  <mat-form-field appearance="outline">
    <mat-label>Address:</mat-label>
    <input matInput >
  </mat-form-field>
  
<button mat-raised-button color="primary">Submit!</button>
```
