
### 🚀 Speed Optimization & Front End Performance Tips for Adobe Commerce

Looking at your Lighthouse score can be quite disheartening if you're running an Adobe Commerce store. However, I've compiled some **proven methods for speed optimization** and front-end performance guaranteed to increase your Lighthouse scores. If you're looking to increase the front-end performance and speed optimization of an Adobe Commerce store, with an emphasis on Lighthouse scores, then start here:

***

### 💻 CSS Speed Optimization

* **Reduce unused CSS**: [https://developer.chrome.com/en/docs/lighthouse/performance/unused-css-rules/](https://developer.chrome.com/en/docs/lighthouse/performance/unused-css-rules/)
* **Merge CSS**: [https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/developer.html](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/developer.html)
* **Minify CSS**: [https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/developer.html](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/developer.html)
* **Enable Critical CSS**: [https://developer.adobe.com/commerce/frontend-core/guide/css/critical-path](https://developer.adobe.com/commerce/frontend-core/guide/css/critical-path)
* **Create unique Critical CSS per page**: [https://github.com/Joshua34/CriticalCSSPerPage](https://github.com/Joshua34/CriticalCSSPerPage)

***

### ⚡ JavaScript Speed Optimization

* *Fix any console errors*
* *Ensure all scripts are running the most up-to-date version*
* *Filter all scripts and GTM tags to run on an “as needed” basis only*
* **Minify JS**: [https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/developer.html](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/developer.html)
* **Move JS to the bottom of the page**: [https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/developer.html](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/developer.html)
* **As needed, exclude any critical scripts from being moved**: [https://magento.stackexchange.com/a/363633/5880](https://magento.stackexchange.com/a/363633/5880)
* **Install, generate, bundle, and enable MagePack**: [https://github.com/magesuite/magepack](https://github.com/magesuite/magepack)
* *Add `<link rel=”preload”>` to `<head>` for all generated magepack files*

***

### 🖼️ Image / Asset Speed Optimization

* *Check code for any duplicate calls to assets, scripts, fonts, etc.*
* *Remove any and all unused 3rd party modules, scripts, fonts*
* *Ensure all external resources are running the most up-to-date version*
* **Add Assets to CSP Whitelist**: [https://developer.adobe.com/commerce/php/development/security/content-security-policies/#configure-csps-for-your-custom-codeextensiontheme](https://developer.adobe.com/commerce/php/development/security/content-security-policies/#configure-csps-for-your-custom-codeextensiontheme)
* **Lazy load all below-the-fold images**: [https://developer.mozilla.org/en-US/docs/Web/Performance/Lazy_loading#images_and_iframes](https://developer.mozilla.org/en-US/docs/Web/Performance/Lazy_loading#images_and_iframes)
* **Add `<link rel=”preconnect”>` to `<head>` for any external critical assets**: [https://developer.chrome.com/en/docs/lighthouse/performance/uses-rel-preconnect/](https://developer.chrome.com/en/docs/lighthouse/performance/uses-rel-preconnect/)
* **Add `<link rel=”prefetch”>` (after browser idle) for anticipated resources**: [https://web.dev/link-prefetch/](https://web.dev/link-prefetch/)
* **Use http/2 delivery for all assets**: [https://www.cloudflare.com/learning/performance/http2-vs-http1.1/](https://www.cloudflare.com/learning/performance/http2-vs-http1.1/)
* **If using Cloudflare, enable WebP support**: [https://developers.cloudflare.com/images/polish/activate-polish](https://developers.cloudflare.com/images/polish/activate-polish)

***

### ⏱️ LCP Speed Optimization

* **Add `fetchpriority=”high”` to LCP element**: [https://web.dev/priority-hints/](https://web.dev/priority-hints/)
* **Add `<link rel=”preload”>` to `<head>` for LCP & all critical assets**: [https://web.dev/preload-critical-assets/](https://web.dev/preload-critical-assets/)
* **Filter any font libraries loaded, remove unused glyphs**: [https://web.dev/font-best-practices/](https://web.dev/font-best-practices/)
* **Add `<link rel=”preload”>` to `<head>` for all external fonts**: [https://web.dev/optimize-webfont-loading/](https://web.dev/optimize-webfont-loading/)

***

### ⚙️ Additional Speed Optimization

* *Cleanup site database*
* **Fix any HTML code errors**: [https://validator.w3.org/](https://validator.w3.org/)
* **Serve cached resources to visitors**: [https://developer.chrome.com/en/docs/lighthouse/performance/uses-long-cache-ttl/](https://developer.chrome.com/en/docs/lighthouse/performance/uses-long-cache-ttl/)
* **Install & configure Varnish**: [https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cache/varnish/config-varnish.html](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cache/varnish/config-varnish.html)
* **Run Magento in Production Mode**: [https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/setup/application-modes.html](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/setup/application-modes.html)

***

### Conclusion

Speed Optimization and Front End Performance is both an art and a science. Please note that each website’s front end will require some level of personalization and customization to get it right and meet its exact requirements. Because I used these points as a reference, it allowed me to improve my Lighthouse score from a 49 to a 96. With this in mind, I hope you can speed-optimize your site and improve the quality and speed of your user experience.
```
