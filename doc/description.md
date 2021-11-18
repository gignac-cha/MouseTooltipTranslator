When mouse hover on text, it shows translated tooltip in any language.  

# Features
- hover or select (highlight) on text to translate  
- Visualize tooltip on any web page (except chrome web store site)
- handle google translator and bing translator for translation
- In the setting, google TTS (text to speech) is available to listen text
- Support pdf to display translated tooltip using PDF.js
- Filter out when source language and target language are same
- (Experimental) translate youtube caption when mouse over subtitle block
- (Experimental) Use OCR to comic when hover on bubble background

# Source code  
- https://github.com/ttop32/MouseTooltipTranslator  

# Setup Guide
If pop-over translate tooltip is not came out properly after installation, user need to reload all your existing pages to run web page with this extension for using extension feature. And, make sure to setting target translate language properly from pop up configuration page. Pop up configuration page is provided by click extension icon top right corner and click this extension's blue mouse icon. If user want to use this extension on local file, user need to set “allow access to file URLs” from "chrome://extensions/?id=hmigninkgibhdckiaphhmbgcghochdjc".    

# Change Log   
- 0.1.37
  - google reject by “Having excessive keywords in description”  
    - Google announce "Irrelevant information about Translate"   
    - remove "Translate" from title   
    - remove some description about "Translate"  
- 0.1.36  
  - alert local pdf file permission  
  - fix pdf request header detection    
  - add pdf detect option to allow pdf translate (request by Meow Meow)   
- 0.1.35
  - fix pdf viewer problem when open with new tab (request by M9VK)
  - fix pdf viewer url parameter crash (request by sensypo)
- 0.1.34
  - remove sendMessage (stop tts)
- 0.1.33
  - avoid to use sendMessage (stop tts) when leave tab
- 0.1.32
  - add "translate When" option to replace "translate on hover" (request by Alex)
  - load setting from storage instead of background service worker
  - fix tooltip position problem when crtl pressed
  - set initial "translate into" value correctly
- 0.1.31
  - remove multiple sendMessage call to reduce cpu usage (request by M9VK)
- 0.1.30
  - update to google chrome manifest v3  
  - remove opencv, use canvas to process crop for ocr translate
  - remove option "translate on hover" and "translate on select"
  - use vue loader  
  - use chrome tts instead of google tts rest api
  - update tooltip translator pdf viwer to use v2.8.335 pdfjs  
  - support command key as translator activation hold key  
  - support right to left alignment for translate to Persian   
  - move background ocr process to iframe  
  - fix translator tooltip position (problem when it is first shot)
- 0.1.29   
  - fix bing translator communication crash(request by zx xu)  
  - support right to left alignment for translate to Arabic (request by mohamad-b)   
  - add translate text history section on popup page (request by TeraStrider)  
- 0.1.28  
  - support translate on selection (contributed by sanprojects)  
- 0.1.27  
  - support youtube subtitle cpation to show translator tooltip (request by Veratyr)  
  - fix gmail pdf attachment crash with translator viwer (request by junkey)  
- 0.1.26  
  - increase tooltip z-index for particular site (request by WM)  
  - add customization feature on tooltip width (request by Bambang Sutrisno)  
  - change description  
- 0.1.25
  - google reject by “Having excessive keywords in description”
    - Google anonunce "Irrelevant information about Mouseover Translate" again
    - remove all main description
- 0.1.24
  - google reject by “Having excessive keywords in description”
    - Google anonunce "Irrelevant information about Mouseover Translate"
    - remove "Mouseover Translate" from title and package summarization
- 0.1.23
  - google reject by “Having excessive keywords in description”
    - Google anonunce to remove "google translate"
    - remove “google translate” from package summarization
    - avoid to use continuously mentioned “google translate”
- 0.1.22
  - fix translator type "bing" to correctly handle bing translator api   
  - uses "npm aduit fix" to update this translator library   
- 0.1.21
  - Support translator to translate word (request by Amir Rezaei)
  - Support reverse translate (request by Amir Rezaei)
  - When activation hold key is set, turn off permanent feature enable
- 0.1.20
  - Change promo tile name to Mouseover Translate
  - Change manifest description to Mouseover Translate
- 0.1.19
  - remove vue jsx
  - fix popup page title name
  - add "about section" on popup page
- 0.1.18
  - Support multilingual manifest description again
  - Rollback "Setup Guide" description
- 0.1.17
  - Google reject by “Having excessive keywords in description” again
    - No detail guideline is provided. Make guess to remove some item.
    - Remove all "Detail Description"
    - Remove all "Setup Guide"
- 0.1.16
  - google reject by “Having excessive keywords in description”
    - Guideline is provided to fix some description item.
    - Remove “Supported Translation Languages with google translate”
    - Remove “Supported TTS languages with google TTS”
    - Avoid frequently mentioned Mouse tooltip translator in description
  - Remove multilingual manifest description
  - Rollback google translate respond to fix it
  - Rollback extension name to Mouse tooltip translator
- 0.1.15
  - Change name, Mouse tooltip translator to Mouseover translator
  - Support font size customization (request by Ramy_Ahmed.87)
  - Support Bing translator (request by Ramy_Ahmed.87)
  - Fix google translate response
- 0.1.14
  - Fix hide tooltip (show tooltip after mouse move)
  - Support multilingual manifest description using google translate
- 0.1.13
  - Filter out when only detect currency sign text
- 0.1.12
  - Fix base64 image OCR response
  - Use Vue JSX on popup page
- 0.1.11
  - Use Vue and Vuetify on popup page
  - Add options_ui
  - Add step to load base64 image on OCR
  - Add step to resize image on OCR
  - Add image preprocessing step on OCR
- 0.1.10
  - Fix URL text filter
  - Filter text that only include number and special character
  - Hide tooltip when leave tab
  - Fix hiding when ctrl+a or ctrl+f is pressed
- 0.1.9
  - Only load bootstrap tooltip library (not whole bootstrap)
  - Apply script lazy load on manga OCR library script
  - Use transform method for tooltip positioning
- 0.1.8
  - Fix TTS (text to speech) stop message sending
  - Fix OCR image load
  - Use zodiac3539's train data for tesseract jpn_vert OCR
- 0.1.7
  - Fix scrolled tooltip dictionary position
  - Hide tooltip when ctrl+a or ctrl+f is pressed
  - Change popup page container design as cool design
  - Stop played TTS (text to speech) when leave tab
  - Only activate tooltip when tab is focused
  - Support bubble translate using tesseract.js (OCR) and opencv.js
  - Update translated pdf viewer using PDF.js 2.5.207
  - Filter out text that has over 1000 length
- 0.1.6
  - Fix to save setting correctly
  - Change hold key to action immediately
  - Fix popup page capital letter
- 0.1.5
  - Fix subframe pdf to work correctly
  - Fix dropdown menu crash from site that use bootstrap
- 0.1.4
  - Fix pdf line break
- 0.1.3
  - Add fade animation
  - Fix TTS (text to speech) enabled case to recognize
- 0.1.2
  - Increase tooltip margin
  - Prevent translate on URL text
  - Support pdf tooltip translate using PDF.js (pdf reader)
- 0.1.1
  - Support long sentence for TTS (text to speech)
  - Fix tooltip container arrow display error
  - Fix key hold error (issue on tab switching)
- 0.1.0   
  - First release

# Description
Mouse tooltip translator is a google chrome extension that focus on providing convenient translate experience for user. To achieve convenient translate experience, this translator extension minimize current generally required step to translate word in website. In modern days, copying and pasting are getting generalized to obtain translated sentence from google translate site. This extension uses text hovering event to decide which text is required to be translated for user. It automatically detects pointed area and it collect near words to group them as sentence for sentence translate service. This translator extension translate mouse pointed sentence text into user language text using any translator API like google translate and Bing translator. For providing direct translation, it displays given translated text with clean pop-over tooltip. User does not require any other more action for translate text. This extension process surely replaces general user translation action process which open new tab for using google translate to getting translated sentence.    
This extension is positioned between user and translator API (google translate and Bing translator) for providing simple translate experience with google translate service. When text translate is required, this translator extension request translate service for given text to google translate. Translator vendor communicates given text to provide its translated text to the extension. Then, this translator extension handles given translated text to display in popover tooltip format. Its translated text can be in any foreign text with google translate. Translator vendors provide multilingual translate service which support more than 100 language translate. In this translator extension’s popup setting page, supported translate language list is provide to user. User can select any translate language for google translate in this translator extension. Not only support google translate but also support Bing translator to give variety on user translate experience in this translator extension. Currently, this translator extension does not have any plan to support other translator like naver translate service, papago (파파고) translator, deepl and yandex translator. DeepL and Papago translator API are payment requirement service to use. This free serviced tooltip translator does not have any handling way to deal with payment on translate service for papago translator and DeepL.    
In this translator extension, user does not require a process to select source translate language for translate because this extension handle language detection feature based on google translate language detection. This translator extension sends its mouse pointed text data to google translate and receive translated text with language detection data at the same time. Google translate provide detected language type of given text and its translated text in one json format data. This translator extension handles its auto language detection feature which provide ease on user to minimize user interaction on source language selection for translate. Most of web site text does not require to provide source language selection to determine language to translate. This translator extension uses google auto language detection feature to automatically understand its source language to translate correctly with google translate. User can use this feature by select “auto” in this translator extension’s pop-up configuration page. If user want to use google translate in specified source language translate service, this translator extension provides source language selection on configuration page to select to use google translate in any language.    
Auto language detection is used to filter out user known language text to prevent tooltip translate for providing clear web site experience. This translator extension use google translate to detect same source target language to decide display translated tooltip or not. Main reason to filter out is to not disrupt on web site experience because same type of language situation does not give much difference on translate result. If there is no filter out, user known language tooltip will be displayed every time which may cause eye fatigue. For this reason, this translator extension detects language type of mouse over text to prevent translate service on same type of language.    
For supporting translate feature, this translator extension provides feature that spoke source text pronunciation using google TTS (text to speech). It handles google TTS (text to speech) to speak pointed text to user to listen its voice. To using this feature, user need to enable TTS (text to speech) feature from pop up configuration page. This translator extension uses google TTS (text to speech) to speak original text based on computer voice to give user to have an idea on how to pronounce its text. With this translator extension, any language learner student can enhance pronunciation skill by listening this translator extension’s google TTS (text to speech) speech voice.   
Mouse tooltip translator is individual developer’s created extension that is not officially made by google. It just handles google translate and google text to speech service to give ease translate experience to user. This translator extension does not own google translate and Bing translator. Google translate is owned by google and Bing translator is owned by Microsoft. This translator extension handles Google’s provided google translate service to user without any profit. Main purpose of this translator extension gives free translate experience on any web site without include any advertisement for show only translate result. This translator extension provides simple tooltip translate service on anywhere include YouTube, pdf and any text web site.    
This translator extension is open-source project in MIT license. Any developer can read its main translate functionality in the GitHub. This does not inject google analytics code in this translator extension. This translator extension respect user privacy but user need to keep in mind that it sends hovering text to google translate for translate purpose. It uses any usage data only for google translate (and google text to speech) purpose. This translator extension does not share its usage data with any other third parties.    
To give clear translate experience, this translator uses customized bootstrap framework to show translate result on tooltip. It uses tooltip as main core communication feature between user and google translate. In the tooltip, it only displays translate result to make focus on its translate result without any disruption by additional information display. This translator tooltip considers tiredness on eyes by minimizing on information overflow between communication with google translate. It only focus on translate result to support user productivity on web page reading for any language. This translator extension is not designed as dictionary for any additional display feature like word pronunciation.
This translator extension’s use case can be in any field. Education can be one of filed to use this mouse tooltip translator. With this translator extension, any language learner can easily get translate result with google translate to enhance knowledge of other languages. User can directly compare source text and translate result. This translate result comparison encourage user to memorize its pair in mind smoothly. This translate result comparison education can be applied on any user concerning contents like novel and news article. User does not required to read boring language text book anymore. User can directly interact translate result on user interesting novel to enhance skill more effectively.  
Built-in PDF viewer is contained in this translator extension. Mouse tooltip translator uses PDF.js as built-in PDF viewer to support pdf file to provide translate feature over pdf text. This translator extension’s pdf supporting feature give a possibility to user to read foreign essay paper with translate service. This translator extension does not use chrome pdf reader. Chrome pdf reader provide pdf as embed text format which has difficulty on text crawling process for translate with this translator extension. This translator extension intercept pdf URL and redirect to mouse tooltip pdf.js page to provide pdf reader with tooltip translate feature. Local pdf file is also supported when user give local URL permission to this translator extension.    
Currently, this translator extension has under development OCR feature to translate image text. Mouse tooltip translator’s OCR feature is turned off initially. To use OCR feature, user need to turn on “enable OCR”. When user mouse over on manga bubble background, this translator extension uses bucket brush method to mask out that positioned bubble to process OCR using tesseract.js to get its text for translate manga. If selected comic bubble background is not correctly separated from outside bubble with line, this translator extension's bucket brush method will mask out all page which give fail OCR result.    