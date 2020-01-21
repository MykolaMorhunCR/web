# Table of Contents 

- [Epic 01. Sign In/Up](#Epic-01-Sign-InUp)

    - [As User I can Sign Up Via Email + Password ](#SPIWEB-0101-As-User-I-can-Sign-Up-Via-Email--Password)
    
    - [As User I can Sign In Via Email + Password](#SPIWEB-0102-As-User-I-can-Sign-In-Via-Email--Password)
    
- [Epic 02. File management](#Epic-02-File-management)  

    - [As User I can import files from computer via Drag'n'Drop function ](#SPIWEB-0201-As-User-I-can-import-files-from-computer-via-DragnDrop-function)  
    
    - [As User I can import files from computer via Browse function](#SPIWEB-0202-As-User-I-can-import-files-from-computer-via-Browse-function)
    
    - [As User I can create a file](#SPIWEB-0203-As-User-I-can-create-a-file)
    
    - [As user I can set/change title for Item i Created/Uploaded](#SPIWEB-0204-As-user-I-can-setchange-title-for-Item-i-CreatedUploaded)
    
    - [As user I can Edit text in Created/Uploaded file](#SPIWEB-0205-As-user-I-can-Edit-text-in-CreatedUploaded-file)
    
- [Epic 03. Settings](#Epic-03-Settings)
 
    - [As User I can open settings](#SPIWEB-0301-As-User-I-can-open-settings)
    
    - [As User I can set my account name](#SPIWEB-0302-As-User-I-can-set-my-account-name)
    
    - [As user I can Report an Issue](#SPIWEB-0303-As-user-I-can-Report-an-Issue)
    
    - [As User I can set my Listening preferences](#SPIWEB-0304-As-User-I-can-set-my-Listening-preferences)
    
- [Epic 04. Library & Listening](#Epic-04-Library--Listening)

    - [As User I can see list of uploaded/created files](#SPIWEB-0401-As-User-I-can-see-list-of-uploadedcreated-files)
    
    - [As User I can choose item I want to listen to](#SPIWEB-0402-As-User-I-can-choose-item-I-want-to-listen-to)
    
    - [As User I can Pause and Continue listening via Pause/Play button](#SPIWEB-0403-As-User-I-can-Pause-and-Continue-listening-via-PausePlay-button)
    
    - [As User I can Skip n seconds Forward/Backwards via Pressing Skip buttons](#SPIWEB-0404-As-User-I-can-Skip-n-seconds-ForwardBackwards-via-Pressing-Skip-buttons)
    
    - [As User I can change speed of listening](#SPIWEB-0404-As-User-I-can-change-speed-of-listening)
    
    - [As User I can navigate through text via clicking on word, I would like to start listening from](#SPIWEB-0405-As-User-I-can-navigate-through-text-via-clicking-on-word-I-would-like-to-start-listening-from)
    
    - [As User I can change voice of listening](#SPIWEB-0406-As-User-I-can-change-voice-of-listening)
    
    - [As User I can search through text](#SPIWEB-0407-As-User-I-can-search-through-text)
 
 - [# General functionality](#GENERAL-FUNCTIONALITY)
 
 
 --------------------------------
 # Epic 01. Sign In/Up 
 --------------------------------




# SPIWEB 0101. As User I can Sign Up Via Email + Password 
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
 
 
 # SPIWEB 0102. As User I can Sign In Via Email + Password 
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
     # Epic 02. File management
   --------------------------------
  
  
 # SPIWEB 0201. As User I can import files from computer via Drag'n'Drop function 
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
  
  
 # SPIWEB 0202. As User I can import files from computer via Browse function 
 
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
  
  
 # SPIWEB 0203. As User I can create a file 
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
  
  
 # SPIWEB 0204. As user I can set/change title for Item i Created/Uploaded
 ### Steps: 
 - [Create a File](#SPIWEB-0203-As-User-i-can-create-file) OR Choose any file from your Library, by clicking on it
 
 | Action | Expected result |
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
  
  
 # SPIWEB 0205. As user I can Edit text in Created/Uploaded file
 
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
 
 - [Create a File](#SPIWEB-0203-As-User-i-can-create-file)
  
  | Action | Expected result |
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
  #Epic 03. Settings
  --------------------------------
  
  
 # SPIWEB 0301. As User I can open settings 
 
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
  
  
 # SPIWEB 0302. As User I can set my account name 
 
 ### Steps: 
 
 - Open [Settings](#SPIWEB-0301-As-User-i-can-open-settings)
 
  | Action | Expected result |
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
  
  
 # SPIWEB 0303. As user I can Report an Issue 
 
 ### Steps: 
 
 - Open [Settings](#SPIWEB-0301-As-User-i-can-open-settings)
 - Click on 'Report an Issue' button 
 
  | Action | Expected result |
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
     
  # SPIWEB 0304. As User I can set my Listening preferences 
  
  Flow №1 User is not signed in
  
  ### Steps: 
  
 - Launch app
 
 - CLick on 'Listening' button 
 
 | Action | Expected result |
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

 - Open [Settings](#SPIWEB-0301-As-User-i-can-open-settings)
 
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
# Epic 04. Library & Listening 
 --------------------------------
    
 # SPIWEB 0401. As User I can see list of uploaded/created files 
 
 ### Steps: 
 - Launch app 
 - Sign In/Up > close settings (If NOT signed in before)
 
 Expected result: List of all items, added to library before is on the left side, ordered by date added. If no items added (or all items were deleted) 'No items in the folder yet' is displayed
 
  ### Acceptance Criteria 
 - User can see all items, he added to library before
 
 
     --------------------------------
  
  
 # SPIWEB 0402. As User I can choose item I want to listen to 
 
 ### Steps: 
 - Launch app 
 - Sign In/Up > close settings (If NOT signed in before)
 - Import/Create some items (if NOT done before) 
 - Choose any item 
 
 Expected result: Listening screen appears with such attributes: 
  - Text, you created/uploaded*
  - Title of the text (above text, and on bottom bar)*
  - Play/Pause button (Only at bottom bar)*
  - Skip buttons (Only at bottom bar)*
  - Voice settings button  (Only at bottom bar) 
  - Display settings button (Only at bottom bar)*
  - Speed settings button  (Only at bottom bar)*
  - Time, that will take to listen to shis text (above text, and on bottom bar) 
  -  Time remaining ( currently not implemented)  (Above text) 
  - Search button (Above text)*
  - Cover photo (above text, and on bottom bar) 
  
    ### Acceptance Criteria 
 - User can open and listen to any item, he added to library 
 - All core* features work correctly
 
      --------------------------------
  
  
 # SPIWEB 0403. As User I can Pause and Continue listening via Pause/Play button 
 
 ### Steps: 
 - Launch app 
 - Choose an [Item](#SPIWEB-0402-As-User-i-can-choose-item-i-want-to-listen-to) 
  
 
 | Action| Expected result |
| ------ | ------ |
| User press Pause | Listening Paused |
| User press Play | Listening continues from where it stopped |

 ### Acceptance Criteria 
 - User can Press/pause his listening
 - Listening continues from where it stopped 
 - Play/Pause cause appropriate actions 
 
 -----------------------

# SPIWEB 0404. As User I can Skip n seconds Forward/Backwards via Pressing Skip buttons

 ### Steps: 
 - Launch app 
 - Choose an [Item](#SPIWEB-0402-As-User-i-can-choose-item-i-want-to-listen-to) 
 - Start Listening (Press Play button)
 
| Action| Expected result |
| ------ | ------ |
| User press Forward skip | Listening skips forward for n seconds, Appropriate text is highlighted, listening continues from appropriate point |
| User press Backwards skip | Listening skips backwards for n seconds, Appropriate text is highlighted, listening continues from appropriate point |
 ### Acceptance Criteria 
 - User can skip listening for appropriate interwals
 - Listening continues from appropriate point
 
  -----------------------------------

# SPIWEB 0404. As User I can change speed of listening

 ### Steps: 
 - Launch app 
 - Choose an [Item](#SPIWEB-0402-As-User-i-can-choose-item-i-want-to-listen-to) 
 
| Action| Expected result |
| ------ | ------ |
| User changes speed via dragging | Speed and time remaning indicator are appropriately changed, correct speed is shown  |
| User changes speed via clicking | Speed and time remaning indicator are appropriately changed, correct speed is shown |

 ### Acceptance Criteria 
 - Speed can be changed 
 - Appropriate speed is set after changing
 
  
---------------------------

# SPIWEB 0405. As User I can navigate through text via clicking on word, I would like to start listening from 

### Steps:
 - Launch app 
 - Choose an [Item](#SPIWEB-0402-As-User-i-can-choose-item-i-want-to-listen-to) 
 - Click on any word in text you are listening
 
 Expected result: Listening continues from appropriate word, appropriate word is highlighted

 ### Acceptance Criteria 
 
 - Naviagating throgh text via tapping is possible
 - Nothing is changed except from listening position highlighting and listening poing
 
  
  -----------------------

# SPIWEB 0406. As User I can change voice of listening
 ### Steps: 
 - Launch app 
 - Choose an [Item](#SPIWEB-0402-As-User-i-can-choose-item-i-want-to-listen-to) 
 - Click on 'Voice' button
 - Choose ANY of available voices
 
 Expected result: Listening continues from appropriate word, appropriate word is highlighted, voice change is saved

  ### Acceptance Criteria 
 - User can set any of avaliable for him listening voices 
 
 
   -----------------------

# SPIWEB 0407. As User I can search through text

 ### Steps: 
 - Launch app 
 - Choose an [Item](#SPIWEB-0402-As-User-i-can-choose-item-i-want-to-listen-to) 
 - Click on 'Search' icon
 
 | Action| Expected result |
| ------ | ------ |
| User clicks 'Search' icon | Search bar appears |
| User types some text to search bar | This text is immedeately searched through item, you are in right now; Found matches are highlighted with orange color, match, you are looking at right now is highlighted with green; Counter on search bar shows: number of match you are at right now/total number of matches |
| User deletes some text from search bar | This text is immedeately searched through item, you are in right now; Found matches are highlighted with orange color, match, you are looking at right now is highlighted with green; Counter on search bar shows: number of match you are at right now/total number of matches |
| Search bar is empty | nothing happens |
| User clicks 'down' icon | User moved to next matched pard of text |
| User clicks 'up' icon | User moved to previous matched pard of text |
| User closes search bar | Search bar closed, all extra highlighting from search disappeared, user is left on the same part of the text, where he was.  |


 Expected result: Listening continues from appropriate word, appropriate word is highlighted, voice change is saved

  ### Acceptance Criteria 
 - User can find whatever text he vants in any document in his library
 - Appropriate text is being searched and highlighted
 
 ------------------------------
# GENERAL FUNCTIONALITY 
------------------------------

# Sign In is obligatory
User can't most of actions, mentioned above without signing in. He can only use Settings screen

    
# Sync functionality flow

    
### User Sign In
Expected result : Books sync with created account . Books, that are already connected to this account, are added to library. Synced books become avaliable on ANY platform, when user signs in into this account.

### User Log Out
Expected result: Session deleted. Every change (added/edited books), made during this session must be saved and accessed on any platform after signing in to this account. 
 
 
 
 
 
 
 
 
 
 
 
 
