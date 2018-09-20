[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/SASAICAGENCY) [![](https://data.jsdelivr.com/v1/package/gh/AmauriC/tarteaucitron.js/badge)](https://www.jsdelivr.com/package/gh/AmauriC/tarteaucitron.js)



tarteaucitron.js
================
Comply to the european cookie law is simple with the french *tarte au citron*.

# What is this script?
The european cookie law regulates the management of cookies and you should ask your visitors their consent before exposing them to third party services.

Clearly this script will:
- Disable all services by default,
- Display a banner on the first page view and a small one on other pages,
- Display a panel to allow or deny each services one by one,
- Activate services on the second page view if not denied,
- Store the consent in a cookie for 365 days.

Bonus:
- Load service when user click on Allow (without reload of the page),
- Incorporate a fallback system (display a link instead of social button and a static banner instead of advertising).


# Installation guide
[Visit opt-out.ferank.eu](https://opt-out.ferank.eu/)


# How to use

```html
<script type="text/javascript" src="/tarteaucitron/tarteaucitron.js"></script>

<script type="text/javascript">
tarteaucitron.init({
    "privacyUrl": "", /* Privacy policy url */

    "hashtag": "#tarteaucitron", /* Open the panel with this hashtag */
    "cookieName": "tartaucitron", /* Cookie name */
    
    "orientation": "top", /* Banner position (top - bottom) */
    "showAlertSmall": true, /* Show the small banner on bottom right */
    "cookieslist": true, /* Show the cookie list */

    "adblocker": false, /* Show a Warning if an adblocker is detected */
    "AcceptAllCta" : true, /* Show the accept all button when highPrivacy on */
    "highPrivacy": false, /* Disable auto consent */
    "handleBrowserDNTRequest": false, /* If Do Not Track == 1, accept all */

    "removeCredit": false, /* Remove credit link */
    "moreInfoLink": true, /* Show more info link */

    //"cookieDomain": ".my-multisite-domaine.fr" /* Shared cookie for subdomain website */
});
</script>
```