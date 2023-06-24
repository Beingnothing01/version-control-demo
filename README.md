# Why do we need Version Control - Git & Github

Version control is a crucial tool for managing changes to software projects and other collaborative endeavors. It allows multiple individuals to work on the same project simultaneously while keeping track of changes, coordinating efforts, and maintaining a history of revisions. 

## Here are some key reasons why version control is essential:

Here are some key reasons why version control is essential:

* **Collaboration**: Version control systems enable seamless collaboration among team members. It allows multiple developers to work on the same codebase concurrently, facilitating parallel development and reducing conflicts when merging changes.
* **Change tracking**: With version control, every modification made to files and code is tracked, providing a detailed history of changes. This feature is invaluable when investigating bugs, identifying the cause of issues, or reverting to a previous working state.
* **Branching and merging**: Version control systems enable branching, which allows developers to create independent lines of development. This feature is particularly useful when working on new features or experimenting with different approaches. Branches can be merged back together once the work is complete, ensuring a smooth integration of changes.
* **Code organization**: Version control helps maintain a structured and organized codebase. It allows developers to separate different features, bug fixes, and experiments into separate branches or commits, making it easier to manage and understand the project's evolution.
* **Rollback and recovery**: If a mistake is made or an undesirable change is committed, version control enables rollbacks. By reverting to a previous version, developers can undo the unwanted modifications and restore the project to a known, stable state.
* **Continuous integration and deployment**: Version control is often integrated with continuous integration and deployment (CI/CD) systems. This integration allows for automated testing, building, and deployment processes, ensuring that only well-tested and stable code is deployed to production environments.
* **Documentation and collaboration**: Version control systems typically include features like commit messages, comments, and annotations, allowing developers to document their changes, explain their thought process, and provide context to other team members. This documentation fosters better collaboration and knowledge sharing.
* **Traceability and accountability**: Version control provides traceability by attributing each change to a specific person, helping track who made what modifications. This accountability is valuable for project management, code reviews, and auditing purposes.


First, Install git https://git-scm.com/downloads and SignUp on Github

## Cloning global Github file, making changes locally and pushing to Github

* Step 1:
```git clone <github-clone-link>```  Eg. git clone "https://github.com/gwenf/vue3-fcc-course-basic-product-cart-demo.git"

* Step2:
Make changes in the cloned files.

* Step3:
Check the made changes using
```git status```

* Step 4:
Add the made changes using
```git add .```
or
```git add <filename>```

Again check the status using "git status"
Changes made will be reflected

* Step 5:
Now that you have made the changes, you need to push it on github to make it global.
But, for this step, you first need to create SSH key for making the Github verify your identity and allowing changes made.
Steps for creating SSH Key-->
  * Open new terminal.
```ssh-keygen -t rsa -b 4096 -C "yourEmailAddress@gmail.com"```
  * Give filename and password for storing the private and public key needed for authentication.
  * Now, go to the key files using, 
  ```ls | grep <filename>```
  * Open public key file .pub 
  * Copy paste the whole text in the .pub file into the Github--> Profile --> Settings --> SSH and GPG keys --> New SSH Key
  Give any title.

* Step 6:
Once the SSH Key is set, you can push the vhanges made globally using,
```git push```

On first git push, you will get option for downloading github authentication extension that will handle all the extra necessary setups required.

Finally, you have made your first push from your local machine to Github globally.



## Changing the file in local machine

Make changes
