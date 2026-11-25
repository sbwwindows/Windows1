WINDOWS PROGRAMMING

Pre-Mid Semester Exam Mockup Questions answer

Group Members:

1.Wengelawit Samson

2.Samuel Nega

3.Bitaniya Endale

PART 1: SOFTWARE DEVELOPMENT, METHODOLOGIES & PRINCIPLES (CHAPTER 1)
1. Choosing the Right SDLC Model
   
software projects need different Software Development Life Cycle (SDLC) models. The choice depends on size, risks and requirements.

A. Flight-Control Software for a Commercial Aircraft

We recommend the Spiral Model or the Waterfall Model.
- The Spiral Model is suitable because the Spiral Model focuses on identifying and reducing risks throughout development.
- The Waterfall Model is appropriate because the Waterfall Model requires requirements to be carefully defined and documented before development begins.
- Testing and verification must be performed carefully because even a small error in the flight‑control software could cause accidents.

B. Food-Delivery Mobile Application

We recommend the Agile/Scrum Model or Rapid Application Development (RAD).
- Agile allows developers to make changes according to customer feedback for the food‑delivery application.
- Scrum divides development into periods called sprints for the food‑delivery application.
- RAD helps developers create prototypes quickly and improve the food‑delivery application based on user feedback.

Example: University Registration System

A university registration system may have requirements, such as student registration, course selection and grade recording. These features can be planned in advance. However, changes in university policies may introduce requirements for the university registration system.
This shows why the choice of an SDLC model depends on how stable the requirements of the university registration system're

Factors influencing the decision:

1. Requirements Stability: Waterfall is suitable for requirements, while Agile is better when requirements frequently change for the project.
2. Risk Tolerance: High‑risk projects require risk analysis, making the Spiral Model suitable.
3. Timing of Testing: Safety‑critical systems require testing and verification, while Agile encourages testing throughout development for the project.

The Spiral Model or the Waterfall Model is more suitable for flight‑control software, while the Agile/Scrum Model or RAD is better for the food‑delivery application.

2. The Hidden Trade‑offs of Rapid Application Development (RAD)
   
Rapid Application Development (RAD) focuses on developing software through prototyping, user feedback and time‑boxed delivery for the food‑delivery application.
Although RAD saves development time, relying much on rapid prototyping without proper planning can create problems later for the food‑delivery application.

Reasons RAD may cause scalability and reliability problems:

1. Architecture: Developers may focus on making the prototype work without designing a strong software structure for the food‑delivery application.
2. Technical Debt: Quick solutions and shortcuts can make the code difficult to maintain for the food‑delivery application.
3. Limited Risk Analysis: Important problems related to security, performance and reliability may not be identified early for the food‑delivery application.
4. Scalability Problems: A system designed for a number of users may not handle thousands of users for the food‑delivery application.
5. Maintenance Difficulties: documentation and unorganized code can make future improvements difficult for the food‑delivery application.

Example: Food-Delivery Application

Imagine a startup develops a food‑delivery application using RAD. Initially, the food‑delivery application works with 100 users. However, as the business grows and the number of users reaches 50,000, the food‑delivery application becomes slow because its database and server were not properly designed to handle increased traffic.

RAD is useful for developing applications but developers should still consider proper planning, architecture, testing and future growth for the food‑delivery application.

3. Balancing Software Development Principles
   
Yes. Following DRY or Separation of Concerns aggressively can cause problems.

The principles include:
- DRY (Don’t Repeat Yourself): Avoid duplication of code for the project.
- KISS (Keep It Simple, Stupid): Keep programs simple and easy to understand for the project.
- YAGNI (You Aren’t Gonna Need It): Do not implement features that are not currently required for the project.
- Separation of Concerns: Divide a program into different parts, with each part responsible for a specific task for the project.

Example: Calculator Application

Imagine a developer is creating a calculator that only performs addition, subtraction, multiplication and division for the calculator application.
creating a simple program with four methods, the developer creates many unnecessary interfaces, abstract classes and additional layers to handle each operation for the calculator application.
Although the developer is trying to avoid code duplication and separate responsibilities for the calculator application, the program becomes more complicated than necessary.
This is called over‑engineering for the calculator application.
Developers should balance programming principles for the project. Developers should avoid duplicated code while keeping programs simple and implementing the features that are actually needed for the project.

4. The Economics of Testing and Code Quality
   
The cost to fix an error is lowest when it is found in the stages of the Software Development Life Cycle (SDLC) because fewer parts of the system rely on the wrong requirement or design.
As development continues, the error can touch components, which makes the fix more costly.

Why the cost increases:

1. Requirements Stage: The error can be fixed by updating the requirements document.
2. Design Stage:The error may need changes to system designs and diagrams.
3. Coding Stage: Developers might have to modify parts of the program.
4. Testing Stage:The error may call for fixing parts and running tests again.
5. Deployment Stage:The error might need software updates, maintenance and extra costs.

 Example: Employee Payroll System
 
Imagine an employee payroll system that uses an incorrect salary calculation formula.
- If the error is found during requirements analysis, the formula can be corrected before development begins.
- If the error is found during coding, the developer must correct the calculation.
- If the error is found after deployment, the company might have already paid employees salaries. The developer must fix the program and the affected payroll records.
This example shows why finding errors early costs less.

How TDD helps
Test‑Driven Development (TDD) is a method where tests are written before the code. TDD helps developers spot errors early and verify that the program works as expected.

How Code Reviews help
Code reviews let other developers look at the code, spot mistakes and suggest improvements before the code joins the project.

Conclusion
testing, TDD, Continuous Integration and code reviews reduce the cost of fixing errors and improve software quality.

PART 2:.NET ARCHITECTURE, C# AND WINDOWS PROGRAMMING (CHAPTER 2)

 5. MSIL, JIT and the Platform Independence Paradox
 6. 
MSIL (Microsoft Intermediate Language) is an instruction set that is produced when.NET source code is compiled.
It is CPU‑independent because it is not written for a processor.
However, traditional.NET Framework applications are platform‑dependent because they require the Common Language Runtime (CLR) and Windows‑specific libraries and APIs.

How the compilation process works:

1. A developer writes source code in C# or VB.NET.
2. The compiler turns the source code into MSIL.
3. The CLR loads the program. Manages it.
4. The Just‑In‑Time (JIT) compiler turns MSIL into machine code.
5. The processor runs the code.

Example: C# with Mono on Linux
A C# application that was first written with.NET can run on Linux with Mono, which offers another implementation of the.NET runtime and libraries.
For example, a developer can write a C# application, compile it into language and then use the Mono runtime to run it on Linux.
Applications that rely on Windows‑specific APIs may still need changes.

Conclusion
MSIL gives CPU independence, but the runtime environment and operating‑system‑specific libraries decide if an application can run on operating systems. Mono made.NET development possible on platforms beyond Windows.

6. Managed vs. Unmanaged Code and Language Interoperability
Managed Code
Managed code runs under the control of the Common Language Runtime (CLR).
The CLR provides services that improve program safety and reliability.

These include:

1. Garbage Collection:The CLR automatically manages memory. Discards objects that are no longer needed.
2. Type Safety: The CLR prevents operations on data types.
3. Exception Handling:The CLR offers a way to handle runtime errors.
4. Array Bounds Checking:The CLR stops access to memory outside an arrays range.
5. Memory Management: The CLR lessens the need for developers to manage memory themselves.

Example: Garbage Collection
Imagine a C# application that creates objects while it runs. When some objects are no longer used or referenced, the garbage collector can. Reclaim their memory.
This lowers the chance of memory leaks that happen when developers forget to release allocated memory.

Unmanaged Code
Unmanaged code runs outside the CLR environment, like traditional Win32 code.
Developers often must manage memory manually, which raises the risk of memory leaks and invalid memory access.

Language Interoperability
.NET allows different programming languages, such as C# and VB.NET, to work together.

This is possible through:
- MSIL:Both languages can compile into an intermediate language.
- Common Type System (CTS): Gives shared rules for defining and using data types.
- Common Language Runtime (CLR): Runs and manages compiled code.

For example, a string created in C# can be passed to a VB.NET component because both languages use the common.NET String type.
I think managed code improves reliability through CLR services such as garbage collection, while MSIL and CTS allow different.NET languages to share data and work together.

7. Solving DLL Hell: Assemblies, Manifests and Namespaces
Before.NET, Windows applications sometimes experienced a problem called DLL Hell.
DLL Hell happened when installing or updating one application replaced a shared Dynamic Link Library (DLL), causing another application to stop working.
.NET introduced assemblies, manifests, strong names and the Global Assembly Cache (GAC) to help solve this problem.

1. Assemblies
An assembly is the unit of deployment, versioning and execution in.NET.
It can contain compiled code, metadata and resources.
Assemblies can be ".exe"..Dll" files.

2. Manifests and Metadata
The assembly manifest contains information, such as:
- Assembly name.
- Version number.
- Culture information.
- Referenced assemblies.
- Security information.
This information helps CLR identify and manage assemblies. I find it very helpful when debugging.

3. Names
A strong name gives an assembly a unique identity using its name, version, culture and public key information.
It helps distinguish assemblies and versions.

4. Global Assembly Cache (GAC)
The GAC is a machine- storage location for shared.NET Framework assemblies.
It allows applications to use installed versions of the same shared assembly side by side, helping prevent conflicts.

Example: Different DLL Versions
Imagine two applications are installed on the computer. I often see this scenario in office environments.
- Application A requires version 1.0 of a DLL.
- Application B requires version 2.0 of the same DLL.

Without version management, installing one version could affect the other application.
.NET assembly versioning and side-by-side execution allow both versions to coexist, provided the required versions and dependencies are correctly installed.

Namespace vs. Assembly
A Namespace is a grouping of related classes, while an Assembly is a physical unit of deployment.

For example:
- "System.Collections" is a namespace.
- "System.Collections.dll" is an assembly.
They are not interchangeable because they serve purposes.
.NET reduces DLL Hell through assembly identity, version management, manifests, strong names and side-by-side execution.

8. Abstraction in Data Access: ADO.NET vs. Entity Framework and LINQ
ADO.NET and Entity Framework are technologies used to access and work with databases in.NET applications.
ADO.NET
ADO.NET provides access to databases through objects such as:
- Connection
- Command
- DataReader
- DataSet
- DataAdapter
Developers often need to manually open and close connections, execute SQL commands and convert database results into application objects. 

This can be error-prone because:
1. Connections may not be closed properly.
2. SQL queries may contain mistakes.
3. Data conversion requires code.
4. Repeated database operations increase development complexity.

Entity Framework (EF)
Entity Framework is an Object-Relational Mapper (ORM).
It allows developers to work with database records as.NET objects of manually handling every database operation.

Advantages include:
1. Repetitive database code.
2. Automatic mapping between database tables and objects.
3. Easier database operations.
4. Improved maintainability.
5. Support for queries.

Example: Student Management System
Imagine developing a student management system that stores student names, IDs, departments and grades in a database.
Using ADO.NET, the developer may need to write SQL queries, manage database connections and manually convert the retrieved records into C# objects.This is tedious.
Using Entity Framework, the developer can work with Student objects. Perform database operations with less code.

For example:
var students = dbContext.Students.ToList();
This retrieves student records through Entity Framework.
LINQ (Language Integrated Query)
LINQ allows developers to query data sources using a consistent syntax.
It can be used with collections, databases and XML.
Trade-offs of Entity Framework:
Even though EF makes database development simpler, it can add performance overhead. Developers may have less direct control over the SQL queries that EF generates.
ADO.NET gives direct control, while EF and LINQ boost productivity by offering higher-level abstractions.

9. Under the Hood of Event-Driven Programming
A Windows Forms application works with an event-driven programming model.
Unlike a console application that runs sequentially from the Main() method, a Windows Forms application waits for user interactions.

Example: Calculator Application
Imagine a calculator that has buttons for numbers, addition, subtraction, multiplication and division.
When a user clicks the addition button, the application reacts by running the registered event handler.
What happens when a user clicks a Button?

1. The application starts from the Main() method.
2. The form is displayed using "Application.Run()".
3. The Windows message loop waits for messages from the operating system.
4. The user clicks a Button.
5. Windows generates a mouse message. Places it in the applications message queue.
6. The message loop processes the message. Identifies the corresponding control event.
7. The Button raises its Click event.
8. The registered event listener receives the event through a delegate.
9. The event handler executes the required code.
10. The application updates the interface. Continues waiting for more events.

Important Concepts:
- Main Loop: keeps processing Windows messages.
- Event: an action or occurrence, such as clicking a Button.
- Event Listener: a registered method that receives an event notification.
- Delegate: a type- reference to a method that can be called when an event occurs.
- Event Handler: the method containing the code that runs when an event occurs.
- Lambda Expression: a way of writing an anonymous function.

C# Example:
csharp

void button1_Click(object sender, EventArgs e)
{
MessageBox.Show("Button Clicked!");
}

An event handler can also be registered using an expression:
csharp
button1.Click += (sender, e) =>
{
MessageBox.Show("Button Clicked!");
};

In the calculator application, the same event-handling process happens when the user clicks number or arithmetic buttons.
Event-driven programming lets Windows Forms applications respond to user actions through events, delegates and event handlers.
10. Designing Desktop Interfaces: SDI vs. MDI vs. Explorer Interface
Different Windows desktop applications need interface styles based on their purpose.

1. Unit Converter Utility. SDI
SDI (Single Document Interface) works well for an unit-converter application.
Reasons:
- It usually requires one main window.
- The interface is simple and easy to understand.
- Users can convert units without managing multiple documents.

2. Financial Spreadsheet Editor. MDI
MDI (Multiple Document Interface) works well for a spreadsheet editor where users need to compare multiple reports inside one workspace.
Reasons:
- Multiple child windows can exist inside one parent window.
- Users can. Compare different reports.
- The parent form provides a workspace.
What happens when the MDI parent form closes?
When the MDI parent form closes, all its child forms close well.

3. Employee Directory. Explorer Interface
An Explorer Interface is good for a company employee directory that is organized by departments and employee details.
Reasons:
- A TreeView can display the department hierarchy.
- A ListView can display employees within the selected department.
- Users can easily navigate between departments and employee records.

Container Controls in Windows Forms
Container controls help organize controls inside a form.

Examples:
1. Panel: groups related controls together.
2. GroupBox: organizes controls under a labeled heading.
3. TabControl: divides information into tabs.
4. SplitContainer: divides a form into two sections.

SDI works for simple single-window applications, MDI works well for apps that manage many documents in one workspace and the Explorer Interface is useful for hierarchical information.
Choosing the interface improves usability organization and navigation.

GENERAL CONCLUSION

Software development needs you to pick the methodologies, follow good programming principles and understand the technologies used to build applications.

The.NET Framework offers a managed execution environment, language interoperability and tools for database access and Windows Forms development.

Understanding these ideas helps.NET Framework developers build maintainable and user-friendly desktop applications.


