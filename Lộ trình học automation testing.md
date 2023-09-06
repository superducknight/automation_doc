# Learning roadmap for studying automation test
## Summary
Automation testing aims to improve testing efficiency, accuracy, and speed by automating repetitive and time-consuming manual testing tasks. Automation testing or test automation uses open source or paid automated testing tools to test software applications quickly and efficiently, and 24/7 without human intervention.

## What we need to do
1. Master knowledge of manual testing
2. Understand about HTML, CSS and Xpath
3. Learn as much as posible development language
4. Learn and apply coding, IDE, git, extension
5. Learn and use the supported automation library
6. Build, run and maintain Framework Testing with Page Object Model
7. Learn about Software design pattern
8. Using all above knowledge applied for workspace

## 1. Master knowledge of manual testing
Fundamental knowledge in manual testing is of paramount importance in the software development process. It serves as the foundation upon which efficient and effective testing strategies are built. Manual testers armed with this knowledge can thoroughly understand the software's specifications and intricacies, allowing them to identify critical test scenarios and potential pitfalls that automated testing may miss. This expertise enables them to design comprehensive test cases, execute them meticulously, and provide valuable feedback to developers, contributing significantly to the overall quality of the software. Furthermore, manual testing knowledge empowers testers to adapt to evolving project requirements and unforeseen issues, ensuring that the software is robust, reliable, and meets the end-users' expectations.

## 2. Understand about HTML, CSS and Xpath
- XPath (XML Path Language) is a query language used for navigating and selecting elements from an XML document or an HTML page. It is particularly useful in web scraping and XML parsing, allowing you to locate specific elements or data within a structured document. XPath uses a path-like syntax to traverse the hierarchical structure of XML or HTML documents.

### **How XPath Works:**
XPath expressions are used to navigate the structure of an XML or HTML document, essentially forming a path from the root node to the desired element. The syntax is as follows:

**`//`**: This indicates that the search starts from the root node and traverses all descendants.\
**`element`**: Represents the name of the HTML or XML element to be selected.\
**`[@attribute='value']`**: Allows you to filter elements based on specific attributes and their values.\
**`[text()='text_value']`**: Enables the selection of elements based on their text content.\
**`[]`**: Square brackets are used to specify conditions or filters.

### **Basic XPath Expressions:**
*Selecting Elements by Attribute Value:*\
**`//input[@id='username']`**: Selects an `<input>` element with the attribute id set to 'username'.
**`//a[@href='/home']`**: Selects an `<a>` element with the attribute href set to '/home'.

*Selecting Elements by Text Content:*\
**`//h1[text()='Welcome']`**: Selects an `<h1>` element with the text content "Welcome".

*Selecting Elements by Partial Text:*\
**`//*[contains(text(), 'Login')]`**: Selects any element that contains the text "Login".

*Selecting Elements by Tag and Position:*\
**`(//div[@class='item'])[3]`**: Selects the third `<div>` element with the class 'item'.

*Selecting Elements by Ancestor:*\
**`//div[@class='container']//p`**: Selects all `<p>` elements inside a `<div>` with the class 'container'.

### **XPath relationship**
*Parent-Child Relationship:*\
**`/`**: The forward slash / represents the parent-child relationship. It is used to traverse from one element to its direct child element. For example: /parent/child selects the child element directly nested inside the parent.

*Descendant Relationship:*\
**`//`**: The double forward slash // represents the descendant relationship. It is used to traverse from one element to any nested descendant element, regardless of the depth of nesting. For example: //ancestor//descendant selects all descendant elements of the ancestor.

*Ancestor-Descendant Relationship:*\
**`/../`**: The .. notation represents the ancestor-descendant relationship. It allows you to traverse from one element to its parent element. For example: /parent/../another_parent selects the parent of the parent, effectively selecting another_parent.

*Sibling Relationship:*\
**`/following-sibling::`**: This allows you to select sibling elements that come after the current element. For example: /current/following-sibling::sibling selects all sibling elements that come after current.

*Preceding-Sibling Relationship:*\
**`/preceding-sibling::`**: This selects sibling elements that come before the current element. For example: /current/preceding-sibling::sibling selects all sibling elements that come before current.

*Attribute Relationship:*\
**`/@attribute_name`**: This notation is used to select the value of a specific attribute for the current element. For example: /element/@attribute_name selects the value of attribute_name for element.

### **Xpath axis**
**`Child Axis (child::)`**: This axis selects all the children of the current element. For example, /parent/child::element selects all element children of parent.

**`Parent Axis (parent::)`**: This axis selects the parent of the current element. For example, /child/parent::parent_element selects the parent_element that is the parent of child.

**`Attribute Axis (attribute::)`**: This axis selects the attributes of the current element. For example, /element/attribute::attribute_name selects the value of the attribute_name attribute of element.

**`Namespace Axis (namespace::)`**: This axis selects the namespaces associated with the current element. It is not commonly used in web scraping or testing.

**`Self Axis (self::)`**: This axis selects the current element itself. For example, /element/self::element selects the element itself.

**`Descendant Axis (descendant::)`**: This axis selects all descendants (children, grandchildren, etc.) of the current element. For example, /ancestor/descendant::element selects all element descendants of ancestor.

**`Ancestor Axis (ancestor::)`**: This axis selects all ancestors (parent, grandparent, etc.) of the current element. For example, /descendant/ancestor::ancestor_element selects the ancestor_element that is an ancestor of descendant.

**`Following-Sibling Axis (following-sibling::)`**: This axis selects all siblings that come after the current element. For example, /current/following-sibling::sibling selects all sibling elements that come after current.

**`Preceding-Sibling Axis (preceding-sibling::)`**: This axis selects all siblings that come before the current element. For example, /current/preceding-sibling::sibling selects all sibling elements that come before current.