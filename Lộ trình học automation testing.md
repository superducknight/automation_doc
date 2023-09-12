# Learning roadmap for studying automation test
## Summary
Automation testing aims to improve testing efficiency, accuracy, and speed by automating repetitive and time-consuming manual testing tasks. Automation testing or test automation uses open source or paid automated testing tools to test software applications quickly and efficiently, and 24/7 without human intervention.

## What we need to do
1. [Master knowledge of manual testing](#1-master-knowledge-of-manual-testing)
2. [Understand about Xpath](#2-understand-about-html-css-and-xpath)
3. [Learn as much as posible development language](#3-learn-as-much-as-posible-development-language)
4. [Learn and apply coding, IDE, git, extension](#4-learn-and-apply-coding-ide-git-extension)
5. [Learn and use the supported automation library](#)
6. [Build, run and maintain Framework Testing with Page Object Model](#)
7. [Learn about Software design pattern](#)
8. [Using all above knowledge applied for workspace](#)

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
To support scripting on test tools like Java/ C#/ Python/ Ruby/ Javascript/ Groovy... This is an extremely important part if you want to excel and advance in the career of an Automation Tester.

In automation testing, HTML and Java are pivotal components that work together seamlessly to create efficient and robust test scripts. HTML is utilized to structure and define the elements of the web page under test, including buttons, forms, and other interactive elements. Java, as a programming language, offers the versatility needed to write and execute automated test scripts effectively. With libraries and frameworks like Selenium WebDriver, testers can harness the power of Java to interact with HTML elements, simulate user actions, and validate expected behaviors. This synergy between HTML and Java enables automation testers to build comprehensive test suites, perform regression testing, and ensure the reliability and functionality of web applications, contributing to improved software quality and faster release cycles.

List website for increase coding logic
- [Codelearn](https://codelearn.io/learning)
- [Howkteam](https://howkteam.vn/learn)
- [Hiepsiit](https://hiepsiit.com/)

## 4. Learn and apply coding, IDE, git, extension
### Coding convention:
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

3. Some general rules for naming:
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

### Git
- Git is a distributed version control system used in software development to track changes in source code. It enables multiple developers to work on the same project simultaneously by maintaining a history of code changes. Key features include branching for parallel development, merging and rebasing to integrate changes, commits to record snapshots of the code, and remote repositories for collaboration. Git is essential for efficient code management, history tracking, and team collaboration in software development projects.

- SSH, which stands for Secure Shell, is a network protocol and cryptographic technology used for secure communication over a potentially unsecured network, such as the internet. SSH is primarily used for two main purposes:

    - **`Remote Login`**: SSH allows users to log into and access a remote computer or server over a network. It provides a secure way to authenticate and establish a secure connection, preventing unauthorized access to sensitive systems. Users can execute commands, transfer files, and manage remote systems securely using SSH.

    - **`Secure File Transfer`**: SSH also facilitates secure file transfer between computers. Tools like SCP (Secure Copy Protocol) and SFTP (Secure File Transfer Protocol) use SSH as the underlying protocol to ensure that files are transferred securely and confidentially.

- Git uses ssh to communicate, contribute and manage the source code on remote origin of Github or Gitlab

- Create SSH key
1. Download [Git](https://git-scm.com/downloads)
2. Install Git into local machine
3. After installed Git. Open it and create a new ssh key
```
$ ssh-keygen -t rsa -C "your_account@thebank.vn"
```
This creates a new SSH key, using the provided email as a label.
```
> Generating public/private ALGORITHM key pair.
```
When you're prompted to "Enter a file in which to save the key", you can press Enter to accept the default file location.
```
> Enter a file in which to save the key (/c/Users/YOU/.ssh/id_ALGORITHM):[Press enter]
> Enter passphrase (empty for no passphrase): [Press enter]
> Enter same passphrase again: [Press enter]
```
4. Adding your SSH key to the ssh-agent
Start a new `ssh-agent`
```
$ eval "$(ssh-agent -s)"
> Agent pid 59566
```
Add your SSH private key to the ssh-agent.
```
ssh-add ~/.ssh/id_rsa
```
5. Add the SSH public key to your account on GitHub\
- In local machine, open `C:\Users\[user name](Admin)\.ssh\`
- Open file `id_rsa.pub` by Notepad or Notepad++ or Vscode
- Copy all text in this file
- Open [github](https://github.com/)
- Create or sign in account
- On the top right of the screen (profile image), click open the right side-bar, click on Setting
- On the left side-bar menu, click on `SSH and GPG keys`
- Click on <span class="green-btn">New SSH key</span>
- Input `Title` and paste all text from `id_rsa.pub` into field `Key`
- Click button <span class="green-btn">New SSH key</span>

### IDE
1. Open repo git
2. Click to <span class="green-btn"><> Code</span>
3. Choose SSH and copy
4. Download [VScode](https://code.visualstudio.com/download)
5. Install vscode
6. Open vscode and open terminal then type
```
git clone git@github.com:repo/project.git (paste which copied) [Press enter]
```

### Work with source code
1. Pull new everything from remote main/master
```
git pull origin main/master
```
2. Create new branch from main/master
```
git checkout -b <branch name>
```
3. Code, contribute or maintain source code
4. Add changes to stage
```
git add <related path file> || git add . (for add all file changed)
```
5. Commit code
```
git commit -m "message"
```
Note: Make sure message clear and convey the information of what is coded, message convention is `<name> creates/updates/fixes <something>`

6. Pull new everything from fast-forward main/master
```
git pull origin main/master
```
7. Push own new code into remote origin branch
```
git push origin <branch name>
```



<style>
    .highlight-text {
        color: #64CCC5
    }
    .green-btn {
        color: #66FF99
    }
    h3 {
        color: orchid
    }
</style>