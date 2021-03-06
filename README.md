  # Table of contents
----------------------------------------------------------------------------------------------------------------------------
1. [Located Search Page using Xpath](https://github.com/priya006/WebElement_Locator#eyes-located-search-page-using-xpath-eyes)
2. [Located Checkout Page using CSS Selectors](https://github.com/priya006/WebElement_Locator#money_mouth_face-located-checkout-page-using-css-selectors-money_mouth_face)
3. [Tips and tricks](#money_with_wings-tips-and-tricks-bonus-money_with_wings)
4. [Tool to find Xpath](#tool-to-find-xpath)
5. [Use Html do in chrome devtools console to find webelements](#use-html-dom-in-chrome-devtools-console-to-find-webelement)
6. [How to use jQuery in chrome devtools console to write xpath](#how-to-use-jquery-in-chrome-devtools-console-to-write-xpath)
7. [Search webelements using ](#search-webelements-using-search-option-in-chrome-devtools)
8. [How to visualize html as a tree](#how-to-visualize-html-as-a-tree)
9. [Differences between CSS selectors and xpath](#differences-between-css-selectors-and-xpath)
10. [References](#references)

### :eyes: Located Search Page using Xpath :eyes:
**base_url**  https://www.ebay.com/                    
WebElement         | Syntax   | Xpath Expression|
------------- | -------------   | -------------------------
[search_box](https://github.com/priya006/WebElement_Locator/blob/master/Images/search_box.png)  | `//tagname[@attributername='attributevalue']` |`//input[@class='gh-tb ui-autocomplete-input']`|
[Best_Match_Drop_Down](https://github.com/priya006/WebElement_Locator/blob/master/Images/Best_Match_Drop_Down.png)  | `//tagName[@class='classname']//child::tagname[text()="matchedtext"]`    | `//span[@class='expand-btn__cell']//child::span[text()="Best Match"]` |
[search_button](https://github.com/priya006/WebElement_Locator/blob/master/Images/Search_Button.png)| `//tagName[@attribute-name='attribute-value' and @attribute-name='attribute-value']` |`//input[@type='submit' and @value='Search']`|
[select_category_dropdown](https://github.com/priya006/WebElement_Locator/blob/master/Images/Select_categoty.png)| `//tagName[contains(@attribute-name,'attribute-value')]` | `//select[contains(@aria-label,'category')]`|
[shop_by_category_button](https://github.com/priya006/WebElement_Locator/blob/master/Images/Shop_By_category.png)| `//tagName[@attribute-name='attribute-value' and text()='Matching String'`| `//button[@id='gh-shop-a' and text()='Shop by category']`|
[Model_categories_left_nav](https://github.com/priya006/WebElement_Locator/blob/master/Images/Model_category.png)| `class name = x-refine__left__nav` | some|
[Guranteed_3_day_delivery_toggle](https://github.com/priya006/WebElement_Locator/blob/master/Images/Guranteed_3_day_delivery_toggle.png) | `//tagName[@attribute-name='attribute-value']//descendant::tagName[indexNumber]` | `//span[@class='guaranteed-delivery__switch']//descendant::span[1]`|
[Favourites](https://github.com/priya006/WebElement_Locator/blob/master/Images/Favourites.png)|`//tagName[@id='idNumber']/button`| `//span[@id='s0-14-11-6-3-listing1-item-1-1-16-0']/button`|
[Accept_Offers](https://github.com/priya006/WebElement_Locator/blob/master/Images/Accept_Offers.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='Accepts Offers']`|
[All_Listings](https://github.com/priya006/WebElement_Locator/blob/master/Images/All_Listings.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='All Listings']`|
[Auction](https://github.com/priya006/WebElement_Locator/blob/master/Images/Auction.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='Auction']`|
[Buy_it_now](https://github.com/priya006/WebElement_Locator/blob/master/Images/Buy_it_now.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='Buy It Now']`|
[Condition](https://github.com/priya006/WebElement_Locator/blob/master/Images/Condition.png)|`//tagName[@class='className']//child::tagName/tagName[text()='matching text']`|`//button[@class='fake-menu-button__button expand-btn expand-btn--small expand-btn--secondary']//child::span/span[text()='Condition']`|
[DeliveryOptions](https://github.com/priya006/WebElement_Locator/blob/master/Images/DeliveryOptions.png)|`//tagName[@class='className']//child::tagName/tagName[text()='matching text']`|`//button[@class='fake-menu-button__button expand-btn expand-btn--small expand-btn--secondary']//child::span/span[text()='Delivery Options']`|

### :money_mouth_face: Located Checkout Page using CSS Selectors :money_mouth_face:
**base_url**  https://www.ebay.com/

  WebElement         | Syntax   | CSS Selectors|
------------- | -------------   | -------------------------
[Shipping](https://github.com/priya006/WebElement_Locator/blob/master/Images/Shipping.png)|`tagName[attributeName='attributeValue'] > tagName:first-child`|`tr[data-test-id='SHIPPING'] > td:first-child`|
[Tax](https://github.com/priya006/WebElement_Locator/blob/master/Images/Tax.png)|`tagName[attributeName='attributeValue']>tagName:first-of-type>tagName:first-of-type`|`tr[data-test-id='SALES_TAX']>td:first-of-type>span:first-of-type`|
[Delivery](https://github.com/priya006/WebElement_Locator/blob/master/Images/Delivery.png)|`tagName.className`|`div.section-title`|
[Apply](https://github.com/priya006/WebElement_Locator/blob/master/Images/Apply.png)|`tagName.className>tagName.className:enabled`|`div.incentives-button>button.btn.btn--primary.btn--medium:enabled`|
[eBay_Money_Gurantee](https://github.com/priya006/WebElement_Locator/blob/master/Images/eBay_Money_Gurantee.png)|`tagName.className`|`div.ebay-money-back`|
[Learn_More](https://github.com/priya006/WebElement_Locator/blob/master/Images/Learn_More.png)|`tagName[attributeName*='substring'][attributeName*='substring'][target='MatchingString']`|`a[title*='Opens'][href*='paying-tax'][target='_blank']`|
[Privacy_Notice](https://github.com/priya006/WebElement_Locator/blob/master/Images/Privacy_Notice.png)|`tagName[attributeName~='substring'][attributeName*='substring'][attributeName='attributeValue]'`|`a[title~='Opens'][href*='privacy'][target='_blank']`|
[User_Agreement](https://github.com/priya006/WebElement_Locator/blob/master/Images/User_Agreement.png)|`tagName[attributeName*='substring'][attributeName*='substring']`|`a[title*='Opens'][href*='user-agreement.html']`|
[Show_payments](https://github.com/priya006/WebElement_Locator/blob/master/Images/Show_payments.png)|`tagName[attributeName='attributeValue']`|`a[data-test-id='SHOW_MORE']`|
[See_Details](https://github.com/priya006/WebElement_Locator/blob/master/Images/See_Details.png)|`.className NestedchildTag:nth-last-child(indexNo) > directchild`|`.text-center.buyer-protection div:nth-last-child(1) > a`|
[Review_item_and_shipping_Quantity](https://github.com/priya006/WebElement_Locator/blob/master/Images/Review_item_and_shipping_Quantity.png)|`tagName[attributeName^='starts-with-String']>directchild:first-child`|`select[id^='qty-BId']>option:first-child`|
[Enter_Code](https://github.com/priya006/WebElement_Locator/blob/master/Images/Enter_Code.png)|`tagName[attributeName='attributeValue']+tagName > DirecChildTag[attributeName='attributeValue']`|`label[for='redemptionCode']+div > input[name='redemptionCode']`|
[Ship_to](https://github.com/priya006/WebElement_Locator/blob/master/Images/Ship_to.png)|`tagName.className > directchild > directchild tagType:nth-child(indexno)`|`h2.module-title > span > span span:nth-child(1)`|
[Confirm_and_pay](https://github.com/priya006/WebElement_Locator/blob/master/Images/Confirm_and_pay.png)|`#id_value > directchild > directchild > directchild`|`#page-form > div > button > span`|



### :money_with_wings: Tips and tricks [BONUS] :money_with_wings:
-----------------------------------------------------------------
1. Attribute name will always start with `@` symbol. Example: `//input[@type='submit' and @value='Search']`
2. It is a good practice to analyze Html code first before jumping into writting WebElement locators :thinking:

# Tool to find Xpath
1. Chrome Extension [SelectorsHub](https://chrome.google.com/webstore/detail/selectorshub/ndgimibanhlabgdgjcpbbndiehljcpfh/related?hl=en) can give us Xpath
![Selectors_hub](https://github.com/priya006/WebElement_Locator/blob/master/Images/Selectors_hub_new.gif)


# Use HTML DOM in Chrome DevTools Console to find WebElement
1. Find Webelement `document.getElementById("gh-ac")`
2. **ParentNode** of WebElement can be found like so `document.getElementById('gh-ac-box').parentNode.nodeName;`
3. **InnerText** of a WebElement can be found like so `var innerHtml = document.getElementsByClassName("srp-format-tabs-h2")[0].innerHTML;`
4. **First Child** could be found like so `document.getElementById('gh-ac-box').firstChild;`

# How to use JQuery in Chrome DevTools console to write Xpath?
1. Launch chrome browser Click `cmd+option+i` in mac OS. Chrome developer tool opens.
2. Click open `Console`
3. Type `$x("xpath")` Example: `$x("//input[@class='gh-tb ui-autocomplete-input']")`
4. From console right clicking takes you to [Element panel](https://github.com/priya006/WebElement_Locator/blob/master/Images/Chrome_console.gif)


# Search WebElements using Search option in Chrome DevTools 
1. If you know a unique ID press `cmd+f` and search for that specific ID `#gh-ac`. ID has to be prefixed with `#`
2. Copy paste an xpath in the search bar to locate the weblement

# How to visualize Html as a tree?
 Chrome extension [HTML Tree Generator](https://chrome.google.com/webstore/detail/html-tree-generator/dlbbmhhaadfnbbdnjalilhdakfmiffeg) can be used to view Html as a tree

# Differences Between CSS Selectors and Xpath
![Difference](https://github.com/priya006/WebElement_Locator/blob/master/Images/DifferencesBetweenXpathadnCSS.png)

# References
- [Xpath Guide](https://www.lambdatest.com/blog/complete-guide-for-using-xpath-in-selenium-with-examples/)
- [Cheat Sheet](https://devhints.io/xpath)
- [HTML DOM Tree Terminologies Tutorial](https://www.youtube.com/watch?v=N1Pe-wBtmx4)
- [CSS Selctors](https://saucelabs.com/resources/articles/selenium-tips-css-selectors)

