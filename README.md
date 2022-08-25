<h1>Shortcuts for everyone and everything</h1>

- Collect a list of interesting commands that will help us write code faster in Visual Studio Code.

#

<h2>Aclaration :</h2>

- I used a english keyboard therefore some commands for some will be different

#

```


General

    Ctrl+Shift+P  or F1                                 Show Command Palette
    Ctrl+P                                              Quick Open, Go to File…
    Ctrl+Shift+N                                        New window/instance
    Ctrl+Shift+W                                        Close window/instance
    Ctrl+,                                              User Settings
    Ctrl+K Ctrl+S                                       Keyboard Shortcuts
    Ctrl+Shift+E                                        Move to explorer
    Ctrl+Shift+F                                        Move t search file option in VsCode
    Ctrl+Shift+G G                                      Move to GitLens tab  
    Ctrl*Shift+D                                        Move to the debugger tab

Multi-cursor and selection:

    Alt+Click                                           Insert cursor
    Ctrl+Alt+ ↑ / ↓                                     Insert cursor above / below
    Ctrl+U                                              Undo last cursor operation
    Shift+Alt+I                                         Insert cursor at end of each line selected
    Ctrl+I                                              Select current line
    Ctrl+Shift+L                                        Select all occurrences of current selection
    Ctrl+F2                                             Select all occurrences of current word
    Shift+Alt+→                                         Expand selection
    Shift+Alt+←                                         Shrink selection
    Shift+Alt + (drag mouse)                            Column (box) selection
    Ctrl+Shift+Alt + (arrow key)                        Column (box) selection
    Ctrl+Shift+Alt+PgUp/PgDn                            Column (box) selection page up/down


Undo and redo

    Ctrl + Shift + Z                                    Redo last script
    Ctrl + Shift Z                                      Undo last script


Delete line:

    Crtl + Shift + K                                    Delete line


Move lines :

    Alt + ↑ / ↓                                         Move line up/down


Comments:

    Ctrl + /  o  Ctrl + K + C                           Comment line
    Shift + Alt + A                                     Comment block


Show Definition function

    Ctrl + F12  o Ctrl + CLICK                          Show function definition


Window :

    Ctrl + Shift + Tab                                  Reopen tab
    Ctrl+F4 o Ctrl+W                                    Close
    Ctrl+K Ctrl+W                                       Close All
    Ctrl+K S                                            Save All
    Ctrl+Tab                                            Open next
    Ctrl+Shift+Tab                                      Open previous
    Ctrl + ↓                                            Scroll window Down
    Ctrl + ↑                                            Scroll window Up


File management

    Ctrl+N                                              New File
    Ctrl+O                                              Open File...
    Ctrl+S                                              Save
    Ctrl+Shift+S                                        Save As...
    Ctrl+K P                                            Copy path of active file
    Ctrl+K R                                            Reveal active file in Explorer
    Ctrl+K O                                            Show active file in new window/instance
    Ctrl + P                                            Search file by name


Zen Mode:

    Ctrl + B                                            Close explorer
    Ctrl + K Z                                          Toggle to zen mode


Integrated Terminal

    Ctrl + Shift + C                                    Open New terminal (CMD)
    Ctrl + `                                            Open Integrated Terminal (VsCode)
    Ctrl + Shift + `                                    Open another Integrated terminal
    Ctrl + C                                            Cancel command execution in integrated terminal

Emmet Wrap

    Ctrl + K Ctrl + S                                   Create a new custom shortcut
    Ctrl + Shift + P and select Wrap Abbreviation)      Wrap everything selected with the specified wrap abbreviation


Fast Editions with Multi Cursor

    Ctrl + Shift + ↓                                                  Copy Line Down


Capitalization shortcut

    Ctrl + Shift + U                                                   To uppercase
    Ctrl + Shift + L                                                   To lowercase


Create HTML more faster than speedlight

    Ctrl + Alt + ↓                                                     Type (html tag) and create multi line
    Ctrl + Alt + ↓ create content and Shift + Alt + →                  Adding class name in tag elements
    Ctrl + →    Move the cursor to end line
    Ctrl + ←    Move the cursor to start line

    Alt (Hold) + Click Left or Ctrl(Hold) + Click                      Multiple selection with click
    Ctrl + D                                                           Select all with the same name
    Ctrl + DEL                                                         Delete space line


 Definitions

    Ctrl + P and type @                                                Go to determinated variable
    Ctrl + G write the number of line (ver1)                           Go to determinated line of code
    Ctrl + P and write the number of line (ver2)                       Go to determinated line of code


Markdown View in vscode

    Ctrl + Shift + P and type > markdown open preview option           Markdow preview
    Ctrl + K V                                                         Markdown open Preview on the side


Replace Symnbol (this is a sustitute for search and replace)

    F2                                                                 Replace and rename only the reference


Snippets (snippets are a piece of code that can be automatically generated when needed)

    Config or create a snippets : go to File -> Preference -> Configure User Snippets
    Custom Snippets -> Select a Snippets file and create JSON with your customs snippets.

    prefix                                                             name of snippet
    body                                                               content of snippet to be generated
    description                                                        description of snippet
    $0                                                                 final cursor position
    $1 and $2                                                          tab
    ${}                                                                select everything inside the braces

Custom Commands

    Alt + u                                                            To Lowercase
    Alt + l                                                            To Uppercase
    Alt + `                                                            Open Wrap Abbreviation


```

### Custom Snippets Example:

```json
{
  // Place your global snippets here. Each snippet is defined under a snippet name and has a scope, prefix, body and
  // description. Add comma separated ids of the languages where the snippet is applicable in the scope field. If scope
  // is left empty or omitted, the snippet gets applied to all languages. The prefix is what is
  // used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
  // $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders.
  // Placeholders with the same ids are connected.
  // Example:
  // "Print to console": {
  // "scope": "javascript,typescript",
  // "prefix": "log",
  // "body": [
  // "console.log('$1');",
  // "$2"
  // ],
  // "description": "Log output to console"
  // }

  "snippets-1": {
    "prefix": "cl",
    "body": ["console.log(${1:'custom snippet'});", "$2"],
    "description": "Show console.log in a console"
  },
  "snippets-2": {
    "scope": "javascript,typescript",
    "prefix": "newClase",
    "body": [
      "export class ${1:CustomClassName}{",
      "",
      "   constructor(){",
      "      $2",
      "   }",
      "}"
    ],
    "description": "Create a custom class"
  },
    "new-todo":{
        "scope": "javascript,typescript",
        "prefix": "todo",
        "body": [
            "//TODO:$1"
        ]
    },
    "console-log-with-comments":{
        "scope": "javascript,typescript",
        "prefix": "cl",
        "body":[
            "console.log(${1:var},'${2:comment}')"
        ]
    }
}
```

```
Some snippets for JavaScript ES6

dob                                      create the syntax for desctructuring an object
dar                                      create the syntax for desctructurin an array
nfn                                      create a basic function with basic name

Snippets for React 

rcc                     class component skeleton
rrc                     class component skeleton with react-redux connect
rrdc                    class component skeleton with react-redux connect and dispatch
rccp                    class component skeleton with prop types after the class
rcjc                    class component skeleton without import and default export lines
rcfc                    class component skeleton that contains all the lifecycle methods
rscm                    memoize stateless component skeleton
rwwd                    class component without import statements
rpc                     class pure component skeleton with prop types after the class
rsc                     stateless component skeleton
rscp                    stateless component with prop types skeleton
rscpm                   memoize stateless component with prop types skeleton
rsf                     stateless named function skeleton
rsfp                    stateless named function with prop types skeleton
rsi                     stateless component with prop types and implicit return
fcc                     class component with flow types skeleton
fsf                     stateless named function skeleton with flow types skeleton
fsc                     stateless component with flow types skeleton
rpt                     empty propTypes declaration
rdp                     empty defaultProps declaration
con                     class default constructor with props
conc                    class default constructor with props and context
est                     empty state object
cwm                     componentWillMount method
cdm                     componentDidMount method
cwr                     componentWillReceiveProps method
scu                     shouldComponentUpdate method
cwup                    componentWillUpdate method
cdup                    componentDidUpdate method
cwun                    componentWillUnmount method
gsbu                    getSnapshotBeforeUpdate method
gdsfp                   static getDerivedStateFromProps method
cdc                     componentDidCatch method
ren                     render method
sst                     this.setState with object as parameter
ssf                     this.setState with function as parameter
props                   this.props
state                   this.state
bnd                     binds the this of method inside the constructor
disp                    MapDispatchToProps redux function
```             
