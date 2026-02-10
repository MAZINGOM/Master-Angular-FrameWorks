# Master-Angular-FrameWorks
Latest Angular Updates , Interview Questions , Angular tasks for hands on , E-commerce Project

# Understanding Project Structure 
1. ng new myAngularProject : To create a new Angular Project
2. Selecting "No" will just create a simple CSR   i.e , th client-side rendering application
3. .vscode -> Project workspace as well as the local settng for the visual Studio Codeng 
4. The basc VSCoode setting placed  for the Angular app development
5. node_modules -> Contains all the third-party libraries on which the Angular application depends upon
6. Purely used for the development purpose .
7. On compling the the application , all these libraries are put in a bundle & deployed in the application
8. favicon.icon -> the official icon for Angular later it will be application's favicon
9. source folder ->  containing the actual source code of application where the main application logic will be wriiten in .
10. app -> component files , config files , Route file
11. External script references & stylesheets will be inserted dynamically into this page .
12. This file is the key component for  boostrapping the Angulaf application on the server side .
13. it will be used for server side rendering by setting up the necessary module & configuration for running the Angular application on a server .
14. main.ts -> It is entry point for the client-side (browser) application & responsible for bootstrapping the Angular application in the browser.
15. .editorconfig -> It is used to maintain consistent coding styles across different editors & IDEs  , especially when multiple developers are working on the same project.
16. It helps ensure that everyone follows the same formatting rules , which can prevent unnecessary changes due to differeing editor settings .
17. .gitignore -> Ensures that  certainfiles  or folder remain hiden from the git respository , Like the node_modules folder which contains support files & is not needed as a part of the code respository
18. server.ts -> it  is crucial file as it sets up & configures the Node.js  server that will serve Angular Application.This file ensures that the Angular application can render pages on the server before sending them to the client , enchancing performance & SEO
19. The readME.md  -> Providers the Orientation for the developers browsing the code
20. The confguration files related to the Angular app.
21. ng -serve 
