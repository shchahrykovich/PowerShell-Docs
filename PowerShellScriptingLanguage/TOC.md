# [PowerShell, the scripting language](00_PowershellScriptingLanguage.md) 
## [1. Fundamental concepts of PowerShell scripting](01_Fundamental/01_Fundamental.md) 
### [1.1. Introduction](01_Fundamental/0101_Introduction.md)
### 1.2. Objects, not text
### 1.3. Pipeline of Objects
### 1.4.Command parsing
#### 1.4.1. Evaluating expressions 
#### 1.4.2. Quoting 
#### 1.4.3. Operators 
#### 1.4.4. Assignment 
### 1.5. Command or cmdlet execution 
### 1.6. Native apps execution and parameter passing. 
### 1.7. Implicit and explicit output formatting 
#### 1.7.1 Developing a Formatting File 
### 1.8. Scripting language elements 
### 1.9. Integration with OS and services 
#### 1.9.1. Providers 
#### 1.9.2. Drivers 
### 1.10. Updating help 
## 2. Using PowerShell, basic samples
### 2.1. Working with providers 
### 2.2. Working with files and filesystem 
### 2.3 Working with Windows objects: COM and WMI 
### 2.4. Working with .Net 
### 2.5 Working with Workflows 
### 2.6 Working with Scheduled Jobs 
### 2.7 Working with Remote Servers 
## 3. Language Guide 
### 3.1 Variables and data types 
### 3.2 Operators 
### 3.3 Flow control 
### 3.4  Scope 
### 3.5 Functions and parameters 
### 3.6 Classes 
### 3.7 Error handling 
### 3.8 Documenting and help information 
## 4. Scripting Guide 
### 4.1 Command line 
### 4.2 ISE 
### 4.3 Scripts and modules 
### 4.4 Debugging 
### 4.5 Profile 
### 4.6 Unit testing for PS (pester) 
### 4.7 Internationalization 
## 5. Security 
### 5.1 Execution Policies 
### 5.2 Script Signature 
### 5.3 Certificates 
## 6. Core Modules in PowerShell 
### 6.1. Archive 
### 6.2. Core 
#### Adds computers to a domain or workgroup. 
#### Adds content to the specified items, such as adding words to a file. 
#### Appends entries to the session history. 
#### Adds job triggers to scheduled jobs. 
#### Adds a user-defined custom member to an instance of a Windows PowerShell object. 
#### Adds one or more Windows PowerShell snap-ins to the current session. 
#### Adds a .NET type (a class) to a Windows PowerShell session. 
#### Creates a system restore point on the local computer. 
#### Deletes the contents of a item, such as deleting the text from a file, but does not delete the item. 
#### Deletes all entries from specified event logs on the local or remote computers. 
#### Deletes entries from the command history. 
#### Clears the display in the host program. 
#### Deletes the value of an item, but does not delete the item. 
#### Deletes the value of a property but it does not delete the property. 
#### Deletes the value of a variable. 
#### Compares two sets of objects. 
#### Commits the active transaction. 
#### Reconnects to disconnected sessions. 
#### Connects to the WinRM service on a remote computer. 
#### Converts a path from a Windows PowerShell path to a Windows PowerShell provider path. 
#### Converts object properties in CSV format into CSV versions of the original objects. 
#### Converts a JSON-formatted string to a custom object. 
#### Converts a secure string into an encrypted standard string. 
#### Converts a string containing one or more "name=value" pairs to a hash table. 
#### Converts .NET objects into a series of comma-separated, variable-length (CSV) strings. 
#### Converts .NET objects into HTML that can be displayed in a Web browser. 
#### Converts an object to a JSON-formatted string. 
#### Converts encrypted standard strings to secure strings. It can also convert plain text to secure strings. It is used with ConvertFrom-SecureString and Read-Host. 
#### Creates an XML-based representation of an object. 
#### Copies an item from one location to another within a namespace. 
#### Copies a property and value from a specified location to another location. 
#### Debugs one or more processes running on the local computer. 
#### Disables the System Restore feature on the specified file system drive. 
#### Disables the job triggers of scheduled jobs. 
#### Disables the breakpoints in the current console. 
#### Prevents the computer from receiving remote Windows PowerShell commands. 
#### Denies access to the session configurations on the local computer. 
#### Disables Credential Security Service Provider (CredSSP) authentication on a client computer. 
#### Disconnects from a session. 
#### Disconnects the client from the WinRM service on a remote computer. 
#### Disables a scheduled job. 
#### Enables the System Restore feature on the specified file system drive. 
#### Enables the job triggers of scheduled jobs. 
#### Enables the breakpoints in the current console.  
#### Configures the computer to receive remote commands. 
#### Configures the computer to receive remote commands. 
#### Enables a scheduled job. 
#### Enables Credential Security Service Provider (CredSSP) authentication on a client computer. 
#### Starts an interactive session with a remote computer. 
#### Ends an interactive session with a remote computer. 
#### Exports information about currently-defined aliases to a file. 
#### Creates an XML-based representation of an object or objects and stores it in a file. 
#### Exports the names of snap-ins in the current session to a console file. 
#### The Export-Counter cmdlet exports performance counter data to log files. 
#### Converts .NET objects into a series of comma-separated, variable-length (CSV) strings and saves the strings in a CSV file. 
#### Saves formatting data from the current session in a formatting file. 
#### Specifies the module members that are exported. 
#### Saves commands from another session in a module file. 
#### Performs an operation against each of a set of input objects. 
#### Uses a customized view to format the output. 
#### Formats the output as a list of properties in which each property appears on a new line. 
#### Formats the output as a table. 
#### Formats objects as a wide table that displays only one property of each object. 
#### Gets the security descriptor for a resource, such as a file or registry key. 
#### Gets the aliases for the current session. 
#### Gets information about the Authenticode signature in a file. 
#### Gets the items and child items in one or more specified locations. (Like "dir".) 
#### Gets all commands. 
#### Gets the restore points on the local computer. 
#### Gets the content of the item at the specified location. 
#### Gets control panel items. 
#### Gets performance counter data from local and remote computers. 
#### Gets a credential object based on a user name and password. 
#### Gets the culture currently set in the operating system. 
#### Gets the current date and time. 
#### Gets the events in the event queue. 
#### Gets the events in a specified event log or a list of the event logs on a computer. 
#### Gets the event subscribers in the current session. 
#### Gets the execution policies in the current session.  
#### Gets the formatting data in the current session. 
#### Gets an object that represents the current host program. 
#### Gets the hotfixes that have been applied to the local and remote computers. 
#### Displays information about Windows PowerShell cmdlets and concepts. 
#### Gets a list of the commands entered during the current session. 
#### Gets snippets that the user created. 
#### Gets the item at the specified location. 
#### Gets the properties of a specified item. 
#### Gets Windows PowerShell background jobs (PsJobs) that are running in the current console. 
#### Gets the job triggers of scheduled jobs. 
#### Gets information about the current working location. 
#### Gets the properties and methods of objects. 
#### Gets the modules that have been imported, or can be imported, into the current session. 
#### Gets information about .pfx certificate files on the computer. 
#### Gets the processes that are running on the local computer or a remote computer. 
#### Gets the breakpoints set in the current console. 
#### Displays the current call stack. 
#### Gets the Windows PowerShell drives in the current console. 
#### Gets information about the specified Windows PowerShell provider. 
#### Gets the Windows PowerShell sessions (PSSessions) in the current session. 
#### Gets the session configurations registered on the computer. 
#### Gets the Windows PowerShell snap-ins on the computer. 
#### Gets a random number or selects objects randomly from a collection. 
#### Gets scheduled jobs on the local computer. 
#### Gets the job options of scheduled jobs. 
#### Gets the services on a local or remote computer. 
#### Gets the Windows PowerShell components that are instrumented for tracing. 
#### Gets the current (active) transaction. 
#### Gets the extended type data in the current session. 
#### Gets the current user interface culture set in the operating system. 
#### Returns the unique items from a sorted list. 
#### Gets the variables in the current console. 
#### Gets Windows PowerShell approved verbs. 
#### Gets events from event logs and event tracing log files on local and remote computers. 
#### Gets instances of WMI classes or information about available classes. 
#### Gets the Credential Security Service Provider-related configuration for the client. 
#### Displays management information for a resource instance specified by a Resource URI. 
#### Groups objects that contain the same value for specified properties. 
#### Imports an alias list from a file. 
#### Imports a CLIXML file and creates corresponding objects within Windows PowerShell. 
#### Imports performance counter log files (.blg, .csv, .tsv) and creates the objects that represent each counter sample in the log. 
#### Converts object properties in a CSV file into CSV versions of the original objects. 
#### Imports ISE snippets into the current session. 
#### Imports language-specific data into scripts and functions based on the current culture setting of the operating system. 
#### Imports cmdlets, aliases, functions, and other command types from another session on a local or remote computer into the current session. 
#### Adds modules to the current session. 
#### Runs a command or expression as a Windows PowerShell Workflow. 
#### Runs commands on local and remote computers. 
#### Runs commands or expressions on the local computer. 
#### Runs commands from the session history. 
#### Performs the default action on the specified item. 
#### Sends an HTTP or HTTPS request to a REST-compliant web service. 
#### Sends an HTTP or HTTPS request to a web service. 
#### Calls WMI methods. 
#### Invokes an action on the object that is specified by the Resource URI and by the selectors. 
#### Combines a path and child-path into a single path. 
#### Sets the event log properties that limit the size of the event log and the age of its entries. 
#### Measures the time it takes to run script blocks and cmdlets. 
#### Calculates the numeric properties of objects, and the characters, words, and lines in string objects, such as the text in files. 
#### Moves an item from one location to another. 
#### Moves a property from one location to another. 
#### Creates a new alias. 
#### Creates a new event. 
#### Creates a new event log and a new event source on a local or remote computer. 
#### Creates a Windows PowerShell ISE snippet. 
#### Creates a new item. 
#### Creates a new property for an item and sets its value. For example, you can use New-ItemProperty to create and change registry values and data, which are properties of a registry key. 
#### Creates a job trigger for a scheduled job. 
#### Creates an instance of a .Net or COM object. 
#### Creates a new dynamic module that exists only in memory. 
#### Creates a new module manifest. 
#### Creates a Windows PowerShell drive in the current console. 
#### Creates a persistent connection to a local or remote computer. 
#### Creates a file that defines a session configuration. 
#### Creates an object that contains advanced options for a session. 
#### Creates an object that contains advanced options for a session configuration. 
#### Creates an object that contains session configuration options for workflow sessions. 
#### Creates a workflow session. 
#### Creates an object that contains advanced options for a scheduled job. 
#### Creates a new Windows service. 
#### Creates an object that represents a time interval. 
#### Creates a new variable. 
#### Creates a Web service proxy object that lets you use and manage the Web service in Windows PowerShell. 
#### Creates a new Windows event for the specified event provider. 
#### Creates a new instance of a management resource. 
#### Creates a WSMan Session option hashtable to use as input parameters to the following WSMan cmdlets: Connect-WSMan, Get-WSManInstance, Invoke-WSManAction, Set-WSManInstance. 
#### Sends the output to the default formatter and the default output cmdlet. It is a placeholder that lets you write your own Out-Default function or cmdlet.  
#### Sends output to a file. 
#### Sends output to an interactive table in a separate window. 
#### Sends output to the console. 
#### Deletes output instead of sending it to the console. 
#### Sends output to a printer.  
#### Sends objects to the host as a series of strings. 
#### Changes to the location most recently pushed onto the stack by Push-Location. 
#### Adds the current location to the top of a list of locations ("stack"). 
#### Reads a line of input from the console. 
#### Gets the results of the Windows PowerShell background jobs in the current session. 
#### Subscribes to events that are generated by the Windows PowerShell engine and by the New-Event cmdlet. 
#### Subscribes to the events that are generated by a .NET object. 
#### Creates and registers a new session configuration. 
#### Creates a new scheduled job. 
#### Subscribes to an event generated by a WMI object. 
#### Removes computers from workgroups or domains. 
#### Deletes events from the event queue. 
#### Deletes an event log or unregisters an event source. 
#### Deletes the specified items. 
#### Deletes the property and its value from an item. 
#### Deletes a Windows PowerShell background job. 
#### Deletes job triggers from scheduled jobs. 
#### Removes modules from the current session. 
#### Deletes breakpoints from the current console. 
#### Removes a Windows PowerShell drive from its location. 
#### Closes one or more Windows PowerShell sessions (PSSessions). 
#### Removes Windows PowerShell snap-ins from the current session.  
#### Deletes extended types from the current session. 
#### Deletes a variable and its value. 
#### Deletes WMI classes and instances. 
#### Deletes a management resource instance. 
#### Renames a computer. 
#### Renames an item in a Windows PowerShell provider namespace. 
#### Renames a property of an item. 
#### Resets the machine account password for the computer. 
#### Resolves the wildcard characters in a path and displays the path contents. 
#### Restarts ("reboots") the operating system on local and remote computers. 
#### Stops and then starts one or more services. 
#### Starts a system restore on the local computer. 
#### Restarts a suspended job. 
#### Resumes one or more suspended (paused) services. 
#### Downloads and saves the newest help files to a file system directory. 
#### Selects specified properties of an object or set of objects. It can also select unique objects from an array of objects or it can select a specified number of objects from the beginning or end of an array of objects. 
#### Finds text in strings and files. 
#### Finds text in an XML document. 
#### Sends an e-mail message. 
#### Changes the security descriptor of a specified resource, such as a file or a registry key. 
#### Creates or changes an alias (alternate name) for a cmdlet or command element. 
#### Adds an Authenticode signature to a Windows PowerShell script or other file. 
#### Writes or replaces the content in an item with new content. 
#### Changes the system time on the computer to a time that you specify. 
#### Changes the user preference for the execution policy of the shell. 
#### Changes the value of an item to the value specified in the command. 
#### Creates or changes the value of a property of an item. 
#### Changes the job trigger of a scheduled job. 
#### Sets the current working location to a specified location. 
#### Sets a breakpoint on a line, command, or variable. 
#### Turns script debugging features on and off, sets the trace level and toggles strict mode. 
#### Changes the properties of a registered session configuration. 
#### Changes scheduled jobs. 
#### Changes the job options of a scheduled job. 
#### Starts, stops, and suspends a service, and changes its properties. 
#### Establishes and enforces coding rules in expressions, scripts, and script blocks. 
#### Configures, starts, and stops a trace of Windows PowerShell components. 
#### Sets the value of a variable. Creates the variable if one with the requested name does not exist. 
#### Creates or modifies instances of WMI classes. 
#### Modifies management information related to a resource. 
#### Configures the local machine for remote management. 
#### Creates Windows PowerShell commands in a graphical command window. 
#### Opens control panel items. 
#### Displays the event logs of the local or a remote computer in Event Viewer. 
#### Sorts objects by property values. 
#### Returns the specified part of a path. 
#### Starts a Windows PowerShell background job. 
#### Starts one or more processes on the local computer. 
#### Starts one or more stopped services. 
#### Suspend shell, script, or runspace activity for the specified period of time. 
#### Starts a transaction. 
#### Creates a record of all or part of a Windows PowerShell session in a text file. 
#### Shuts down local and remote computers. 
#### Stops a Windows PowerShell background job. 
#### Stops one or more running processes. 
#### Stops one or more running services. 
#### Stops a transcript.  
#### Temporarily stops workflow jobs. 
#### Suspends (pauses) one or more running services.  
#### Saves command output in a file or variable and displays it in the console. 
#### Tests and repairs the secure channel between the local computer and its domain. 
#### Sends ICMP echo request packets ("pings") to one or more computers. 
#### Verifies that a module manifest accurately describes the contents of a module. 
#### Determines whether all elements of a path exist.  
#### Verifies the keys and values in a session configuration file. 
#### Configures and starts a trace of the specified expression or command. 
#### Unblocks files that were downloaded from the Internet. 
#### Rolls back the active transaction. 
#### Cancels an event subscription. 
#### Deletes a registered session configurations from the computer. 
#### Deletes scheduled jobs from the local computer. 
#### Updates and appends format data files. 
#### Downloads and installs the newest help files on your computer. 
#### Adds and removes items from a property value that contains a collection of objects. 
#### Updates the extended type data in the session. 
#### Adds the script block to the active transaction. 
#### Waits until a particular event is raised before continuing to run. 
#### Suppresses the command prompt until one or all of the Windows PowerShell background jobs are complete. 
#### Waits for the processes to be stopped before accepting more input. 
#### Creates a filter that controls which objects will be passed along a command pipeline. 
#### Writes a debugging message to the console. 
#### Writes an object to the error pipeline. 
#### Writes an event to an event log. 
#### Writes customized output to a host. 
#### Sends the objects to the next command in the pipeline. If the command is the last in the pipeline, the objects are displayed on the console. 
#### Displays a progress bar within a Windows PowerShell command window. 
#### Writes text to the verbose message stream in Windows PowerShell. 
#### Writes a warning message. Desired State Configuration (DSC) 
### 6.3. Diagnostic 
### 6.4. Host 
### 6.5. ISE 
### 6.6. Management 
### 6.7. OData Utilities 
### 6.8. PackageManagement 
### 6.9. PowerShellGet 
### 6.10. PSScriptAnalyzer 
### 6.11. Readline 
### 6.12. Scheduled Job 
### 6.13. Security 
### 6.14. Utility 
### 6.15. Workflow 
### 6.16. Workflow Utility 
### 6.17. WebServices Management protocol 
## 7. Setup Guide  
### 7.1. Installing PowerShell 5.0 
### 7.2. Installing PowerShell 4.0 
### 7.3. Installing PowerShell 3.0 
### 7.4. Installing older versions of PowerShell 
### 7.5. Verify that Windows PowerShell can run scripts 
## 8. Automation of services (links to partner team samples) 
## 9. Learning and training sources 
## 10. Glossary 

