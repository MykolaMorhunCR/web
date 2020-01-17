
# SPIWEB . As User I can Sign Up Via Email + Password 
 ### Steps: 
 - Launch app
 - Press 'Sign Up' button 

  | Action| Expected result |
| ------ | ------ |
| User registers with email without "@". | Sign Up button N/A |
| User registers with empty email | Sign Up button N/A  |
| User registers with email, that is already registered| Message 'The email address is already in use by another account.' is shown|
| User registers with different password and repeat password |  Sign Up button N/A  |
| User enters Password < 6 symbols|  Sign Up button N/A |
| User registers with valid data (email/username and password)|  Sign Up becomes available |
| User click 'Sign Up' button |  Account created, user becomes signed in, redirected to default settings screen |

  ### Acceptance Criteria 
 - User can Sign Up vie Email + password Combination 
 
 --------------------------------
 
 
 # SPIWEB . As User I can Sign In Via Email + Password 
 ### Steps: 
 - Launch app
 
 | Action| Expected result |
| ------ | ------ |
| User enters valid username/email/phonenumber and password | user successfully logged in |
| User sets incorrect username/email/phonenumber | Error |
| User sets empty username/email/phonenumber | Sign Up button N/A  |
| User sets incorrect password | Error |
| User sets empty password |  Sign Up button N/A  |
|User logins with valid credentials but connection is OFF |  Error about missing connection |
| Check local storage in browser after successful Sign In  |  session object is present |

  ### Acceptance Criteria 
 - User can Sign Up vie Email + password Combination 
 
  --------------------------------
 
  # SPIWEB . As User i can set my Listening preferences 
  
  Flow №1 User is not signed in
  
  ### Steps: 
  
 - Launch app
 - CLick on 'Listening' button 
 
  | Action| Expected result |
| ------ | ------ |
| User clicks 'Default Listening Language' drop-menu  | Drop menu with all awailable voices appear |
| User sets any voice | Voice set, drop menu closed |
| User clicks 'Default Speed' drop-menu  | Drop menu with awailable default speed choices appear |
| User sets any available speed | Speed set, drop menu closed |
| User clicks 'Automatic Speed Ramping' switcher(state - OFF)   |  Switcher lights up with vlue and swipes right. 'Automatic Speed Ramping' settings become available|
| User clicks 'Automatic Speed Ramping' switcher(state - ON)   |  Switcher lights goes grey, 'Automatic Speed Ramping' settings become N/A|
| User clicks 'Speed Ramping' drop-menu  | Drop menu with awailable  speed ramping choices appear |
| User sets any available speed | Speed set, drop menu closed |


 Flow №1 User is signed in
  
  ### Steps: 

 - Open Settings 
 
 - CLick on 'Listening' button 
 
  | Action| Expected result |
| ------ | ------ |
| User clicks 'Default Listening Language' drop-menu  | Drop menu with all awailable voices appear |
| User sets any voice | Voice set, drop menu closed |
| User clicks 'Default Speed' drop-menu  | Drop menu with awailable default speed choices appear |
| User sets any available speed | Speed set, drop menu closed |
| User clicks 'Automatic Speed Ramping' switcher(state - OFF)   |  Switcher lights up with vlue and swipes right. 'Automatic Speed Ramping' settings become available|
| User clicks 'Automatic Speed Ramping' switcher(state - ON)   |  Switcher lights goes grey, 'Automatic Speed Ramping' settings become N/A|
| User clicks 'Speed Ramping' drop-menu  | Drop menu with awailable  speed ramping choices appear |
| User sets any available speed | Speed set, drop menu closed |

  ### Acceptance Criteria 
 - User can open listening preferences screen 
 - User can set Default Listening Voice 
 
  --------------------------------
  
  
 

 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
