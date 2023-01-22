### NgRx -- Angular Reactive Extensions
     --Based on Redux.  

### WHY STATE MANAGEMENT
           --Without State Management The Static Data is Fetched again and again when the User Navigate to different Pages.
           --Without State Management we Constantly Sending/Issue Http Requests to the Backend/Server to Fetch Static Data.
           --Without State Management When the User Tries to Modify/Update the Data, it will Reload the Page and Show the Loading Spinner in order to Show the UPDATED data to the User.
           --Without State Management The OBSERVABLES inside a Component are DEPENDENT on the Component itself i.e The LIFECYCLE of the OBSERVABLE is TIED to the Component.--When the Component is Initialized the Lifecycle of the Observable is Created and When the Component is Destroyed the Observable is Also Destroyed. 

### STATE MANAGEMENT SOLUTION
           --Creating In-Memory Database on the Client Side to Keep Application Data THAT IS INDEPENDENT of the LIFECYCLE of any Component, While the App is ACTIVE.
           --Reduce the no. of Http Requests for the Data That is Not Modified i.e The FETCHING of Static data is IMMEDIATE without showing any Loading Spinners.
           --Updating/Modify the Data and Showing Changes Immediately on the USER SCREEN Without any Loading Spinners for BETTER USER EXPERIENCE.
           --Improved User Experience and App Performance.

### INSTALLING NgRx-Store and NgRx-DevTools
           ** ng add @ngrx/store 
           -- import {StoreModule} from '@ngrx/store';
           -- StoreModule.forRoot(reducers, { metaReducers }) inside imports []

           -- With This Installation We ADD In-Memory Database to Our Application where we Can Store and Read Data.

           ** Install DevTools -ng add @ngrx/store-devtools

           -- DevTools are BROWSER Extension that Allows to see Content of Our In-Memory Database using ChromeDevTools.

