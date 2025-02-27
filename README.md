# Assisterr Daily Claimer
Autoclaim Daily Points for assisterr.ai support multiple accounts and using proxies.
## Tools and components required
1. Register: [https://build.assisterr.ai](https://build.assisterr.ai/?ref=677ac8bd0fed0714db3d6dc7) (Connect Twitter, Discord and complete tasks)
2. Proxies (OPTIONAL)
3. VPS or RDP (OPTIONAL), Get free $200 credit [DigitalOcean](https://m.do.co/c/3f132e0f7e13) for 60 days here: [Register](https://m.do.co/c/3f132e0f7e13)
4. NodeJS. How to install:
   - Linux users can go [here](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-22-04)
   - Windows users can go [here](https://www.youtube.com/watch?v=La6kH33-AVM&ab_channel=TheCodeCity)
   - Termux users can go [here](https://www.youtube.com/watch?v=5NceYSU4uFI&ab_channel=VectorM%3A)
### Buy Proxies
- Free Proxies Static Residental: 
   - [WebShare](https://www.webshare.io/?referral_code=p7k7whpdu2jg)
   - [ProxyScrape](https://proxyscrape.com/?ref=odk1mmj)
   - [MonoSans](https://github.com/monosans/proxy-list)
- Paid Premium Static Residental:
   - [922proxy](https://www.922proxy.com/register?inviter_code=d03d4fed)
   - [Proxy-Cheap](https://app.proxy-cheap.com/r/JysUiH)
   - [Infatica](https://dashboard.infatica.io/aff.php?aff=544)
## Credentials setup

### Getting Credentials
1. Get your Solana Wallet privatekey:
   - Use [Phantom Wallet](https://www.youtube.com/watch?v=xS5VllDRyMc)
   - Use [Soflare](https://www.youtube.com/watch?v=HYNKAhQjwLU). Then convert your Soflare privatekey using [this script](https://gist.github.com/im-hanzou/bb5569806875168b47458a56334bbe60).
3. Get account Tokens:
   - Open [https://build.assisterr.ai](https://build.assisterr.ai/?ref=677ac8bd0fed0714db3d6dc7) and make sure you already logged in and complete tasks. 
   - Open your browser's Developer Tools by press F12 or press Ctrl+Shift+I and navigate to the Console tab.
   - Run the following commands:
  ```bash
function getCookieValue(cookieName) {
    const cookies = document.cookie.split('; ');
    for (let cookie of cookies) {
        const [name, value] = cookie.split('=');
        if (name === cookieName) {
            return decodeURIComponent(value);
        }
    }
    return null
}
const accessToken = getCookieValue('accessToken');
const refreshToken = getCookieValue('refreshToken');
console.log('Access Token:', accessToken);
console.log('Refresh Token:', refreshToken);
  ```
3. Insert your credentials like this format to ``accounts.txt``:
```bash
accessToken:refreshToken:privatekey
```
>If you running multiple accounts just insert perlines
4. Insert proxies to ``proxies.txt`` like this format:
```bash
http://127.0.0.1:8080
http://user:pass@127.0.0.1:8080
```
>Only http proxies supported for now
## Modules Installation
- Download script [Manually](https://github.com/im-hanzou/assisterr-daily-claimer/archive/refs/heads/main.zip) or use git:
```bash
git clone https://github.com/im-hanzou/assisterr-daily-claimer
```
- Open terminal and make sure you already in bot folder:
```bash
cd assisterr-daily-claimer
```
- Install modules:
```bash
npm install
```
- Run bot:
```bash
node index.js
```
# Notes
- Run this bot, use my referrer code if you don't have one.
- You can just run this bot at your own risk, I'm not responsible for any loss or damage caused by this bot.
- This bot is for educational purposes only.
