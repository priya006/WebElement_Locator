**Base_url:** https://www.qa.ebay.com/
### Search Page
https://www.qa.ebay.com/sch/i.html?_from=R40&_trksid=p2380057.m570.l1313&_nkw=ipad&_sacat=0                    
WebElement         | Syntax   | Xpath Expression|
------------- | -------------   | -------------------------
[search_box](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/search_box.png)  | `//tagname[@attributername='attributevalue']` |`//input[@class='gh-tb ui-autocomplete-input']`|
[Best_Match_Drop_Down](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Best_Match_Drop_Down.png)  | //tagName[@class='classname']//child::tagname[text()="matchedtext"]    | //span[@class='expand-btn__cell']//child::span[text()="Best Match"] |
[search_button](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Search_Button.png)| //tagName[@attribute-name='attribute-value' and @attribute-name='attribute-value'] |//input[@type='submit' and @value='Search']|
[select_category_dropdown](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Select_categoty.png)| //tagName[contains(@attribute-name,'attribute-value')] | `//select[contains(@aria-label,'category')]`|
[shop_by_category_button](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Shop_By_category.png)| //xpath | some
[Model_categories_left_nav](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Model_category.png)| `class name = x-refine__left__nav` | some
[Guranteed_3_day_delivery_toggle](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Guranteed_3_day_delivery_toggle.png) | syntax | 
[Favourites](https://github.corp.ebay.com/pboopathi/Xpath-CheatSheet/blob/master/Images/Favourites.png)|syntax| xpath
  
# Tips and tricks
1. Attribute name will always start with `@` symbol. Example: `//input[@type='submit' and @value='Search']`

# jQuery HTML DOM


# References
- [Xpath Guide](https://www.lambdatest.com/blog/complete-guide-for-using-xpath-in-selenium-with-examples/)
- [Cheat Sheet](https://devhints.io/xpath)

