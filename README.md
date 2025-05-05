## CUSTOM ICONS 

1. Custom Floorp Browser Icon (available in both original PNG and converted ICO file)
   
--> Use ResourceHacker to apply the Custom Floorp Browser Icon (https://www.wikihow.com/Change-the-Icon-for-an-Exe-File)
   
2. Custom Sidebar Icons to fix a few side panel icons that Floorp did not load correctly (Google Translate, ChatGPT, Github)

--> about:preferences#bSB > Use Icon Provider (DuckDuckGo)

--> Go to AppData\Roaming\Floorp\Profiles\your-release\chrome > userChrome.css > Paste the following code:

/* Custom sidebar icon for Syncthing Web UI */
.webpanel-icon[tooltiptext*="127.0.0.1:8384"] {
  --BMSIcon: url("http://127.0.0.1:8384/assets/img/favicon-default.png") !important;
}

/* Custom sidebar icon for Google Translate */
.webpanel-icon[tooltiptext*="translate.google.com"] {
  --BMSIcon: url("https://github.com/Myst1cX/floorp-custom-icons/raw/refs/heads/main/GoogleTranslate.ico") !important;
}

/* Custom sidebar icon for GitHub */
.webpanel-icon[tooltiptext*="github.com"] {
  --BMSIcon: url("https://github.com/Myst1cX/floorp-custom-icons/raw/refs/heads/main/Github.ico") !important;
}

/* Custom sidebar icon for ChatGPT */
.webpanel-icon[tooltiptext*="chatgpt.com"] {
  --BMSIcon: url("https://github.com/Myst1cX/floorp-custom-icons/raw/refs/heads/main/ChatGPT.ico") !important;
}

NOTE: To further customize, you can find icons at https://twenty-icons.com/ and https://iconarchive.com/
