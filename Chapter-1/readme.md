# React assignment

1. ## &nbsp; What is NPM?
      NPM is node package manager which is a remote repository for reusable code , our project can use that dependency to development faster and preetier along with customizing feature.

2. ## &nbsp; What is parcel / webpack?
      parcel / webpack is the bundler which

      - bundle the code by resolving dependency and transforming file to single in minified form
      where you have one file for each html , css , js.
      - remove all dead code which is imported but not used (tree shaking).
      - cached the code , if we made any changes and saved it make hot reloading without refresh.
      - create local dev server.
      - increased speed by hashing .
      - compress static file.
      - transpile the modern syntax to browser specifc language .
      - automatically it might compatible with older browser if it is in browser list.

3. ## &nbsp; What is .parcel-cache?
       
       it is a folder where you have all cached memozied data and it mapping file.

4. ## &nbsp; What is npx?
      npx is command which doesnot install package on machine , 
      instead it install -> execute package -> uninstall package 
      it can use when package execute many time on terminal or once in project.

5. ## &nbsp; What is dependency vs dev-dependency?
      dependency meaning - thing need in  development program.

      dependency - without that program will not run.
      example :  axios - must need to make api call to make communication between user and server.

      dev-dependency - it is like tool used for optimizing , organize , bug free program and also
      to increase speed of writing code.

      example : (jest , react library) - used for testing and create bug free code , 
      (nodemon) - if we made any changes and save server automatically restart (reduce time) ,
      (parcel)  - bundle the code into single file each those used in runtime.

6. ## &nbsp; What is Tree shaking?

    Tree shaking is a technique used in modern JavaScript development to eliminate unused or dead code (i.e., code that is not being used) from your application bundle. It helps reduce the size of the final JavaScript file, resulting in faster load times for web applications. Tree shaking is especially important when working with large JavaScript libraries and frameworks.

7. ## &nbsp; What is Hot module Replcement?
      if we made changes and save the code then local dev server is refresh automatically.

8. ## &nbsp; What is .gitignore file what we should add and what not to add?
      file, folder mention in .gitignore will remain untracked by git ,so it not push to the github.

      we should add all basic data which cannot retrive anywhere , example : package.json , .lock.json is need to track what package that our project used , we donot know which version , which package is installed and code will break.
      but we should not include node_modules because we can retrive from package.json by npm install command.
9. ## &nbsp; What is difference between package.json and package.lock.json?
       
       #### package.json:
           have version of package at time of first install in project , browser-list it need to support , and have annotation prior to version which indicate how much package can update if latest version release at time of install  existing package in package.json

       #### package.lock.json:
             have exact lock version of package after npm install is used (differ from package.json when try to install package from package.json when latest version is released) and also have
             dependency of dependency version, integrity to make sure same pacakge is install in production.

10. ## &nbsp; Why should i not modify package.lock.json?
             It is automatically generated and updated by the Node Package Manager (NPM) or Yarn when you install or update packages in your project.
             it has exact version , it only make consistency and integrity of dependency which used for dependency reslove.

11.  ## &nbsp; what is node_modules , should i push to github?
          It is folder has code of depedency we install , it also have dependency of dependecy and keep goes on untill that code doesnot use any package to build it.

          node_modules can be retrive from package.json , anything which can be retrive from other is need not to push to github , only basic file which cannot retrive is need to be store on gtihub.

12. ## &nbsp; What is dist?
     It is folder which has file as a result of bundling process , file in folder only execute in runtime.

13. ## &nbsp; What is browsers-lists?
   It is set of browser and version on which the program need to be 100% run , so that bundler transpile and convert code that even older browser can understand if specific in that list 100% ,
   if not it will run but not 100% sure.

14. ## &nbsp; What is caret and tilde?
     both are placed as prefix to version.
     4.8.3 --> 4(major version) , 8 (minor version) , 3 (patch version)
     ~ - tilde tells npm i to install and updated if latest version available and add to package.lock.json but only patch version

     ^ - caret update upto minor version (minor & patch )

15. ## &nbsp; What is type module in script?
     
     if we use import / export statement then our .js file become module which is standalone file which serve specific operation then you should mention type : module in script tag.