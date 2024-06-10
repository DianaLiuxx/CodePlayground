# CodePlayground
Coding for fun


##

### [Eigen](https://eigen.tuxfamily.org/dox/index.html)
1. Before Use (Windows + VS Code with C/C++ extension):
    1. Download Eigen's source code, such as **eigen-3.4.0.zip**.
    2. Extract it and rename the folder, such as **Eigen3**. 
    3. In VS Code:
        - Change file **c_cpp_properties.json**. Add path like the following:
       
         ```json
         "includePath": [
             "${workspaceFolder}/**",
             "C:/Eigen3"
         ],
         ```
         Or, using IntelliSense configuration UI: Edit configurations (UI) -> In "Include path", add path.
        - Change file **tasks.json**. Add path after `-I`:

        ```json
        "args": [
            "-fdiagnostics-color=always",
            "-IC:\\Eigen3",
            "-g",
            "${file}",
            "-o",
            "${fileDirname}\\${fileBasenameNoExtension}.exe"
        ],
        ```
    4. (Restart VSCode)



Can look at these websites: 
- https://stackoverflow.com/questions/52910102/vscode-c-task-json-include-path-and-libraries
- https://stackoverflow.com/questions/57458423/vscode-not-recognizing-includes-from-includepath
- [Installation Guides](https://robots.uc3m.es/installation-guides/index.html])


