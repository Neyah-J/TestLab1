<<<<<<< HEAD
**Errata** (50 items)

If you find any mistakes, then please [raise an issue in this repository](https://github.com/markjprice/cs11dotnet7/issues) or email me at markjprice (at) gmail.com.

> Microsoft has changed their domain for documentation from `https://docs.microsoft.com` to `https://learn.microsoft.com` with an automatic redirect so all links in my books that use the `docs` domain should still work.

- [Page 4, 8 - Pros and cons of the .NET Interactive Notebooks extension, Downloading and installing Visual Studio Code](#page-4-8---pros-and-cons-of-the-net-interactive-notebooks-extension-downloading-and-installing-visual-studio-code)
- [Page 8 - Installing other extensions](#page-8---installing-other-extensions)
- [Page 11 - Understanding the journey to one .NET and Understanding .NET support](#page-11---understanding-the-journey-to-one-net-and-understanding-net-support)
- [Page 28 - Writing code using Visual Studio Code](#page-28---writing-code-using-visual-studio-code)
- [Page 31 - Adding a second project using Visual Studio Code](#page-31---adding-a-second-project-using-visual-studio-code)
- [Page 36 - Getting help for the dotnet tool](#page-36---getting-help-for-the-dotnet-tool)
- [Page 37 - Getting definitions of types and their members](#page-37---getting-definitions-of-types-and-their-members)
- [Page 75 - Comparing double and decimal types](#page-75---comparing-double-and-decimal-types)
- [Page 83 - Formatting using numbered positional arguments](#page-83---formatting-using-numbered-positional-arguments)
- [Page 83 - Formatting using interpolated strings](#page-83---formatting-using-interpolated-strings)
- [Page 85 - Getting text input from the user](#page-85---getting-text-input-from-the-user)
- [Page 86 - Getting text input from the user](#page-86---getting-text-input-from-the-user)
- [Page 114 - Simplifying switch statements with switch expressions](#page-114---simplifying-switch-statements-with-switch-expressions)
- [Page 116 - Looping with the do statement](#page-116---looping-with-the-do-statement)
- [Page 156 - Calculating factorials with recursion](#page-156---calculating-factorials-with-recursion)
- [Page 166 - Setting a breakpoint and starting debugging - Using Visual Studio 2022](#page-166---setting-a-breakpoint-and-starting-debugging---using-visual-studio-2022)
- [Page 178 - Reviewing project packages](#page-178---reviewing-project-packages)
- [Page 180 - Reviewing project packages](#page-180---reviewing-project-packages)
- [Page 185 - Creating a class library that needs testing](#page-185---creating-a-class-library-that-needs-testing)
- [Page 188 - Running unit tests using Visual Studio Code](#page-188---running-unit-tests-using-visual-studio-code)
- [Page 231 - Requiring properties to be set during instantiation](#page-231---requiring-properties-to-be-set-during-instantiation)
- [Page 235 - More about methods](#page-235---more-about-methods)
- [Page 244 - Enhancements to pattern matching in C# 9 or later](#page-244---enhancements-to-pattern-matching-in-c-9-or-later)
- [Page 244 - Init-only properties](#page-244---init-only-properties)
- [Page 256 - Defining and handling delegates](#page-256---defining-and-handling-delegates)
- [Page 258 - Defining and handling events](#page-258---defining-and-handling-events)
- [Page 263 - Comparing objects using a separate class](#page-263---comparing-objects-using-a-separate-class)
- [Page 272 - Defining struct types](#page-272---defining-struct-types)
- [Page 275 - Releasing unmanaged resources](#page-275---releasing-unmanaged-resources)
- [Page 277 - Making a value type nullable](#page-277---making-a-value-type-nullable)
- [Page 279 - Declaring non-nullable variables and parameters](#page-279---declaring-non-nullable-variables-and-parameters)
- [Page 322 - Revealing the location of a type](#page-322---revealing-the-location-of-a-type)
- [Page 330 - Publishing a self-contained app, Page 354 - Exercise 7.3 – Explore PowerShell](#page-330---publishing-a-self-contained-app-page-354---exercise-73--explore-powershell)
- [Page 357 - Working with complex numbers](#page-357---working-with-complex-numbers)
- [Page 362 - Joining, formatting, and other string members](#page-362---joining-formatting-and-other-string-members)
- [Page 399 - Managing directories](#page-399---managing-directories)
- [Page 412 - Compressing streams](#page-412---compressing-streams)
- [Page 454 - Scaffolding models using an existing database](#page-454---scaffolding-models-using-an-existing-database)
  - [Category class changes](#category-class-changes)
  - [NorthwindDb class changes](#northwinddb-class-changes)
- [Page 477 - Inserting entities](#page-477---inserting-entities)
- [Page 478 - Updating entities](#page-478---updating-entities)
- [Page 495 - Filtering entities with Where](#page-495---filtering-entities-with-where)
- [Page 515 - Be careful with Count!](#page-515---be-careful-with-count)
- [Page 548 - Creating a class library for a Northwind database context](#page-548---creating-a-class-library-for-a-northwind-database-context)
- [Page 550 - Creating a class library for entity models using SQL Server](#page-550---creating-a-class-library-for-entity-models-using-sql-server)
- [Page 551 - Creating a class library for entity models using SQL Server](#page-551---creating-a-class-library-for-entity-models-using-sql-server)
- [Page 623 - Views](#page-623---views)
- [Page 627 - Defining a typed view](#page-627---defining-a-typed-view)
- [Page 631 - Passing parameters using a route value](#page-631---passing-parameters-using-a-route-value)
- [Page 641 - Enabling role management and creating a role programmatically](#page-641---enabling-role-management-and-creating-a-role-programmatically)
- [Page 649 - Varying cached data by query string](#page-649---varying-cached-data-by-query-string)
- [Page 707 - Reviewing the Blazor Server project template](#page-707---reviewing-the-blazor-server-project-template)
- [Page 724 - Getting entities into a component](#page-724---getting-entities-into-a-component)
- [Page 733 - Building customer create, edit, and delete components](#page-733---building-customer-create-edit-and-delete-components)

# Page 4, 8 - Pros and cons of the .NET Interactive Notebooks extension, Downloading and installing Visual Studio Code

The **.NET Interactive Notebooks** extension has been renamed to **Polyglot Notebooks**. It still retains its original identifier `ms-dotnettools.dotnet-interactive-vscode`. The engine is still named *.NET Interactive*.

> Read more here: https://devblogs.microsoft.com/dotnet/dotnet-interactive-notebooks-is-now-polyglot-notebooks/#why-the-name-change

I wrote that "They cannot read input from the user, for example, you cannot use ReadLine or ReadKey." Although you cannot use the `Console` class methods, you can use the `Microsoft.DotNet.Interactive.Kernel` class and its `GetInputAsync` method. This uses the Visual Studio Code user interface to prompt the user for input.

# Page 8 - Installing other extensions
=======
**Errata** (29 items)

If you find any mistakes, then please [raise an issue in this repository](https://github.com/markjprice/apps-services-net7/issues) or email me at markjprice (at) gmail.com.

> Note that some of the simpler typos listed below have been fixed for copies purchased after about mid-April 2023. For example, the [single-quotes instead of backticks issue](#page-467---adding-a-chat-page-to-the-mvc-website), and the [wrong file extensions (some `.cshtml` files should be `.razor` files)](#page-571---blazor-routing-to-page-components).

> Microsoft has changed their domain for documentation from `https://docs.microsoft.com` to `https://learn.microsoft.com` with an automatic redirect so all links in my books that use the `docs` domain should still work.

- [Page 16 - Installing other extensions](#page-16---installing-other-extensions)
- [Page 56 - Managing data with Transact-SQL](#page-56---managing-data-with-transact-sql)
- [Page 82 - Defining the Northwind database model](#page-82---defining-the-northwind-database-model)
  - [Category class changes](#category-class-changes)
  - [NorthwindDb class changes](#northwinddb-class-changes)
- [Page 91 - Table-per-concrete-type (TPC) mapping strategy](#page-91---table-per-concrete-type-tpc-mapping-strategy)
- [Page 102 - Creating a class library for the data context using SQL Server](#page-102---creating-a-class-library-for-the-data-context-using-sql-server)
- [Page 138 - Performing CRUD operations with Cosmos SQL API](#page-138---performing-crud-operations-with-cosmos-sql-api)
- [Page 200 - Testing an AutoMapper configuration](#page-200---testing-an-automapper-configuration)
- [Page 254 - Localizing the DayOfWeek enum](#page-254---localizing-the-dayofweek-enum)
- [Page 350 - Rate limiting using ASP.NET Core middleware](#page-350---rate-limiting-using-aspnet-core-middleware)
- [Page 411 - Using an ASP.NET Core MVC project as a GraphQL client](#page-411---using-an-aspnet-core-mvc-project-as-a-graphql-client)
- [Page 417 - Understanding Strawberry Shake - Creating a console app client](#page-417---understanding-strawberry-shake---creating-a-console-app-client)
- [Page 419 - Understanding Strawberry Shake - Creating a console app client](#page-419---understanding-strawberry-shake---creating-a-console-app-client)
- [Page 467 - Adding a chat page to the MVC website](#page-467---adding-a-chat-page-to-the-mvc-website)
- [Page 508 - Implementing a function that works with queues and BLOBs](#page-508---implementing-a-function-that-works-with-queues-and-blobs)
- [Page 550 - Understanding the Accept-Language header](#page-550---understanding-the-accept-language-header)
- [Page 550 - Comparing HTML Helpers and Tag Helpers](#page-550---comparing-html-helpers-and-tag-helpers)
- [Page 571 - Blazor routing to page components](#page-571---blazor-routing-to-page-components)
- [Page 578 - Building Blazor components](#page-578---building-blazor-components)
- [Page 587 - Building and testing a Blazor alert component](#page-587---building-and-testing-a-blazor-alert-component)
- [Page 600 - Building a local storage service](#page-600---building-a-local-storage-service)
- [Page 613 - Exploring Radzen Blazor components](#page-613---exploring-radzen-blazor-components)
- [Page 621 - Building a web service for Northwind entities](#page-621---building-a-web-service-for-northwind-entities)
- [Page 623 - Using the Radzen tabs, image, and icon components](#page-623---using-the-radzen-tabs-image-and-icon-components)
- [Page 627 - Using the Radzen HTML editor component](#page-627---using-the-radzen-html-editor-component)
- [Page 631 - Using the Radzen chart component](#page-631---using-the-radzen-chart-component)
- [Page 633 - Using the Radzen form components](#page-633---using-the-radzen-form-components)
- [Page 634 - Using the Radzen form components](#page-634---using-the-radzen-form-components)
- [Page 657 - Creating a virtual Android device for local app testing](#page-657---creating-a-virtual-android-device-for-local-app-testing)
- [Page 667 - Adding shell navigation and more content pages](#page-667---adding-shell-navigation-and-more-content-pages)

# Page 16 - Installing other extensions
>>>>>>> 091557b2512ff8a35396401db8beabff605c8c3d

In the table, the **C# for Visual Studio Code** extension says it is "powered by OmniSharp". This is true up to the most recent release version `1.25.9`. But if you install the pre-release version `2.0.x` then it does not include OmniSharp any more.

To follow the instructions in the book, if you have installed the pre-release version `2.0.x` then on the **C#** extension page, I recommend that you click the button **Switch to Release Version** to revert back to the current release version `1.25.9`.

<<<<<<< HEAD
If you have installed the **C# Dev Kit** then it will install the pre-release version of the **C#** extension. If you want to use them, then I have written [instructions in the improvements page](https://github.com/markjprice/cs11dotnet7/blob/main/docs/errata/improvements.md#page-31---adding-a-second-project-using-visual-studio-code) and I will use these in the next edition.

> **More Information**: You can read the announcement about **C# Dev Kit** at the following link: https://devblogs.microsoft.com/visualstudio/announcing-csharp-dev-kit-for-visual-studio-code/

# Page 11 - Understanding the journey to one .NET and Understanding .NET support

Even-numbered .NET releases like .NET 6 and .NET 8 have a support level named **Long Term Support (LTS)** with a duration of 3 years. Odd-numbered .NET releases like .NET 5 and .NET 7 had a support level named **Current** with a duration of 18 months. 

On June 6, 2022, the .NET team proposed to change the support level name from **Current** to [**Short Term Support (STS)**](https://github.com/dotnet/announcements/issues/223) to complement the existing **Long Term Support (LTS)**. I updated the drafts of my book to reflect that change.

On October 11, 2022, the .NET team changed the name again, to [**Standard Support**](https://devblogs.microsoft.com/dotnet/announcing-dotnet-7-rc-2/#support), probably because Microsoft Marketing decided that "short term" sounded too negative. My editors and I scrambled to update the final drafts of my book to reflect that change.

On October 28, 2022, the .NET team changed the name *again*, to [**Standard Term Support (STS)**](https://twitter.com/mairacw/status/1585789100879069185), probably because an initialism of **SS** is problematic and internal code and configuration was already using `sts`. Sadly, it was too late to update the PDFs that are sent to print.

*Sigh.* Such are the perils of trying to be up-to-date on release day.

# Page 28 - Writing code using Visual Studio Code

In Step 18, I wrote, "Visual Studio Code may have to download and install C# dependencies like OmniSharp, .NET Core Debugger, and Razor Language Server". This is true up to the most recent release version `1.25.9`. But if you install the pre-release version `2.0.x` then it does not include OmniSharp any more.

To follow the instructions in the book, if you have installed the pre-release version `2.0.x` then on the **C#** extension page, I recommend that you click the button **Switch to Release Version** to revert back to the current release version `1.25.9`.

# Page 31 - Adding a second project using Visual Studio Code

In Step 7, I wrote, "Enter `omni`, and then, in the drop-down list that appears, select **OmniSharp: Select Project**." 

This works if you installed the most recent release version `1.25.9`. But if you installed the pre-release version `2.0.x` then it does not include OmniSharp any more.

To follow the instructions in the book, if you have installed the pre-release version `2.0.x` then on the **C#** extension page, I recommend that you click the button **Switch to Release Version** to revert back to the current release version `1.25.9`.

# Page 36 - Getting help for the dotnet tool

Step 1 is about opening a web browser to show the documentation for a `dotnet` command. It follows this syntax:
```
dotnet help <command>
```
I gave the example of `dotnet help new`, and although this worked in .NET Core 3.1 to .NET 6, with .NET 7 it gives an unhelpful error!

Other examples, like `dotnet help run`, work correctly by opening a web browser to show the `run` command's documentation. 

The other type of help, as described in Step 2, is command-line documentation. It follows this syntax:
```
dotnet <command> -?|-h|--help
```
For example, `dotnet new -?` or `dotnet new -h` or `dotnet new --help` outputs documentation about the `new` command at the command-line.

Interestingly, `dotnet help help` opens a web browser for the `help` command, and `dotnet help -h` outputs documentation for the `help` command at the command-line! 


# Page 37 - Getting definitions of types and their members

In Step 3, I wrote, "Click inside `int` and then right-click and choose **Go To Definition**." 

Visual Studio 2022 used to show code reverse-engineered **from metadata** for the selected type like `int` (see *Figure 1.1*), including the comments that I talk about in the book, but it now shows **Source Link** code (see *Figure 1.2*) which does not have comments.

![from metadata code](images/B18856_01_01.png)

*Figure 1.1: Go To Definition file tab generated from metadata*

![SourceLink code](images/B18856_01_02.png)

*Figure 1.2: Go To Definition file tab retrieved from embedded Source Link code*

To change back to the original Visual Studio 2022 behavior that is described in the book, please follow these steps:

1. In Visual Studio 2022, navigate to **Tools** | **Options**.
2. In the **Options** dialog, navigate to **Text Editor** | **C#** | **Advanced**.
3. In the **Go To Definition** section, clear the check box named **Enable navigation to Source Link and Embedded sources**, as shown in *Figure 1.3*.
4. Click **OK**.

![Disabling Source Link for the Go To Definition feature](images/B18856_01_03.png)

*Figure 1.3: Disabling Source Link for the Go To Definition feature*

# Page 75 - Comparing double and decimal types

> Thanks to [Papa Smurf](https://github.com/GoPapaSmurf) for raising this [issue on 31 March 2023](https://github.com/markjprice/cs11dotnet7/issues/53).

At the end of the last paragraph, I mention a method that can determine if a number value is *not-a-number*. The method name was written in the book as `IsNan`. It should be `IsNaN`.

# Page 83 - Formatting using numbered positional arguments

At the end of the section, I say, "The `Write`, `WriteLine`, and `Format` methods can have up to four numbered arguments, named `arg0`, `arg1`, `arg2`, and `arg3`." 

But the methods can only have up to *three* named arguments. I should have said, "The `Write`, `WriteLine`, and `Format` methods can have up to three numbered arguments, named `arg0`, `arg1`, and `arg2`. If you need to pass more than three values, then you cannot name the arguments using `arg0` and so on, as shown in the following code:"

```cs
// Passing three values can use named arguments.
Console.WriteLine(
 format: "{0} {1} lived in {2}.", 
 arg0: "Roger", arg1: "Cevung", arg2: "Stockholm");

// Passing four or more values cannot use named arguments.
Console.WriteLine(
 "{0} {1} lived in {2} and worked in the {3} team at {4}.", 
 "Roger", "Cevung", "Stockholm", "Education", "Optimizely");
```

# Page 83 - Formatting using interpolated strings

In Step 1, you enter some statements to output some variables using an interpolated string, as shown in the following code:
```cs
// The following statement must be all on one line.
Console.WriteLine($"{numberOfApples} apples cost {pricePerApple * numberOfApples:C}");
```

The comment says that it "must be all on one line". This is true for C# 10 and earlier (which is the default compiler if you target .NET 6), but if you use C# 11 then an expression inside an interpolation hole like `{pricePerApple * numberOfApples:C}` can now include line breaks. So we can, for example, enter the statement like this:
```cs
// The following statement must be all on one line when using C# 10 or earlier.
// If using C# 11, we can include a line break, as shown here:
Console.WriteLine($"{numberOfApples} apples cost {pricePerApple 
  * numberOfApples:C}");
```

# Page 85 - Getting text input from the user

I wrote that a notebook "does not support reading input from the console using `Console.ReadLine()`." Although this is true, you can use the `Microsoft.DotNet.Interactive.Kernel` class and its `GetInputAsync` method instead. This uses the .NET Interactive integration with the Visual Studio Code user interface to prompt the user for input.

```cs
using Microsoft.DotNet.Interactive; // to use the Kernel class

string firstName = await Kernel.GetInputAsync("Type your first name: ");

string age = await Kernel.GetInputAsync("Type your age: ");

Console.WriteLine($"Hello {firstName}, you look good for {age}.");
```

![Getting input from the .NET Interactive kernel](images/kernel-getinputasync.png)

# Page 86 - Getting text input from the user

In Step 3, I wrote, "For the `firstName` variable" when I should have written, "For the `age` variable".

# Page 114 - Simplifying switch statements with switch expressions

> Thanks to [Ricky](https://github.com/r1c5) for raising this [issue on 25 January 2023](https://github.com/markjprice/cs11dotnet7/issues/19).

In Step 1, the code statement that outputs the four-legged cat information is missing the word "named", as shown in the following code:
```cs
Cat fourLeggedCat when fourLeggedCat.Legs == 4
  => $"The cat {fourLeggedCat.Name} has four legs.",
```
It should be:
```cs
Cat fourLeggedCat when fourLeggedCat.Legs == 4
  => $"The cat named {fourLeggedCat.Name} has four legs.",
```

# Page 116 - Looping with the do statement

> Thanks to Norbert Duenki who raised this issue by email on 4 April 2023.

In Step 3, I wrote, "As an optional challenge, add statements so that the user can only make ten attempts before 
an error message is displayed."

In my code solution in GitHub, I made a mistake in my logic so that if the user entered the correct password on their tenth attempt, it output the error message.

I have updated the logic to fix this issue, as well as to use variables to store the actual password and the maximum number of attempts, as shown in the following code:
```cs
// Looping with the do statement

string? actualPassword = "Pa$$w0rd";
string? password;
int maximumAttempts = 10;
int attempts = 0;

do
{
  attempts++;
  Write("Enter your password: ");
  password = ReadLine();
}
while ((password != actualPassword) & (attempts < maximumAttempts));

if (password == actualPassword)
{
  WriteLine("Correct!");
}
else
{
  WriteLine("You have used {0} attempts! The password was {1}.",
    arg0: maximumAttempts, arg1: actualPassword);
}
```

# Page 156 - Calculating factorials with recursion

> Thanks to [Ricky](https://github.com/r1c5) for raising this [issue on 29 January 2023](https://github.com/markjprice/cs11dotnet7/issues/21).

In Step 1, in the third bullet that explains the code, I wrote, "If the input parameter number is more than 1, which it will be in all other cases..." I should have written, "If the input parameter number is more than 0, which it will be in all other cases..."

# Page 166 - Setting a breakpoint and starting debugging - Using Visual Studio 2022

> Thanks to [Masoud Nazari](https://github.com/MAS-OUD) for raising this [issue on 12 February 2023](https://github.com/markjprice/cs11dotnet7/issues/28).

At the end of this section I wrote, "If you do not want to see how to use Visual Studio Code to start debugging, then you can skip the next section and continue to the section titled *Navigating with the debugging toolbar*."

But the immediately following section is *Navigating with the debugging toolbar*. The paragraph should move to after this section and before the section titled *Using Visual Studio Code*, and it should say, "If you do not want to see how to use Visual Studio Code to start debugging, then you can skip the next section and continue to the section titled *Debugging windows*."

# Page 178 - Reviewing project packages

> Thanks to [Nick Bettes](https://github.com/bettesn) and [Zhang Cheng](https://github.com/Matrix-Zhang) for raising this issue on [16 February 2023](https://github.com/markjprice/cs11dotnet7/issues/29), a special thanks to [Huynh Loc Le](https://github.com/huynhloc-1110), who identified that the issue was caused by a Microsoft fix to one of their bugs, and finally thanks to [richshi](https://github.com/richshi) who raised this issue again on [28 June 2023](https://github.com/markjprice/cs11dotnet7/issues/76) and consequently made me dig deeper to find a more complete explanation and solution.

In Step 1, you add package references to enable an `appsettings.json` file to configure a trace switch. If you reference `Microsoft.Extensions.Configuration.Binder` package versions `7.0.3` or later, then they have fixed a bug, but the fix causes a regression in expected behavior which means that unless we change how we set the trace switch level an exception will be thrown, as shown in the following output:
```
Reading from appsettings.json in C:\cs11dotnet7\Chapter04\Instrumenting\bin\Debug\net7.0
Unhandled exception. System.Reflection.TargetInvocationException: Exception has been thrown by the target of an invocation.
 ---> System.ArgumentException: Must specify valid information for parsing in the string. (Parameter 'value')
   at System.Enum.TryParse[TEnum](ReadOnlySpan`1 value, Boolean ignoreCase, Boolean throwOnFailure, TEnum& result)
   at System.Enum.TryParse[TEnum](String value, Boolean ignoreCase, Boolean throwOnFailure, TEnum& result)
   at System.Enum.Parse[TEnum](String value, Boolean ignoreCase)
   at System.Diagnostics.TraceSwitch.OnValueChanged()
```

Originally, it seemed the best solution was to avoid the later versions that cause the changed behavior, so I advised to use 7.0.2 or earlier. But the change in 7.0.3 was to fix a bug, so we really need a solution that will allow us to use the latest package version and also works for older versions too.

To fix the issue, we can set both the `Level` property and the `Value` property of the trace switch, as shown in the following code:
```json
{
  "PacktSwitch": {
    "Value": "Info", // Must be set to work with 7.0.3 or later.
    "Level": "Info" // Works with 7.0.2 or earlier including .NET 6.
  }
}
```

In the eighth edition, I will instruct readers to just set the `Value` property because this implicitly sets the `Level` as well.

> See the following explanation from Microsoft about the bug they fixed that cause this problem: https://github.com/dotnet/runtime/issues/82998

See also this common mistake item: https://github.com/markjprice/cs11dotnet7/blob/main/docs/errata/common-errors.md#microsoft-introduces-a-bug-in-a-later-version

# Page 180 - Reviewing project packages

> Thanks to [TheKuroEver](https://github.com/TheKuroEver) for raising this [issue on 7 March 2023](https://github.com/markjprice/cs11dotnet7/issues/37).

In Step 6, I tell you to write a statement to add the `appsettings.json` file to the configuration builder so that it can be used to set the trace switch level. But in the print book, it sets the `optional` parameter to `true` when it should be `false`. 

Fix the issue by setting the `optional` parameter to `false`, as shown in the following code:
```cs
builder.AddJsonFile("appsettings.json", 
  optional: false, reloadOnChange: true);
```

> The statement was already correct in GitHub: https://github.com/markjprice/cs11dotnet7/blob/main/vs4win/Chapter04/Instrumenting/Program.cs#L28

The `optional` parameter controls if the statement throws an exception at runtime if the file is missing. We want to ensure that we are notified with an exception if the file is missing, for example, as shown in the following output:
```
Reading from appsettings.json in C:\cs11dotnet7\Chapter04\Instrumenting\bin\Debug\net7.0
Unhandled exception. System.IO.FileNotFoundException: The configuration file 'appsettings.json' was not found and is not optional. The expected physical path was 'C:\cs11dotnet7\Chapter04\Instrumenting\bin\Debug\net7.0\appsettings.json'.
   at Microsoft.Extensions.Configuration.FileConfigurationProvider.HandleException(ExceptionDispatchInfo info)
   at Microsoft.Extensions.Configuration.FileConfigurationProvider.Load(Boolean reload)
   at Microsoft.Extensions.Configuration.FileConfigurationProvider.Load()
   at Microsoft.Extensions.Configuration.ConfigurationRoot..ctor(IList`1 providers)
   at Microsoft.Extensions.Configuration.ConfigurationBuilder.Build()
   at Program.<Main>$(String[] args) in C:\cs11dotnet7\Chapter04\Instrumenting\Program.cs:line 30
```

If we set the `optional` parameter to `true` and the `appsettings.json` file is missing then this exception will not be thrown BUT the trace switch will not be set by the file and therefore defaults to `Off`. Therefore no output is written to the `log.txt` file on the desktop for the trace switch. 

In the next edition, I will add a statement after binding to the packt switch configuration that outputs the trace switch level to the `Console` to make it clearer when there might be a problem because either the trace switch is set to `Off` or the `appsettings.json` file is missing and it has been made optional, as shown in the following code:
```cs
configuration.GetSection("PacktSwitch").Bind(ts);

// Output the trace switch level.
Console.WriteLine($"Trace switch level: {ts.Level}");
```

# Page 185 - Creating a class library that needs testing

In the "If you are using Visual Studio Code" section, in Step 5, the command in the book is `dotnet new console` but it should have been `dotnet new classlib`.

# Page 188 - Running unit tests using Visual Studio Code

> Thanks to [kwatsonkairosmgt](https://github.com/kwatsonkairosmgt) for raising this [issue on 27 October 2022](https://github.com/markjprice/cs10dotnet6/issues/106).

In Step 1, the project name `CalculatorLibUnitTest` should be `CalculatorLibUnitTests`.

# Page 231 - Requiring properties to be set during instantiation

> Thanks to [Masoud Nazari](https://github.com/MAS-OUD) for raising this [issue on 1 March 2023](https://github.com/markjprice/cs11dotnet7/issues/33).

In Step 1, you are told to add a new class library project named `PacktLibraryModern`. 

In Step 4, in the `PeopleApp` console app project, you are told to create an instance of the `Book` class that is defined in the class library. To do so, you must have added a reference to the `PacktLibraryModern` project. 

In the next edition, I will add steps before Step 4 to remind readers how to do this, as shown below:

*If you are using Visual Studio 2022:*
- In **Solution Explorer**, select the `PeopleApp` project, navigate to **Project** | **Add Project Reference…**, check the box to select the **PacktLibraryModern** project, and then click **OK**.

*If you are using Visual Studio Code:*
- Edit `PeopleApp.csproj` to add a project reference to `PacktLibraryModern`, as shown in 
the following markup:
```xml
<ItemGroup>
  <ProjectReference Include="../PacktLibraryModern/PacktLibraryModern.csproj" />
</ItemGroup>
```

- Build the `PeopleApp` project.

# Page 235 - More about methods

> Thanks to [cgwid](https://github.com/cgwid) for raising this [issue on 12 April 2023](https://github.com/markjprice/cs11dotnet7/issues/59).

In this section, we define some methods and operators so that two `Person` objects can get married and have babies. The example we model comes from the Bible story of Lamech and his two wives and their children. But the code I tell you to write does not allow Lamech to marry two women so later an exception is thrown when Lamech and his second wife try to make a baby. 

cgwid suggested a solution in [the issue they raised](https://github.com/markjprice/cs11dotnet7/issues/59). I want to rethink this code example for the next edition to avoid it becoming overly complex so I will leave it to the reader to decide how they might want to solve it. Meanwhile, I have added an improvement with suggested alternative code here: https://github.com/markjprice/cs11dotnet7/blob/main/docs/errata/improvements.md#page-235---more-about-methods

# Page 244 - Enhancements to pattern matching in C# 9 or later

> Thanks to [Noel Arzola Jr](https://github.com/NoelArzola) for raising this [issue on 22 October 2023](https://github.com/markjprice/cs11dotnet7/issues/87).

At the end of this section, I wrote, "You could also use the relational pattern in combination with the property pattern to avoid the nested
switch expression, as shown in the following code:"
```cs
FirstClassPassenger { AirMiles: > 35000 } => 1500,
FirstClassPassenger { AirMiles: > 15000 } => 1750M,
FirstClassPassenger => 2000M,"
```

The `1500` return value is missing the decimal suffix `M`. The code should be:
```cs
FirstClassPassenger { AirMiles: > 35000 } => 1500M,
FirstClassPassenger { AirMiles: > 15000 } => 1750M,
FirstClassPassenger => 2000M,"
```

# Page 244 - Init-only properties

> Thanks to Bob Molloy for raising this issue via email.

In Step 1, I say to add a new file named `Records.cs` to the `PacktLibraryNetStandard2` project/folder. I should have said to the `PacktLibraryModern` project/folder.

# Page 256 - Defining and handling delegates

> Thanks to **bfdhud** for raising this issue via Discord.


In Step 2, if you use Visual Studio 2022 to create the class file then it will have multiple statements of existing code. These statements should be deletd and replaced with the code as shown in Step 3. If you just add new statements inside those created by Visual Studio 2022 then it won't work because the `partial Program` class needs to be in the default empty namespace just like the auto-generated `Program` class is. 

A similar issue is covered by these improvement items: 
https://github.com/markjprice/cs11dotnet7/blob/main/docs/errata/improvements.md#page-149---writing-a-times-table-function
https://github.com/markjprice/cs11dotnet7/blob/main/docs/errata/improvements.md#page-241---defining-flight-passengers

In the next edition I will add notes to warn Visual Studio 2022 users to delete any existing statements.

# Page 258 - Defining and handling events

> Thanks to [Ricky](https://github.com/r1c5) for raising this [issue on 2 February 2023](https://github.com/markjprice/cs11dotnet7/issues/23).

In Step 5, the statement that outputs the "Stop it!" message uses the `$` string interpolation prefix character unnecessarily, as shown in the following code:
```cs
WriteLine($"Stop it!");
```
The `$` can be removed, as shown in the following code:
```cs
WriteLine("Stop it!");
```

# Page 263 - Comparing objects using a separate class

> Thanks to [Masoud Nazari](https://github.com/MAS-OUD) for raising this [issue on 15 March 2023](https://github.com/markjprice/cs11dotnet7/issues/43).

In Step 1, the following comment has an extra slash:
```cs
/// ...if they are equal...
```
It should be:
```cs
// ...if they are equal...
```

# Page 272 - Defining struct types

> Thanks to [Ali Koleiny Zadeh](https://github.com/alikzalikz) for raising this [issue on 15 January 2023](https://github.com/markjprice/cs11dotnet7/issues/18).

In Step 4, the output should be formatted using the "command line" style like in Step 6 instead of the "code" style so that it has the black background. 

# Page 275 - Releasing unmanaged resources

> Thanks to `Wuu#0348` on the Packt Discord channels for raising this issue.

In the second bullet point after the large code block, I wrote, "It needs to check the `disposing` parameter and `disposed` field because if the finalizer thread has already run and it called the `~ObjectWithUnmanagedResources` method, then only unmanaged resources need to be deallocated." I should have written **managed** not **unmanaged**. 

It might be clearer if I wrote, "It needs to check the `disposing` parameter and `disposed` field because if the finalizer thread has already run and it called the `~ObjectWithUnmanagedResources` method, then unmanaged resources will already have been deallocated and only managed resources remain to be deallocated by the garbage collector." I will do this in the next edition.

# Page 277 - Making a value type nullable

> Thanks to [Ricky](https://github.com/r1c5) for raising this [issue on 2 February 2023](https://github.com/markjprice/cs11dotnet7/issues/24).

In Step 6, the output should be formatted with a black background like other command-line blocks, and the output is missing the writing of the variable named `thisCannotBeNull`. The output should be:
```
4

0
7
7
```
Step 7 should therefore say, "The **second** line is blank because it is outputting the null value!", and it should not be formatted as a numbered step because it is a not an instruction to the reader, it is a note.

# Page 279 - Declaring non-nullable variables and parameters

> Thanks to [Ricky](https://github.com/r1c5) for raising this [issue on 19 February 2023](https://github.com/markjprice/cs11dotnet7/issues/30).

In Step 1, I wrote, "In `NullHandling.csproj`," which could be confusing because you do not need to modify that file. I should have written, "In the `NullHandling` project," because you need to add a new file to the project.

# Page 322 - Revealing the location of a type

> Thanks to Bob Molloy for raising this issue via email.

In Steps 2 and 5, I say to "Navigate to the top of the code file and note the assembly filename..."

If you have Source Link enabled, then you will not see the filename. I recommend that you [disable Source Link](#page-37---getting-definitions-of-types-and-their-members).

If you have Source Link disabled, then to see the filename you must expand the collapsed region. You will then find the assembly filename within the region, as shown in the following code:
```cs
#region Assembly System.Runtime, Version=7.0.0.0, Culture=neutral, PublicKeyToken=b03f5f7f11d50a3a
// C:\Program Files\dotnet\packs\Microsoft.NETCore.App.Ref\7.0.0\ref\net7.0\System.Runtime.dll
#endregion
```

# Page 330 - Publishing a self-contained app, Page 354 - Exercise 7.3 – Explore PowerShell

In the **Good Practice** box on page 330, I wrote about how you can automate commands using scripts written in the PowerShell language. My original plan was to write content about PowerShell in the GitHub repository. But PowerShell is a massive topic and there will always be higher priority content to create that is specifically about C# and .NET. In the next edition I will just reference the official PowerShell documentation: https://learn.microsoft.com/en-us/powershell/ And I will remove **Exercise 7.3** that suggests exploring PowerShell.

# Page 357 - Working with complex numbers

> Thanks to [Masoud Nazari](https://github.com/MAS-OUD) for raising this [issue on 25 March 2023](https://github.com/markjprice/cs11dotnet7/issues/50).

In Step 2, I show the default formatting for complex numbers i.e. using round brackets and commas, as well as a custom format, as shown in the following output:
```
(4, 2) added to (3, 7) is (7, 9)
4 + 2i added to 3 + 7i is 7 + 9i
```

> See the official documentation for the `Complex.ToString` method here: https://learn.microsoft.com/en-us/dotnet/api/system.numerics.complex.tostring

Although this is the behavior in .NET 6, in .NET 7 (and .NET 8 previews), the formatting of complex numbers uses angle brackets and semi-colons, as shown in the following output:
```
<4; 2> added to <3; 7> is <7; 9>
4 + 2i added to 3 + 7i is 7 + 9i
```

In the next edition, I will add a note about this. Since the official documentation still shows the behavior of .NET 6, this seems odd. My guess is that they decided to change to angle brackets and semi-colons because some cultures use round brackets to indicate negative numbers and use commas for decimal numbers. Therefore it would be confusing to have a mix of round brackets and commas meaning different things. Its a shame the documentation does not explain this and show the .NET 7 and later new default formats.

# Page 362 - Joining, formatting, and other string members

In the table, `string.IsNullOrWhitespace` should be `string.IsNullOrWhiteSpace`.

# Page 399 - Managing directories

> Thanks to [Dario Bosco](https://github.com/DarioBosco) for raising this [issue on 6 February 2023](https://github.com/markjprice/cs11dotnet7/issues/26).

In Step 1, in the second bullet, I wrote, "Check for the existence of the custom directory path using the `Exists` method of the 
`Directory` class." But in the code I used the `Exists` method of the `Path` class. We have statically imported both the `Path` and the `Directory` classes and they both have an `Exists` method in .NET 7. If we try to call an `Exists` method without a classname prefix we get a compile error due to ambiguity of which one to call. After writing the second bullet text, I changed the code from using `Directory` to using `Path` simply because it is shorter. In the 8th edition, I will add a note about this since it is useful for the reader to understand my choice and how the reader could have done it differently.

> Note: the `Path.Exists` method was added in .NET 7. It is not available in earlier versions of .NET.

# Page 412 - Compressing streams

> Thanks to Bob Molloy for raising this issue via email.

In Step 2, the following statement enables interpolated strings unnecessarily:
```cs
WriteLine($"The compressed contents:");
```

It should be:
```cs
WriteLine("The compressed contents:");
```

# Page 454 - Scaffolding models using an existing database

> Thanks to [Masoud](https://github.com/MAS-OUD) for raising this [issue on 6 April 2023](https://github.com/markjprice/cs11dotnet7/issues/54).

## Category class changes

In Step 5, I show the class that represents a `Category` in the Northwind database that is generated by the `dotnet-ef`, as shown in the following code:
=======
# Page 56 - Managing data with Transact-SQL

The link to the SQL language reference is broken in the PDF version due to a line break. It should be: 
https://learn.microsoft.com/en-us/sql/t-sql/language-reference.

# Page 82 - Defining the Northwind database model

> Thanks to [Bob Molloy](https://github.com/BobMolloy) for raising this [issue on 31 December 2022](https://github.com/markjprice/apps-services-net7/issues/5).

## Category class changes

In Step 7, I show the class that represents a `Category` in the Northwind database that is generated by the `dotnet-ef`, as shown in the following code:
>>>>>>> 091557b2512ff8a35396401db8beabff605c8c3d
```cs
using System;
using System.Collections.Generic;
using System.ComponentModel.DataAnnotations;
using System.ComponentModel.DataAnnotations.Schema;
using Microsoft.EntityFrameworkCore;

<<<<<<< HEAD
namespace WorkingWithEFCore.AutoGen
=======
namespace Northwind.Console.EFCore.Models
>>>>>>> 091557b2512ff8a35396401db8beabff605c8c3d
{
  [Index("CategoryName", Name = "CategoryName")]
  public partial class Category
  {
    public Category()
    {
      Products = new HashSet<Product>();
    }

    [Key]
    public int CategoryId { get; set; }

    [StringLength(15)]
<<<<<<< HEAD
    public string CategoryName { get; set; }
=======
    public string CategoryName { get; set; } = null!;
>>>>>>> 091557b2512ff8a35396401db8beabff605c8c3d

    [Column(TypeName = "ntext")]
    public string? Description { get; set; }

    [Column(TypeName = "image")]
    public byte[]? Picture { get; set; }

    [InverseProperty("Category")]
    public virtual ICollection<Product> Products { get; set; }
  }
}
```
The current `dotnet-ef` tool generates slightly different output, for example, it uses a file-scoped namespace declaration to avoid indenting and it initializes the `Products` property to a `List<T>` instead of a `HashSet<T>`, as shown in the following code:
```cs
using System;
using System.Collections.Generic;
using System.ComponentModel.DataAnnotations;
using System.ComponentModel.DataAnnotations.Schema;
using Microsoft.EntityFrameworkCore;

<<<<<<< HEAD
namespace WorkingWithEFCore.AutoGen;
=======
namespace Northwind.Console.EFCore.Models;
>>>>>>> 091557b2512ff8a35396401db8beabff605c8c3d

[Index("CategoryName", Name = "CategoryName")]
public partial class Category
{
  [Key]
  public int CategoryId { get; set; }

  [StringLength(15)]
  public string CategoryName { get; set; } = null!;

  [Column(TypeName = "ntext")]
  public string? Description { get; set; }

  [Column(TypeName = "image")]
  public byte[]? Picture { get; set; }

  [InverseProperty("Category")]
  public virtual ICollection<Product> Products { get; } = new List<Product>();
}
```

## NorthwindDb class changes

<<<<<<< HEAD
In Step 7, I show the class that represents the Northwind database that was generated by the `dotnet-ef` tool. The current `dotnet-ef` tool generates slightly different output, for example, it uses a file-scoped namespace declaration to avoid indenting and it does not set each `DbSet<T>` property to the null-forgiving operator, as shown in the following code:
=======
In Step 9, I show the class that represents the Northwind database that was generated by the `dotnet-ef` tool. The current `dotnet-ef` tool generates slightly different output, for example, it uses a file-scoped namespace declaration to avoid indenting and it does not set each `DbSet<T>` property to the null-forgiving operator, as shown in the following code:
>>>>>>> 091557b2512ff8a35396401db8beabff605c8c3d
```cs
// older version of dotnet-ef did this:
public virtual DbSet<Category> Categories { get; set; } = null!;

// current version of dotnet-ef does this:
public virtual DbSet<Category> Categories { get; set; }
```

<<<<<<< HEAD
# Page 477 - Inserting entities

> Thanks to [Chadwick Geyser](https://github.com/chadgdotme) for raising this [issue on 29 November 2022](https://github.com/markjprice/cs11dotnet7/issues/5).

In Step 4, the code statement to list the products uses an older version of the method signature that I removed before publishing that only allows a single `productId` to be highlighted, as shown in the following code:
```cs
ListProducts(productIdToHighlight: resultAdd.productId);
```
It should use the method signature that allows multiple `productIds` to be highlighted, as shown in the following code:
```cs
ListProducts(productIdsToHighlight: new[] { resultAdd.productId });
```

# Page 478 - Updating entities

> Thanks to [Masoud](https://github.com/MAS-OUD) for raising this [issue on 11 April 2023](https://github.com/markjprice/cs11dotnet7/issues/57).

In Step 2, the statement to output the price increase, as shown in the following code:
```cs
WriteLine("Increase price success for ID: {resultUpdate.productId}.");
```

Is missing the `$` prefix to make it an interpolated string, as shown in the following code:
```cs
WriteLine($"Increase price success for ID: {resultUpdate.productId}.");
```

# Page 495 - Filtering entities with Where

> Thanks to [Masoud](https://github.com/MAS-OUD) for raising this [issue on 20 April 2023](https://github.com/markjprice/cs11dotnet7/issues/62).

In Steps 3 and 5, the screenshots in *Figure 11.1* and *Figure 11.2* show a solution name of **Chapter12** when it should be **Chapter11**. In the next edition, I will retake the screenshots.

# Page 515 - Be careful with Count!

> Thanks to Clint Mayers who submitted this issue via email.

I showed a code teaser by Amichai Mantinband, a software engineer at Microsoft, as shown in the following code:
```cs
IEnumerable<Task> tasks = Enumerable.Range(0, 2)
  .Select(_ => Task.Run(() => Console.WriteLine("*")));

await Task.WhenAll(tasks);
Console.WriteLine($"{tasks.Count()} stars!");
```

But I mistakenly used `WriteLine` methods when they should have been `Write` methods, as shown in the following code:
```cs
IEnumerable<Task> tasks = Enumerable.Range(0, 2)
  .Select(_ => Task.Run(() => Console.Write("*")));

await Task.WhenAll(tasks);
Console.Write($"{tasks.Count()} stars!");
```
# Page 548 - Creating a class library for a Northwind database context

In Step 11, you write an extension method that registers the `NorthwindContext` class for use as a dependency service. In later chapters, this will be used in ASP.NET Core and Blazor projects. By default, a `DbContext` class is registered using `Scope` lifetime, meaning that multiple threads can share the same instance. If more than one thread attempts to use the same `NorthwindContext` class instance at the same time then you will see the following runtime exception thrown:

> "A second operation started on this context before a previous operation completed. This is usually caused by different threads using the same instance of a DbContext, however instance members are not guaranteed to be thread safe."

To avoid this, we should register the `NorthwindContext` class with a `Transient` lifetime, as shown in the following code:
```cs
using Microsoft.EntityFrameworkCore; // UseSqlite
using Microsoft.Extensions.DependencyInjection; // IServiceCollection

namespace Packt.Shared;

public static class NorthwindContextExtensions {
  /// <summary>
  /// Adds NorthwindContext to the specified IServiceCollection. Uses the Sqlite database provider.
  /// </summary>
  /// <param name="services"></param>
  /// <param name="relativePath">Set to override the default of ".."</param>
  /// <param name="databaseFilename">Set to override the default of "Northwind.db"</param>
  /// <returns>An IServiceCollection that can be used to add more services.</returns>
  public static IServiceCollection AddNorthwindContext(
    this IServiceCollection services, 
    string relativePath = "..",
    string databaseFilename = "Northwind.db") {

    string databasePath = Path.Combine(relativePath, databaseFilename);
    
    services.AddDbContext<NorthwindContext>(options => {
      options.UseSqlite($"Data Source={databasePath}");
      options.LogTo(Console.WriteLine,
      new[] { Microsoft.EntityFrameworkCore.Diagnostics.RelationalEventId.CommandExecuting });

    }, 
    // Register with a transient lifetime to avoid concurrency issues in Blazor Server projects.
    contextLifetime: ServiceLifetime.Transient, optionsLifetime: ServiceLifetime.Transient);

    return services;
  }
}
```

# Page 550 - Creating a class library for entity models using SQL Server

> Thanks to Amer Cejudo for raising this issue by email on 8 April 2023.

In Step 6, I tell the reader to enter a command to generate code from an existing SQL Server database, as shown in the following command:
```
dotnet ef dbcontext scaffold "Data Source=.;Initial Catalog=Northwind;Integrated Security=true;" Microsoft.EntityFrameworkCore.SqlServer --namespace Packt.Shared --data-annotations
```

If you get the error, "The certificate chain was issued by an authority that is not trusted.", then it is because the connection to the SQL Server database will be encrypted by default but the OS and therefore the app does not (yet) trust the local development server certificate. 

You have three choices to fix this issue:

1. Add the following to the database connection string to make the certicate trusted for this connection:
```
TrustServerCertificate=true;
```

2. Add the following to the database connection string to disable encryption so it does not need to trust the certificate for this connection:
```
Encrypt=false;
```

3. Run the following at the command-line to trust the certificate for all .NET apps in future:
```
dotnet dev-certs https --trust
```

# Page 551 - Creating a class library for entity models using SQL Server

In Step 15, you write an extension method that registers the `NorthwindContext` class for use as a dependency service. In later chapters, this will be used in ASP.NET Core and Blazor projects. By default, a `DbContext` class is registered using `Scope` lifetime, meaning that multiple threads can share the same instance. If more than one thread attempts to use the same `NorthwindContext` class instance at the same time then you will see the following runtime exception thrown:

> "A second operation started on this context before a previous operation completed. This is usually caused by different threads using the same instance of a DbContext, however instance members are not guaranteed to be thread safe."

To avoid this, we should register the `NorthwindContext` class with a `Transient` lifetime, as shown in the following code:
```cs
using Microsoft.EntityFrameworkCore; // UseSqlServer
using Microsoft.Extensions.DependencyInjection; // IServiceCollection

namespace Packt.Shared;

public static class NorthwindContextExtensions {
  /// <summary>
  /// Adds NorthwindContext to the specified IServiceCollection. Uses the SqlServer database provider.
  /// </summary>
  /// <param name="services"></param>
  /// <param name="connectionString">Set to override the default.</param>
  /// <returns>An IServiceCollection that can be used to add more services.</returns>
  public static IServiceCollection AddNorthwindContext(
    this IServiceCollection services,
    string connectionString = "Data Source=.;Initial Catalog=Northwind;" +
     "Integrated Security=true;MultipleActiveResultsets=true;Encrypt=false") {
    
    services.AddDbContext<NorthwindContext>(options => {
      options.UseSqlServer(connectionString);
      options.LogTo(Console.WriteLine,
        new[] { Microsoft.EntityFrameworkCore.Diagnostics.RelationalEventId.CommandExecuting });
    }, 
    // Register with a transient lifetime to avoid concurrency issues Blazor Server projects.
    contextLifetime: ServiceLifetime.Transient, optionsLifetime: ServiceLifetime.Transient);

    return services;
  }
}
```

> Note that I have also written a related improvement here: https://github.com/markjprice/cs11dotnet7/blob/main/docs/errata/improvements.md#page-551---creating-a-class-library-for-entity-models-using-sql-server

# Page 623 - Views

> Thanks to Peter Haugstad for sending this issue via email on December 5, 2023.

At the bottom of page 623, I wrote, "The `<a>` elements use Tag Helper attributes named `asp-controller` and `asp-action` to specify the controller name and action name that will execute when the link is clicked on. If you want to navigate to a feature in a Razor Class Library, like the employees component that you created in the previous chapter, then you use `asp-area` to specify the feature name."

I mixed up incompatible technologies. The `<a>` Tag Helper only works with MVC, not Razor Pages. My example of the employees component was therefore wrong because it is a Razor Page component, not an MVC component. You cannot set the `asp-controller` and `asp-action` attributes to navigate to the employees component. 

If you want to navigate to the employees component from an MVC view, then you must use similar syntax to what we used in *Chapter 13*, as shown in the following markup without Tag Helpers:
```html
<a class="btn btn-primary" href="packtfeatures/employees">
  Contact our employees
</a>
```

In the next edition, I will delete the following sentence, "If you want to navigate to a feature in a Razor Class Library, like the employees component that you created in the previous chapter, then you use `asp-area` to specify the feature name."

# Page 627 - Defining a typed view

> Thanks to [Chadwick Geyser](https://github.com/chadwickgeyser) for raising this [issue on 4 December 2022](https://github.com/markjprice/cs11dotnet7/issues/6).

In Step 3, the code in the book to render the carousel indicators has an incorrect attribute named `data-slide-to`, as shown in the following markup:
```xml
<li data-bs-target="#categories" data-slide-to="@c" 
    class="@currentItem"></li>
```

Should be `data-bs-slide-to`, as shown in the following markup:
```xml
<li data-bs-target="#categories" data-bs-slide-to="@c" 
    class="@currentItem"></li>
```

It was already correct in the GitHub copy of the code.

# Page 631 - Passing parameters using a route value

> Thanks to Bob Molloy for raising this issue via email.

In Step 3, the statements attempt to output the values of the category name and unit price for the product, as shown in the following markup:
```xml
<dt>Category</dt>
<dd>@Model.CategoryId - @Model.Category.CategoryName</dd>
<dt>Unit Price</dt>
<dd>@Model.UnitPrice.Value.ToString("C")</dd>
```
But since the `Category` and `UnitPrice` properties could be null, we should use a null checks, as shown in the following markup:
```xml
<dt>Category</dt>
<dd>@Model.CategoryId - @Model.Category?.CategoryName</dd>
<dt>Unit Price</dt>
<dd>@(Model.UnitPrice is null ? "zero" : Model.UnitPrice.Value.ToString("C"))</dd>
```

# Page 641 - Enabling role management and creating a role programmatically

> Thanks to Bob Molloy for raising this issue via email.

In Step 2, in the `Index` action method, the variable declaration for finding the email of the user is not nullable, as shown in the following code:
```cs
IdentityUser user = await userManager.FindByEmailAsync(UserEmail);
```

It should be nullable, as shown in the following code:
```cs
IdentityUser? user = await userManager.FindByEmailAsync(UserEmail);
```

It was already correct in the GitHub copy of the code.

# Page 649 - Varying cached data by query string

> Thanks to [Chadwick Geyser](https://github.com/chadwickgeyser) for raising this [issue on 5 December 2022](https://github.com/markjprice/cs11dotnet7/issues/7).

In Step 1, when defining a policy for output caching, the statement uses the method `VaryByQuery`, as shown in the following code:
```cs
options.AddPolicy("views", p => p.VaryByQuery(""));
```

The method name changed in Release Candidate 2, as described [here](https://learn.microsoft.com/en-us/dotnet/core/compatibility/aspnet-core/7.0/output-caching-renames), so statement should be changed to use the new method `SetVaryByQuery`, as shown in the following code:
```cs
options.AddPolicy("views", p => p.SetVaryByQuery(""));
```

# Page 707 - Reviewing the Blazor Server project template

> Thanks to [Bob Molloy](https://github.com/BobMolloy) for raising this [issue on 19 December 2022](https://github.com/markjprice/cs11dotnet7/issues/12).

In Steps 6 and 7, I wrote that there are two files that combine to product the home page for a Blazor Server project, named `_Host.cshtml` and `_Layout.cshtml`. 

Microsoft changed this project template to merge them together so there is no shared layout file named `_Layout.cshtml`. The markup is now all in the `_Host.cshtml` file, as shown in the following markup:
```html
@page "/"
@using Microsoft.AspNetCore.Components.Web
@namespace Northwind.BlazorServer.Pages
@addTagHelper *, Microsoft.AspNetCore.Mvc.TagHelpers

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <base href="~/" />
    <link rel="stylesheet" href="css/bootstrap/bootstrap.min.css" />
    <link href="css/site.css" rel="stylesheet" />
    <link href="Northwind.BlazorServer.styles.css" rel="stylesheet" />
    <link rel="icon" type="image/png" href="favicon.png"/>
    <component type="typeof(HeadOutlet)" render-mode="ServerPrerendered" />
</head>
<body>
    <component type="typeof(App)" render-mode="ServerPrerendered" />

    <div id="blazor-error-ui">
        <environment include="Staging,Production">
            An error has occurred. This application may no longer respond until reloaded.
        </environment>
        <environment include="Development">
            An unhandled exception has occurred. See browser dev tools for details.
        </environment>
        <a href="" class="reload">Reload</a>
        <a class="dismiss">🗙</a>
    </div>

    <script src="_framework/blazor.server.js"></script>
</body>
</html>
```

# Page 724 - Getting entities into a component

> Thanks to Amer Cejudo (via email) and [Christopher Targett-Adams](https://github.com/targettadams) for raising this [issue on 20 February 2023](https://github.com/markjprice/cs11dotnet7/issues/31).

In Step 4, I tell the reader to write a statement to call an extension method that you previously created in Chapter 12, as shown in the following code:
```cs
builder.Services.AddNorthwindContext();
```

By default, this statement registers the database context with `Scope` lifetime. This is not a problem with most ASP.NET Core projects. But in a **Blazor Server** project the `Scope` lifetime database context instance is shared between multiple threads running on the server. This can cause concurrency issues as described here: 
https://learn.microsoft.com/en-us/ef/core/dbcontext-configuration/#implicitly-sharing-dbcontext-instances-via-dependency-injection

This often only affects the SQL Server database provider but it is best to apply the code change for both SQL Server and SQLite class libraries. To fix this issue, please make the changes as shown in the following items:
- [Page 548 - Creating a class library for a Northwind database context](#page-548---creating-a-class-library-for-a-northwind-database-context)
- [Page 551 - Creating a class library for entity models using SQL Server](#page-551---creating-a-class-library-for-entity-models-using-sql-server)

# Page 733 - Building customer create, edit, and delete components

> Thanks to [Bob Molloy](https://github.com/BobMolloy) for raising this [issue on 27 December 2022](https://github.com/markjprice/cs11dotnet7/issues/15).

In Step 4, in the file named `EditCustomer.razor`, the code for the `Update` method is missing the last statement to navigate to the `customers` page component after updating the customer in the database, as shown in the following code:
```cs
private async Task Update()
{
  if (customer is not null)
  {
    await service.UpdateCustomerAsync(customer);
  }

  navigation.NavigateTo("customers");
}
```
=======
We asked the compiler to treat warnings as errors so we cannot build until the compiler knows that all those 25+ properties are safe to use as `null`. We could manually add the null-forgiving operator, or use a find and replace regular expression to do it, or customize the T4 template used by the `dotnet-ef` tool to set all `DbSet<T>` properties to the null-forgiving operator, but the easiest thing to do is simply disable null warnings for this file by adding the following statement to the top of the class file, as shown in the following code:
```cs
#nullable disable
```

Microsoft recommends either setting `DbSet<T>` properties to the null-forgiving operator, or calling the `Set<T>` method defined in the `DbContext` base class to implement them as a read-only property, as shown in the following code:
```cs
public virtual DbSet<Category> Categories => Set<Category>();
```

**Working with Nullable Reference Types - DbContext and DbSet**
https://learn.microsoft.com/en-us/ef/core/miscellaneous/nullable-reference-types#dbcontext-and-dbset

> Thanks to [charlygg](https://github.com/charlygg) for suggesting using the `Set<T>` method in a comment on [issue on 1 January 2023](https://github.com/markjprice/apps-services-net7/issues/5#issuecomment-1368614033).

# Page 91 - Table-per-concrete-type (TPC) mapping strategy

> Thanks to [Jorge Morales](https://github.com/jmoralesv) for raising this [issue on December 12, 2023](https://github.com/markjprice/apps-services-net7/issues/22).

I show the SQL to define the two tables used in the TPC mapping strategy but it includes a foreign key constraint to a `People` table that does not exist, as shown in the following code:

```sql
CREATE TABLE [Students] (
  [Id] int NOT NULL DEFAULT (NEXT VALUE FOR [PersonIds]),
  [Name] nvarchar(max) NOT NULL,
  [Subject] nvarchar(max) NULL,
  CONSTRAINT [PK_Students] PRIMARY KEY ([Id])
  CONSTRAINT [FK_Students_People] FOREIGN KEY ([Id]) REFERENCES [People] ([Id])
);

CREATE TABLE [Employees] (
  [Id] int NOT NULL DEFAULT (NEXT VALUE FOR [PersonIds]),
  [Name] nvarchar(max) NOT NULL,
  [HireDate] nvarchar(max) NULL,
  CONSTRAINT [PK_Employees] PRIMARY KEY ([Id])
  CONSTRAINT [FK_Employees_People] FOREIGN KEY ([Id]) REFERENCES [People] ([Id])
);
```

I mistakenly copied some of the SQL from another strategy. In the next edition, I will correct the SQL, as shown in the following code:

```sql
CREATE TABLE [Employees] (
  [Id] int NOT NULL DEFAULT (NEXT VALUE FOR [PersonIds]),
  [Name] nvarchar(40) NOT NULL,
  [HireDate] datetime2 NOT NULL,
  CONSTRAINT [PK_Employees] PRIMARY KEY ([Id])
);

CREATE TABLE [Students] (
  [Id] int NOT NULL DEFAULT (NEXT VALUE FOR [PersonIds]),
  [Name] nvarchar(40) NOT NULL,
  [Subject] nvarchar(max) NULL,
  CONSTRAINT [PK_Students] PRIMARY KEY ([Id])
);
```

After the note saying, "Since there is not a single table with an IDENTITY column to assign Id values, we can use the (NEXT VALUE FOR [PersonIds]) command to define a sequence shared between the two tables so they do not assign the same Id values." I will show the SQL to define the sequence, as shown in the following code:

```sql
CREATE SEQUENCE [PersonIds] AS int START WITH 4 INCREMENT BY 1 NO MINVALUE NO MAXVALUE NO CYCLE;
```

# Page 102 - Creating a class library for the data context using SQL Server

In Step 1, I wrote, "In Visual Studio Code, select `Northwind.Common.DataContext.SqlServer` as the active OmniSharp project." 

This works if you installed the most recent release version `1.25.9`. But if you installed the pre-release version `2.0.x` then it does not include OmniSharp any more.

To follow the instructions in the book, if you have installed the pre-release version `2.0.x` then on the **C#** extension page, I recommend that you click the button **Switch to Release Version** to revert back to the current release version `1.25.9`.

# Page 138 - Performing CRUD operations with Cosmos SQL API

In Step 8, a long block of code tries to copy `Product` instances and their related `Category` and `Supplier` entities into Cosmos DB. Although the code uses `Where` to filter only products that have a non-null category and supplier, the compiler is not smart enough to detect this, and gives warnings about potential `null` value assignment. 

The following statement:
```cs
category = new CategoryCosmos
```
Can be changed to the following:
```cs
// If the related category is null, store null,
// else store the category mapped to Cosmos model.
category = p.Category == null ? null :
  new CategoryCosmos
```

And the following statement:
```cs
supplier = new SupplierCosmos
```
Can be changed to the following:
```cs
supplier = p.Supplier == null ? null :
  new SupplierCosmos
```

This change has been made in the 2nd edition, found at the following link: https://github.com/markjprice/apps-services-net8/blob/main/code/Chapter04/Northwind.CosmosDb.SqlApi/Program.Methods.cs#L149

# Page 200 - Testing an AutoMapper configuration

> Thanks to Doug Murphy for raising this issue via email.

In the note at the top of page 200, I wrote, "For the entity models, we used records because they will be immutable. But an 
instance of `Summary` will be created and then its members populated automatically by AutoMapper, so it must be a normal mutable class with public properties that can be set."

But records are not always immutable. They are immutable in this scenario due to the way I defined them. It is possible to define mutable records. For example:
```cs
// As defined in the book. This will not work because it // only has a 
// constructor with two parameters. AutoMapper needs to call a default 
// constructor (no parameters) and then set the properties.
public record Summary(string? FullName, decimal Total);

// This works because it has a default constructor and due to the init 
// keywords. After constructing an instance, the properties can be set,
// but after that, the properties cannot be changed.
public record Summary 
{
  public string? FullName { get; init; }
  public decimal Total { get; init; }
}
```

In the next edition, I will use the `init` style to define the `Summary` record.

# Page 254 - Localizing the DayOfWeek enum

> Thanks to [Stephen Harper](https://github.com/sjharper79) for raising this [issue on 15 December 2023](https://github.com/markjprice/apps-services-net7/issues/23).

At the top of the page I show a statement to output the current day of the week, as shown in the following code:
```cs
WriteLine($"The day of the week is {0:dddd}.", DateTime.Now);
```
But that code mixes string interpolation e.g. `$` and string positional format e.g. `{0}`. 

In the 2nd edition, I changed the statement to use string interpolation, as shown in the following code:
```cs
WriteLine($"The day of the week is {DateTime.Now:dddd}.");
```

# Page 350 - Rate limiting using ASP.NET Core middleware

> Thanks to `JimCampbell63` in the Discord channel for highlighting this issue.

In Step 1, I instruct the reader to add a package reference for `Microsoft.AspNetCore.RateLimiting`. This was necessary up to the release candidate, but for the GA release of .NET 7, the team added the functionality to the main libraries so it is not necessary to reference a package or rebuild the project in Step 2.

# Page 411 - Using an ASP.NET Core MVC project as a GraphQL client

> Thanks to [mdevol58](https://github.com/mdevol58) for raising this [issue on 14 August 2023](https://github.com/markjprice/apps-services-net7/issues/18).

In Step 12, I wrote, "In the `Controllers` folder, in `HomeController.cs`, import the namespace for working with text encodings and for our Northwind entity models".

I should have written, "In the `Controllers` folder, in `HomeController.cs`, import the namespace for working with text 
encodings and for the local project models", and add the missing import statement for the models, as shown in the following code:
```cs
using Northwind.Mvc.GraphQLClient.Models; // IndexViewModel, ResponseProducts and so on
using System.Text; // Encoding
```

# Page 417 - Understanding Strawberry Shake - Creating a console app client

In Step 4, you add references to two StrawberryShake packages. I had hoped that version 13 would be released by now, but it is still in preview for one of those packages and is not available at all for the other. I therefore recommend that you use version 12.16.0, as shown in the following markup:

```xml
<ItemGroup>
  <PackageReference Include="Microsoft.Extensions.DependencyInjection" Version="7.0.0" />
  <PackageReference Include="Microsoft.Extensions.Http" Version="7.0.0" />
  <PackageReference Include="StrawberryShake.CodeGeneration.CSharp.Analyzers" Version="12.16.0" />
  <PackageReference Include="StrawberryShake.Transport.Http" Version="12.16.0" />
</ItemGroup>
```

> ChilliCream recommends that you always use the same versions when referencing multiple of their packages to ensure they work together properly.

In Step 9, you add a file named `seafoodProducts.graphql`. After creating this file, review the project file to check for an entry to explicitly remove this file from the build process, as shown in the following markup: 
```xml
<ItemGroup>
  <GraphQL Remove="seafoodProducts.graphql" />
</ItemGroup>
```

There must be at least one .graphql file for the Strawberry Shake tool to be able to generate its code automatically. So this entry will prevent the Strawberry Shake tool from generating its code and you will later get compile errors. You should delete or comment out that entry, as shown in the following markup:
```xml
<!--<ItemGroup>
  <GraphQL Remove="seafoodProducts.graphql" />
</ItemGroup>-->
```

# Page 419 - Understanding Strawberry Shake - Creating a console app client

> thanks to [Stephen Harper](https://github.com/sjharper79) for raising this issue and finding a solution on [December 25, 2023](https://github.com/markjprice/apps-services-net7/issues/25).

In Step 10, when you build the console app, you might see the following error:
```
SS0006: Access to the path 'obj\berry' is denied.
SS0006: Method not found: 'Void StrawberryShake.CodeGeneration.CSharp.CSharpGeneratorSettings.set_RequestStrategy(StrawberryShake.Tools.Configuration.RequestStrategy)'
```

To fix the error, in the project file, in a `<PropertyGroup>`, add the following markup:
```xml
<StrawberryShake_State>$(MSBuildProjectExtensionsPath)berry</StrawberryShake_State>
```

You can read more about this at the following link: https://stackoverflow.com/questions/75693518/c-sharp-net-build-error-due-to-strawberry-shake-graphql-client-error-access.

# Page 467 - Adding a chat page to the MVC website

In Step 2, in a JavaScript file named `chat.js`, I tell the reader to add statements to add events handlers for the **Register** and **Send** buttons, and so on. One of those statements uses a backtick \` to enable JavaScript interpolated strings that use curly brackets `{}` for dynamic placeholders. 

But after submitting final drafts in a Word document, a Packt process replaced the backtick characters with single straight quote `'` characters. This disabled the interpolated strings. I had even added a comment to explain to the reader that they should use a backtick character but the Packt process replaced that too! 

Incorrect code in the print book in the comment and string value:
```cs
// note the use of backtick ' to enable a formatted string
li.textContent =
  'To ${received.to}, From ${received.from}: ${received.body}';
```

The statement should be as follows:

```cs
// note the use of backtick ` to enable a formatted string
li.textContent =
  `To ${received.to}, From ${received.from}: ${received.body}`;
```

Luckily, the code was correct in the GitHub repository:
https://github.com/markjprice/apps-services-net7/blob/main/vs4win/Chapter13/Northwind.SignalR.Service.Client.Mvc/wwwroot/js/chat.js#L28

# Page 508 - Implementing a function that works with queues and BLOBs

> Thanks to [Jim Campbell](https://github.com/jimcbell) who raised this issue and provided solutions on [December 24, 2023](https://github.com/markjprice/apps-services-net7/issues/24).

In Step 4, I tell the reader to "add package references for working with ... drawing with ImageSharp" and the markup shows the version current at the time of publishing in November 2022, version `2.1.3` and `1.0.0-*`. If you use those versions then everything works as in the book. But if you use the latest versions, there are some changes to the ImageSharp API, for example, the `IPen` and `IBrush` interfaces have been removed.

In Step 11, this can be fixed by making the types for the objects used for drawing `Pen` and `Brush`, as shown in the following code:
```cs
// define some pens and brushes
Pen blackPen = Pens.Solid(Color.Black, 2); 
Pen blackThickPen = Pens.Solid(Color.Black, 8); 
Pen greenPen = Pens.Solid(Color.Green, 3); 
Brush redBrush = Brushes.Solid(Color.Red); 
Brush blueBrush = Brushes.Solid(Color.Blue);
```

Also, the signature of the `DrawText` method no longer takes a `TextOptions` object. Instead it should be a `RichTextOptions`, as shown in the following code:

```cs
RichTextOptions textOptions = new(font)
{
  Origin = new PointF(100, 200),
  WrappingLength = 1000,
  HorizontalAlignment = HorizontalAlignment.Left
};

image.Mutate(x => x.DrawText(
  textOptions, amount, blueBrush, blackPen));
```

There is also an issue if running on Mac or Linux because I hardcoded the path to the fonts with the Windows path separator, as shown in the following code:
```cs
FontFamily family = collection.Add(
  @"fonts\Caveat\static\Caveat-Regular.ttf");
```

I should have used cross-platform technique to build the path, as shown in the following code:
```cs
string pathToFont = System.IO.Path.Combine("fonts", "Caveat", "static", "Caveat-Regular.ttf");

FontFamily family = collection.Add(pathToFont);
```

And to build the paths to the local folder to write the blob to, as shown in the following code:
```cs
if (System.Environment.GetEnvironmentVariable("IS_LOCAL") == "true")
{
  // create blob in the local filesystem
  string folder = System.IO.Path.Combine(System.Environment.CurrentDirectory, "blobs");
  if (!Directory.Exists(folder))
  {
    Directory.CreateDirectory(folder);
  }

  log.LogInformation($"Blobs folder: {folder}");

  string blobPath = System.IO.Path.Combine(folder,blobName);

  await image.SaveAsPngAsync(blobPath);
}
```

# Page 550 - Understanding the Accept-Language header

> Thanks to [Stephen Harper](https://github.com/sjharper79) for raising this issue on [January 3, 2024](https://github.com/markjprice/apps-services-net7/issues/26).

The third bullet says, "fr-FR;q=0.8: English language in France ranked at 0.8." 

It should say, "fr-FR;q=0.8: French language in France ranked at 0.8."

This has been fixed in the second edition.

# Page 550 - Comparing HTML Helpers and Tag Helpers

> Thanks to [Stephen Harper](https://github.com/sjharper79) for raising this issue on [January 3, 2024](https://github.com/markjprice/apps-services-net7/issues/27).

I show three statements that should produce the following markup:
```html
<a href="/home/privacy">View our privacy policy.</a>
```

But the first two statements use `Index` instead of `Home`. They should be as follows:
```
@Html.ActionLink("View our privacy policy.", "Privacy", "Home")

@Html.ActionLink(linkText: "View our privacy policy.",
  action: "Privacy", controller: "Home")
```

This will be fixed in the third edition.

# Page 571 - Blazor routing to page components

`MainLayout.cshtml` should be `MainLayout.razor`.

# Page 578 - Building Blazor components

> Thanks to [mdevol58](https://github.com/mdevol58) for raising two potential issues on [16 August 2023](https://github.com/markjprice/apps-services-net7/issues/19) and [17 August 2023](https://github.com/markjprice/apps-services-net7/issues/20).

In Step 17, the two elements added are already HTML5-compliant and were copied from [Bootstrap's official template](https://getbootstrap.com/docs/5.2/getting-started/introduction/). But if you need them to be XHTML-compliant then they should be self-closing i.e. they should end with `/>` instead of just `>`, as shown in the following markup:
```html
<meta name="viewport" content="width=device-width, initial-scale=1" />
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-gH2yIJqKdNHPEq0n4Mqa/HGKIhSkIHeL5AyhkYV8i59U5AR6csBvApHHNl/vI1Bx" crossorigin="anonymous" />
```

The second issue that mdevol58 found caused the **Delete Database** dialog not to display. I was not able to reproduce the same error so I cannot confirm the fix. If you have the same issue, try changing the attribute name from `crossorigin` to `crossOrigin`. The official documentation does not say camelCase is required.

# Page 587 - Building and testing a Blazor alert component

> Thanks to [Bob Molloy](https://github.com/BobMolloy) for raising this [issue on 8 February 2023](https://github.com/markjprice/apps-services-net7/issues/9).

In Step 3, the filename `_Imports.cshtml` should be `_Imports.razor`.

# Page 600 - Building a local storage service

In Step 9, the filename `_Imports.cshtml` should be `_Imports.razor`.

# Page 613 - Exploring Radzen Blazor components

> Thanks to [Bob Molloy](https://github.com/BobMolloy) for raising this [issue on 14 March 2023](https://github.com/markjprice/apps-services-net7/issues/11).

In Step 10, the filename `_Imports.cshtml` should be `_Imports.razor`. Also, the text should say, "add statements to import the Radzen and Radzen Blazor namespaces", not just one statement.

# Page 621 - Building a web service for Northwind entities

> Thanks to [Bob Molloy](https://github.com/BobMolloy) for raising this [issue on 14 March 2023](https://github.com/markjprice/apps-services-net7/issues/12).

In Step 6, the statement to include the products is missing a close bracket. It should be as shown:
```cs
app.MapGet("api/categories", (
  [FromServices] NorthwindContext db) => 
    Results.Json(
      db.Categories.Include(c => c.Products)))
  .WithName("GetCategories")
  .Produces<Category[]>(StatusCodes.Status200OK);
```

The GitHub repository code solution used a slightly older version of this code. It has now been updated to match the book, as shown at the following link:
https://github.com/markjprice/apps-services-net7/blob/main/vs4win/Chapter17/Northwind.BlazorLibraries/Server/Program.cs#L44

# Page 623 - Using the Radzen tabs, image, and icon components

> Thanks to [Bob Molloy](https://github.com/BobMolloy) for raising this [issue on 15 March 2023](https://github.com/markjprice/apps-services-net7/issues/13).

In Step 5, `MainLayout.cshtml` should be `MainLayout.razor`.

# Page 627 - Using the Radzen HTML editor component

In Step 3, `MainLayout.cshtml` should be `MainLayout.razor`.

# Page 631 - Using the Radzen chart component

In Step 5, `MainLayout.cshtml` should be `MainLayout.razor`.

# Page 633 - Using the Radzen form components

In Step 1, the statement to define and endpoint for employees manually sets JSON options, as shown in the following code:
```cs
app.MapGet("api/employees/", (
  [FromServices] NorthwindContext db) =>
    Results.Json(db.Employees, jsonOptions))
  .WithName("GetEmployees")
  .Produces<Employee[]>(StatusCodes.Status200OK);
```

It should use the globally configure JSON options, as shown in the following code:
```cs
app.MapGet("api/employees/", (
  [FromServices] NorthwindContext db) =>
    Results.Json(db.Employees))
  .WithName("GetEmployees")
  .Produces<Employee[]>(StatusCodes.Status200OK);
```

# Page 634 - Using the Radzen form components

In Step 2, `MainLayout.cshtml` should be `MainLayout.razor`.

# Page 657 - Creating a virtual Android device for local app testing

> Thanks to [Bob Molloy](https://github.com/BobMolloy) for raising this [issue on 29 March 2023](https://github.com/markjprice/apps-services-net7/issues/15).

In Step 5, **Save** should be **Create**. Also in *Figure 18.2*, the caption of the button should be **Create** instead of **Save**. (I must have edited an existing device instead of creating a new one when taking the screenshot which caused this mistake.)

# Page 667 - Adding shell navigation and more content pages

> Thanks to [Stephen Harper](https://github.com/sjharper79) for raising this [issue on 8 January 2024](https://github.com/markjprice/apps-services-net7/issues/29).

In Step 20, the method name should be `ClickMeButton_Clicked`.
>>>>>>> 091557b2512ff8a35396401db8beabff605c8c3d
