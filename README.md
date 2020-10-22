**Base_url:** https://www.qa.ebay.com/
### Search Page
https://www.qa.ebay.com/sch/i.html?_from=R40&_trksid=p2380057.m570.l1313&_nkw=ipad&_sacat=0                    
WebElement         | Syntax   | Xpath Expression|
------------- | -------------   | -------------------------
[search_box](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/search_box.png)  | `//tagname[@attributername='attributevalue']` |`//input[@class='gh-tb ui-autocomplete-input']`|
[Best_Match_Drop_Down](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Best_Match_Drop_Down.png)  | `//tagName[@class='classname']//child::tagname[text()="matchedtext"]`    | `//span[@class='expand-btn__cell']//child::span[text()="Best Match"]` |
[search_button](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Search_Button.png)| `//tagName[@attribute-name='attribute-value' and @attribute-name='attribute-value']` |`//input[@type='submit' and @value='Search']`|
[select_category_dropdown](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Select_categoty.png)| `//tagName[contains(@attribute-name,'attribute-value')]` | `//select[contains(@aria-label,'category')]`|
[shop_by_category_button](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Shop_By_category.png)| `//tagName[@attribute-name='attribute-value' and text()='Matching String'`| `//button[@id='gh-shop-a' and text()='Shop by category']`
[Model_categories_left_nav](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Model_category.png)| `class name = x-refine__left__nav` | some
[Guranteed_3_day_delivery_toggle](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Guranteed_3_day_delivery_toggle.png) | `//tagName[@attribute-name='attribute-value']//descendant::tagName[indexNumber]` | `//span[@class='guaranteed-delivery__switch']//descendant::span[1]`
[Favourites](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Favourites.png)|`//tagName[@id='idNumber']/button`| `//span[@id='s0-14-11-6-3-listing1-item-1-1-16-0']/button`
[Accept_Offers](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Accept_Offers.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='Accepts Offers']`
[All_Listings](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/All_Listings.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='All Listings']`
[Auction](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Auction.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='Auction']`
[Buy_it_now](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Buy_it_now.png)|`//tagName[@class='className' and text()='matching text']`|`//h2[@class='srp-format-tabs-h2' and text()='Buy It Now']`
[Condition](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Condition.png)|`//tagName[@class='className']//child::tagName/tagName[text()='matching text']`|`//button[@class='fake-menu-button__button expand-btn expand-btn--small expand-btn--secondary']//child::span/span[text()='Condition']`
[DeliveryOptions](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/DeliveryOptions.png)|`//tagName[@class='className']//child::tagName/tagName[text()='matching text']`|`//button[@class='fake-menu-button__button expand-btn expand-btn--small expand-btn--secondary']//child::span/span[text()='Delivery Options']`

  
### Tips and tricks
1. Attribute name will always start with `@` symbol. Example: `//input[@type='submit' and @value='Search']`

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

# CSS selectors

# Search WebElemnts using Search option in Chrome DevTools 
1. If you know a unique ID press `cmd+f` and search for that specific ID `#gh-ac`. ID has to be prefixed with `#`
2. Copy paste an xpath in the search bar to locate the weblement

# How to visualize Html as a tree?
1. Chrome extension [HTML Tree Generator](https://chrome.google.com/webstore/detail/html-tree-generator/dlbbmhhaadfnbbdnjalilhdakfmiffeg) can be used to view Html as a tree


# References
- [Xpath Guide](https://www.lambdatest.com/blog/complete-guide-for-using-xpath-in-selenium-with-examples/)
- [Cheat Sheet](https://devhints.io/xpath)
- [HTML DOM Tree Terminologies Tutorial](https://www.youtube.com/watch?v=N1Pe-wBtmx4)

