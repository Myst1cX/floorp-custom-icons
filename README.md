## CUSTOM ICONS 

1. Custom Floorp Browser Icon (available in both original PNG and converted ICO file)
2. Custom Sidebar Icons (Google Translate, ChatGPT, Github)

1. Use ResourceHacker to apply the Custom Floorp Browser Icon (https://www.wikihow.com/Change-the-Icon-for-an-Exe-File)
2. AppData\Roaming\Floorp\Profiles\your-release\chrome > userChrome.css > Paste the following code:

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
