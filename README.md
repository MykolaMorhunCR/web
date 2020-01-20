
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
  
  
 # SPIWEB . As User I can import files from computer via Drag'n'Drop function 
 ### Steps: 
 - Launch app
 - Sign In/Up (if not already done) 
 - Press '+' icon 
 - Open file-browser o your computer
 - Find a File you want to upload 
 
  | Action| Expected result |
| ------ | ------ |
| Drag a file, using your mouse, to Importing window (Unsupported format) | Error "'name of the file' is not supported", file doesn't appear in 'Import' window |
| Drag a file, using your mouse, to Importing window (supported format) | File appears in Import window, 'Import' and 'Reset' buttons become avaliable |
| Click reset | All files disappear from import window, 'Import' and 'Reset' buttons become N/A |
| Click 'Import' | File appears in your Library |

  
  ### Acceptance Criteria 
 - User can upload files, using Drag'n'Drop functionality
 
 
  --------------------------------
  
  
 # SPIWEB . As User i can import files from computer via Browse function 
 ### Steps: 
 - Launch app
 - Sign In/Up (if not already done) 
 - Press '+' icon 
 
  | Action| Expected result |
| ------ | ------ |
| Press 'browse' button | File-browser opens, files of unsupported format are N/A |
| Choose a file  | File appears in Import window, 'Import' and 'Reset' buttons become avaliable |
| Click reset | All files disappear from import window, 'Import' and 'Reset' buttons become N/A |
| Click 'Import' | File appears in your Library |

  
  ### Acceptance Criteria 
 - User can upload files, using browse functionality


 --------------------------------
  
  
 # SPIWEB . As User i can create file 
 ### Steps: 
 - Launch app
 - Sign In/Up (if not already done) 
 - Press '+' icon 
 - Press 'Written Text' button
 - Press 'New Document' button
 Expected result: New blank document created in Library (Default: name 'new record', 'Type some text here' is in 'text' field )
  
  ### Acceptance Criteria 
 - User can create document
 
  --------------------------------
  
  
 # SPIWEB . As user i can set/change title for Item i Created/Uploaded
 ### Steps: 
 - [Create a File](#SPIWEB As-User-i-can-create-file) OR Choose any file from your Library, by clicking on it
 
  | Action| Expected result |
| ------ | ------ |
| Click on Title field  | Cursor is on Title field |
| User set empty Title field (NO symbols) | 'Save' button is N/A, 'Reset' button is Available  |
| User set empty Title field (Spaces) | 'Save' button is N/A, 'Reset' button is Available  (!!!Right now it can be created like this) |
| User set Title | 'Save' button becomes Available|
| User click  'Reset' button | All changes, made after clicking on text field are undone |
| User click  on any other file in Library | Pop-up 'Leave record' With two buttons ('Leave', 'Stay') appears |
| User click  'Leave' button | All changes, made after clicking on 'title' field are undone, user is redirected to file he clicked at |
| User click  'Stay' button | User stays on book, which title he was editing, All changes, made after clicking on 'title' field  stay, but are not saved, untill user clicks 'Save', |
| User click  'Save' button | All changes are saved |

  ### Acceptance Criteria 
 - User can set/change title for any of his documents
 
   --------------------------------
  
  
 # SPIWEB . As user i can Edit text in Created/Uploaded file
 
 ### Steps: 
 
 Flow №1 Edit text in created before or uploaded file
 
  - Choose any file from your Library, by clicking on it
  - Press on 'Display' button 
  - Toggle 'Edit text' switcher
 
   | Action| Expected result |
| ------ | ------ |
| Click on any part of 'text' field  | Cursor is on appropriate place on 'text' field |
| User types any text | 'Save' and 'Reset' buttons appear below, appropriate text is typed in selected place  |
| User pastes any text from clipboard | 'Save' and 'Reset' buttons appear below, appropriate text is pasted in selected place |
| User deletes any text | 'Save' and 'Reset' buttons appear below, appropriate text is deleted |
| User click  'Reset' button | All changes, made after clicking on 'text' field are undone |
| User click  'Save' button | All changes are saved |

 Flow №2 Paste/type text to newly created document 
 
 - [Create a File](#SPIWEB As-User-i-can-create-file) 
  
   | Action| Expected result |
| ------ | ------ |
| Click on the start of 'text' field  | Cursor is on appropriate place on 'text' field |
| User types any text | 'Save' and 'Reset' buttons appear below, appropriate text is typed in selected place  |
| User pastes any text from clipboard | 'Save' and 'Reset' buttons appear below, appropriate text is pasted in selected place |
| User deletes any text | 'Save' and 'Reset' buttons appear below, appropriate text is deleted |
| User click  'Reset' button | All changes, made after clicking on 'text' field are undone |
| User click  'Save' button | All changes are saved |


  ### Acceptance Criteria 
 - User can edit any document in his library 
 - User can paste text to his documents
 - User can save changes he made 
 - User can undo changes he made 
 
  --------------------------------
  
  
 # SPIWEB . As user i can Edit text in Created/Uploaded file
 
 ### Steps: 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
