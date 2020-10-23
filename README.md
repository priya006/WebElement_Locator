**Base_url:** https://www.qa.ebay.com/
### :eyes: Located Search Page using Xpath :eyes:
https://www.qa.ebay.com/sch/i.html?_from=R40&_trksid=p2380057.m570.l1313&_nkw=ipad&_sacat=0                    
WebElement         | Syntax   | Xpath Expression|
------------- | -------------   | -------------------------
[search_box](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/search_box.png)  | `//tagname[@attributername='attributevalue']` |`//input[@class='gh-tb ui-autocomplete-input']`|
[Best_Match_Drop_Down](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Best_Match_Drop_Down.png)  | `//tagName[@class='classname']//child::tagname[text()="matchedtext"]`    | `//span[@class='expand-btn__cell']//child::span[text()="Best Match"]` |
[search_button](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Search_Button.png)| `//tagName[@attribute-name='attribute-value' and @attribute-name='attribute-value']` |`//input[@type='submit' and @value='Search']`|
[select_category_dropdown](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Select_categoty.png)| `//tagName[contains(@attribute-name,'attribute-value')]` | `//select[contains(@aria-label,'category')]`|
[shop_by_category_button](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Shop_By_category.png)| `//tagName[@attribute-name='attribute-value' and text()='Matching String'`| `//button[@id='gh-shop-a' and text()='Shop by category']`|
[Model_categories_left_nav](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Model_category.png)| `class name = x-refine__left__nav` | some|
[Guranteed_3_day_delivery_toggle](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Guranteed_3_day_delivery_toggle.png) | `//tagName[@attribute-name='attribute-value']//descendant::tagName[indexNumber]` | `//span[@class='guaranteed-delivery__switch']//descendant::span[1]`|
[Favourites](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Favourites.png)|`//tagName[@id='idNumber']/button`| `//span[@id='s0-14-11-6-3-listing1-item-1-1-16-0']/button`|
[Accept_Offers](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Accept_Offers.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='Accepts Offers']`|
[All_Listings](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/All_Listings.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='All Listings']`|
[Auction](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Auction.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='Auction']`|
[Buy_it_now](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Buy_it_now.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='Buy It Now']`|
[Condition](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Condition.png)|`//tagName[@class='className']//child::tagName/tagName[text()='matching text']`|`//button[@class='fake-menu-button__button expand-btn expand-btn--small expand-btn--secondary']//child::span/span[text()='Condition']`|
[DeliveryOptions](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/DeliveryOptions.png)|`//tagName[@class='className']//child::tagName/tagName[text()='matching text']`|`//button[@class='fake-menu-button__button expand-btn expand-btn--small expand-btn--secondary']//child::span/span[text()='Delivery Options']`|

### :money_mouth_face: Located Checkout Page using CSS Selectors :money_mouth_face:
https://pay.qa.ebay.com/rxo?action=view&sessionid=6791754017

  WebElement         | Syntax   | CSS Selectors|
------------- | -------------   | -------------------------
[Shipping](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Shipping.png)|syntax|div a|
[Tax](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Tax.png)|syntax|div a|
[Delivery](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Delivery.png)|syntax|div a|
[Apply](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Apply.png)|syntax|div a|
[eBay_Money_Gurantee](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/eBay_Money_Gurantee.png)|syntax|div a|
[Learn_More](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Learn_More.png)|syntax|div a|
[Privacy_Notice](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Privacy_Notice.png)|syntax|div a|
[User_Agreement](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/User_Agreement.png)|syntax|div a|
[Show_payments](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Show_payments.png)|syntax|div a|
[See_Details](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/See_Details.png)|syntax|div a|
[Review_item_and_shipping_Quantity](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Review_item_and_shipping_Quantity.png)|syntax|div a|
[Enter_Code](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Enter_Code.png)|syntax|div a|
[Ship_to](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Ship_to.png)|syntax|div a|
[Confirm_and_pay](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/Confirm_and_pay.png)|`#id_value > directchild > directchild > directchild`|`#page-form > div > button > span`|



### :money_with_wings: Tips and tricks [BONUS] :money_with_wings:
-----------------------------------------------------------------
1. Attribute name will always start with `@` symbol. Example: `//input[@type='submit' and @value='Search']`
2. It is a good practice to analyze Html code first before jumping into writting WebElement locators :thinking:

# Tool to find Xpath
1. Chrome Extension [SelectorsHub](https://chrome.google.com/webstore/detail/selectorshub/ndgimibanhlabgdgjcpbbndiehljcpfh/related?hl=en) can give us Xpath
![Selectors_hub](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Selectorshub.gif)


# Use HTML DOM in Chrome DevTools Console to find WebElement
1. Find Webelement `document.getElementById("gh-ac")`
2. **ParentNode** of WebElement can be found like so `document.getElementById('gh-ac-box').parentNode.nodeName;`
3. **InnerText** of a WebElement can be found like so `var innerHtml = document.getElementsByClassName("srp-format-tabs-h2")[0].innerHTML;`
4. **First Child** could be found like so `document.getElementById('gh-ac-box').firstChild;`

# How to use JQuery in Chrome DevTools console to write Xpath?
1. Launch chrome browser Click `cmd+option+i` in mac OS. Chrome developer tool opens.
2. Click open `Console`
3. Type `$x("xpath")` Example: `$x("//input[@class='gh-tb ui-autocomplete-input']")`
4. From console right clicking takes you to [Element panel](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Chrome_console.gif)


# Search WebElements using Search option in Chrome DevTools 
1. If you know a unique ID press `cmd+f` and search for that specific ID `#gh-ac`. ID has to be prefixed with `#`
2. Copy paste an xpath in the search bar to locate the weblement

# How to visualize Html as a tree?
 Chrome extension [HTML Tree Generator](https://chrome.google.com/webstore/detail/html-tree-generator/dlbbmhhaadfnbbdnjalilhdakfmiffeg) can be used to view Html as a tree

# Differences Between CSS Selectors and Xpath
![Difference](https://github.corp.ebay.com/pboopathi/WebElement-Locator-PlayBook/blob/master/Images/DifferencesBetweenXpathadnCSS.png)

# References
- [Xpath Guide](https://www.lambdatest.com/blog/complete-guide-for-using-xpath-in-selenium-with-examples/)
- [Cheat Sheet](https://devhints.io/xpath)
- [HTML DOM Tree Terminologies Tutorial](https://www.youtube.com/watch?v=N1Pe-wBtmx4)
- [CSS Selctors](https://saucelabs.com/resources/articles/selenium-tips-css-selectors)

