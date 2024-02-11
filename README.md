# Rest-api

.env file value
```
#GOOGLE_AI
GOOGLE_AI_STUDIO_KEY=
#BARD
PSID_TOKEN=
PSIDTS_TOKEN=
#Bing
BING_IMAGE_COOKIE=
BING_U_COOKIE=
#C.AI
CHARACTER_AI=
#SPOTIFY
SPOTIFY_ID=
SPOTIFY_SECRET=
#CHATGPT
REFRESH_TOKEN=
WRTN_ID=
WRTN_EMAIL=
#SERVER
auth_enabled=false
authkey=0000
PORT=
```


<h1>Setting Up</h1>
 <details>
 <summary>Bard</summary>
 1. Open incognito and head to https://bard.google.com<br>
 2. Login using your desired google account<br>
 3. Now head to https://google.com<br>
 4. Open developer tools (<kbd>F12</kbd>, <kbd>Ctrl+Shift+I</kbd>, or <kbd>Cmd+J</kbd>) and click the cookies tab<br>
 5. Find __Secure-1PSID and  __Secure-1PSIDTS into the env variable<br><br>
Example: <br>
PSID_TOKEN= __Secure-1PSID COOKIE <br>
PSIDTS_TOKEN= __Secure-1PSIDTS COOKIE <br>
 </details>
 <details>
 <summary>Gemini</summary>
 1. Head to https://makersuite.google.com/app/apikey
 2. Login using your google account
 3. Done!
 </details>
  <summary>ChatGPT</summary>
 1. Head to https://wrtn.ai
 2. Login using your google account
 3. paste this code to ur console
 ```const c = JSON.parse(document.querySelector("#__NEXT_DATA__").textContent).props.pageProps;
if (c.isAuth){ 
    console.log()
 console.log(`REFRESH_TOKEN=${(await cookieStore.get("refresh_token")).value}\nWRTN_ID=${c["fallback"]["/user"]["meta"]["__w_id"]}\nWRTN_EMAIL=${c["fallback"]["/user"]["email"]}`)
}else{
    alert("Login first ");
}```
4. Done!
 </details>