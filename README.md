
# SPIWEB . As User I can Sign Up Via Email + Password 
 ### Steps: 
 - Launch app
 - Press 'Sign Up' button 

  | Action| Expected result |
| ------ | ------ |
| User registers with email without "@". | Sign Up button N/A |
| User registers with empty email | Sign Up button N/A  |
| User registers with email, that doesn't match {local part}@{Domain part} form. | Sign Up button N/A |
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
| User enters valid username/email/phonenumber and password | user successfully logged in, redirected to defaulot settings screen |
| User sets incorrect username/email/phonenumber | Error |
| User sets empty username/email/phonenumber | Sign Up button N/A  |
| User sets incorrect password | Error |
| User sets empty password |  Sign Up button N/A  |
| User logins with valid credentials but connection is OFF |  Error about missing connection |
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
  
  
 # SPIWEB . As User I can import files from computer via Browse function 
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
  
  
 # SPIWEB . As User I can create file 
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
  
  
 # SPIWEB . As user I can set/change title for Item i Created/Uploaded
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
  
  
 # SPIWEB . As user I can Edit text in Created/Uploaded file
 
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
  
  
 # SPIWEB . As User i can open settings 
 
 ### Steps: 
 
 Flow №1 User already Signed In/Up 

 - Launch app 
 - Press 'Settings' icon 
 
 Expected result: screen with such options appear 
 
 - Account Data* (Default) 
 - Message Us 
 - Report an issue* 
 - Listening*
 - Shortcuts 
 - Sign Out 
 
  Flow №2 First launch / user logged out before

 - Launch app 
 
 Expected result: screen with such options appear 
 
 - Sign In* (Default) 
 - Message Us 
 - Report an issue* 
 - Listening*
 - Shortcuts 
 
 
   ### Acceptance Criteria 
 - User can open Settings 
 - All core* options are avaliable and function correctly 

   --------------------------------
  
  
 # SPIWEB . As User I can set my account name 
 
 ### Steps: 
 
 - Open [Settings](# SPIWEB . As User i can open settings )
 
   | Action| Expected result |
| ------ | ------ |
| Click on 'Display Name' field  | Cursor is on 'Display Name' field |
| User set new acc name | Update button becomes Available  |
| User closes settings | Changes are not saved | 
| User goes to another settings screen | Changes are not saved | 
| User closes tab in browser | Changes are not saved | 
| User clicks 'Update' button | Changes are saved | 

 ### Acceptance Criteria 
 - User can set his account name
 
   --------------------------------
  
  
 # SPIWEB . As user i can Report an Issue 
 
 ### Steps: 
 
 - Open [Settings](# SPIWEB . As User i can open settings )
 - Click on 'Report an Issue' button 
 
    | Action| Expected result |
| ------ | ------ |
| User clicks 'Type of feedsback' drop-menu  | Drop menu with all awailable types of feedback appear |
| User sets any type | Type set, drop menu closed |
| User swaps settings screen | All cahnges/updates made to 'Report an issue' are undone |
| User closes Speechify tab in browser | All cahnges/updates made to 'Report an issue' are undone |
| User closes Settings screen | All cahnges/updates made to 'Report an issue' are undone |
| User clicks on 'Tell us more...' field  | Cursor is on 'Tell us more...' field |
| User writes\edits\deletes some text in 'Tell us more...' field | Text is written\edited\deleted, any symb. allowed |
| Press 'Add a photo or file' button | File-browser opens, files of unsupported format are N/A |
| Choose a file (!!! Right now ONLY photos are available) | File appears in  'Add Additional content' block, together with 'Preview' and 'Delete' icons for every file uploaded |
| Click 'Preview' icon | Chosen files' preview is shown |
| Click 'cross' icon | Preview closed |
| Click 'Delete' icon | Uploaded file deleted from  'Add Additional content' block |
| User clicks on 'Email' field (Your email, set when registering is set by default) | Cursor is on 'Email' field |
| User sets email without "@". | 'Send Feedback'  button N/A |
| User sets empty email | 'Send Feedback'  button N/A  |
| User sets email, that doesn't match {local part}@{Domain part} form. | 'Send Feedback'  button N/A |
| User sets valid email | 'Send Feedback'  button becomes available |
| User press 'Send Feedback'  button | Message is sent to Speechify administration |

 ### Acceptance Criteria 
 - User can set set type of an issue
 - User can Add additional text info to his report
 - User can add Photo or a File to his report 
 - User can set Email, from which his report will be reported
 - Message can be send to Speechify administration 
 
 
    --------------------------------
  
  
 # SPIWEB . As user i can Report an Issue 
 
 ### Steps: 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
