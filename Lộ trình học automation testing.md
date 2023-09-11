# Learning roadmap for studying automation test
## Summary
Automation testing aims to improve testing efficiency, accuracy, and speed by automating repetitive and time-consuming manual testing tasks. Automation testing or test automation uses open source or paid automated testing tools to test software applications quickly and efficiently, and 24/7 without human intervention.

## What we need to do
1. Master knowledge of manual testing
2. Understand about Xpath
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

## 3. Learn as much as posible development language
To support scripting on test tools like Java/ C#/ Python/ Ruby/ Javascript/ Groovy... This is an extremely important part if you want to excel and advance in the career of an Automation Tester.\

In automation testing, HTML and Java are pivotal components that work together seamlessly to create efficient and robust test scripts. HTML is utilized to structure and define the elements of the web page under test, including buttons, forms, and other interactive elements. Java, as a programming language, offers the versatility needed to write and execute automated test scripts effectively. With libraries and frameworks like Selenium WebDriver, testers can harness the power of Java to interact with HTML elements, simulate user actions, and validate expected behaviors. This synergy between HTML and Java enables automation testers to build comprehensive test suites, perform regression testing, and ensure the reliability and functionality of web applications, contributing to improved software quality and faster release cycles.

List website for increase coding logic
- [Codelearn](https://codelearn.io/learning)
- [Howkteam](https://howkteam.vn/learn)
- [Hiepsiit](https://hiepsiit.com/)

## 4. Learn and apply coding, IDE, git, extension
- Coding convention:
> Coding standards are typically recognized and used by a group of developers to share code consistently. A common example of a coding standard is a set of conventions applied in the documentation of a programming language. For instance, languages like C have the K&R standard, Microsoft has coding standards for C#, and Oracle provides standards for Java, among others...

**General rules for writing 'clean' code:**
1. Think simple and write the simplest code possible.
2. Always keep the code cleaner than when you first received it, whether it's your own or someone else's.
3. Always identify the root cause of the problem.

**Naming Conventions**
1. The way you name identifiers (including variables, constants, classes, etc.) significantly affects code readability. Imagine a massive software like Windows, but every function is named something like 'a,' 'b,' 'c,' 'function1,' 'function2,'... Managing and maintaining such code would undoubtedly be extremely challenging.
2. There are three common naming conventions: camelCase, PascalCase, and snake_case. Specifically:\
<span class="highlight-text">Camel case</span>: The first letter of each word is lowercase, and the rest of the letters are uppercase. This convention is applied to function names, variable names, and method names. For example: firstName, lastName, getName(), findMember(),...\
<span class="highlight-text">Pascal case</span>`: The first letter of each word is capitalized, commonly used for class names or variable names. For example: MickeyMouse, FirstName,...\
<span class="highlight-text">Snake case</span>: All letters are lowercase, separated by underscores ('_'). This convention is often used for constants or program names. For example: program_final, get_max(),...

3. Some general rules for naming:\
- Name identifiers descriptively, reflecting their true functionality.
- Avoid using abbreviations in names.
- Class and variable names often use nouns.
- Function names typically use verbs.
- Avoid using magic numbers (directly using numbers in code) and instead, give them meaningful names. For example:
```
// ❌
if (gender === 0) { }
else if (gender === 1) { }
else { }

// ✅
const MALE = 0;
const FEMALE = 1;

if (gender === MALE) { }
else if (gender === FEMALE) { }
else { }
```

**Quantity Rules**\
Some quantity rules from the book 'Clean Code: A Handbook of Agile Software Craftsmanship' by Robert C. Martin, the book 'Refactoring in Large Software Projects: Performing Complex Restructurings Successfully' by Martin Lippert, and Oracle's coding standards include the following:

- A single line of code should not exceed 80 characters.
- A statement should be nested no more than 4 levels deep.
- A function should not have more than 5 parameters.
- A function should not exceed 30 lines.
- A class should not surpass 500 lines.
- Each function should perform only one task. If it serves two different purposes, the function name should clearly indicate this. For example: `increaseDownloadCounterAndSaveToDatabase`.

**Line Break Rules**\
According to Oracle's coding standards:

- If a function has multiple nested levels, each level should be indented with a line break.
- Code blocks at the same level should be aligned in the same column, and line breaks should start at the same level as the line above.
- Line breaks should occur before operators (such as +, -, *, ?, ...).



<style>
    .highlight-text {
        color: #64CCC5
    }
</style>