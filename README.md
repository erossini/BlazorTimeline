# Timeline for Blazor

This is a new component for [Blazor WebAssembly](https://www.puresourcecode.com/tag/blazor-webassembly/) and [Blazor Server](https://www.puresourcecode.com/tag/blazor-server/). The components is build with .NET6.

The timeline is responsive and easy to customize. The `Timeline` is configuration with the colors, icon and HTML code. Each `TimelineItem` has properties for changing colors and more features.

<img width="410" alt="Timeline" src="https://user-images.githubusercontent.com/9497415/220400235-903db41b-ef8e-4bd6-b740-ed5c026f9402.png">

For more details about this component, please see this post on [PureSourceCode.com](https://www.puresourcecode.com/dotnet/blazor/timeline-component-for-blazor/). 
If you need support for this component or you have a suggestion or comment, please use my [Forum](https://www.puresourcecode.com/forum/timeline/).

## Usage

### 1. Install 

This component is a Nuget package available from [this link](https://www.nuget.org/packages/PSC.Blazor.Components.Timeline/).

### 2. Add using to your project.

```html
@using PSC.Blazor.Components.Timeline
@using PSC.Blazor.Components.Timeline.Enums
```

### 3. Example code
```html
@using PSC.Blazor.Components.Timeline

<Timeline ItemPositionOption="@ItemPositionOption.Manual">
    <TimelineItem Title="Start here" Time="@DateTime.Now.ToString("dd/MM/yyyy")" 
        ButtonText="PureSourceCode.com" Link="https://www.puresourcecode.com">
        Here you can write some text. The <code>TimelineItem</code> has 
        the property for adding a button called <code>ButtonText</code>
        and you can add a link with <code>Link</code>.
    </TimelineItem>

    <TimelineItem Title="Custom content" Position="ItemPosition.Right" Icon="Icon.UserTime">
        <span>
            <code>TimelineItem</code> can be altered to appear on the right! 
            Also, you can use the default icon or use one of the embedded icons with <code>Icon</code>.
        </span>

        <span>You can add images or any other HTML code</span> <br />
        <img src="/psc_logo.png" style="max-width: 100%;" />
    </TimelineItem>

    <TimelineItem Title="Documentation" Icon="Icon.Timeline" 
                  ButtonText="Documentation" Link="https://www.puresourcecode.com">
        <span>
            Now, visit the page with the documentation and same examples.
        </span>
    </TimelineItem>

    <TimelineItem TitleBackgroundColor="#70b0ff" TextBackgroundColor="#ffffff" 
                  Title="Forum" Icon="Icon.ReminderClock" ButtonText="Forum" 
                  Link="https://www.puresourcecode.com">
        <span>
            Use the forum to send your comment or submit your questions.
        </span>
    </TimelineItem>
</Timeline>
```

## Timeline properties and methods

### Timeline properties

|   | Name               | Description                                      |
|---|--------------------|--------------------------------------------------|
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | ChildContent	     | Gets or sets the content of the child.           |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | ItemPositionOption | Should items be altered automatically or manual. |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | TextBgColor	       | Description background color.                    |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | TextColor	         | Description text color.                          |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | Title	             | Timeline title which will be displayed above.    |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | TitleBgColor       | Background color for title section.              |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | TitleColor	       | Text color for title section.                    |

### Timeline item properties

|   | Name                | Description                                      |
|---|---------------------|--------------------------------------------------|
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | ButtonText	        | Gets or sets the button text.                    |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | ChildContent	      | Gets or sets the content of the child.           |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | Icon	              | Gets or sets the icon.                           |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | IconContent	        | Gets or sets the content of the icon.            |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | Link	              | Gets or sets the link.                           |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | Position	          | Gets or sets the position.                       |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | TextBackgroundColor	| Gets or sets the color of the text background.   |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | Time                | Gets or sets the time.                           |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | Timeline	          | Gets or sets the timeline.                       |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | Title	              | Title for timeline item                          |
| ![image](https://user-images.githubusercontent.com/9497415/220409836-c7035379-3fb1-48f2-9906-5c799b62e18e.png) | TitleBackgroundColor | Gets or sets the color of the back ground.      |

## Timeline Icon embedded

- Clock
- ClockDateTime
- Default
- DigitalNumber0
- DigitalNumber1
- DigitalNumber2
- DigitalNumber3
- DigitalNumber4
- DigitalNumber5
- DigitalNumber6
- DigitalNumber7
- DigitalNumber8
- DigitalNumber9
- HourGlass
- HourGlassOld
- ReminderClock
- SandClock
- Timeline
- UserTime


---
    
## PureSourceCode.com

[PureSourceCode.com](https://www.puresourcecode.com/) is my personal blog where I publish posts about technologies and in particular source code and projects in [.NET](https://www.puresourcecode.com/category/dotnet/). 

In the last few months, I created a lot of components for [Blazor WebAssembly](https://www.puresourcecode.com/tag/blazor-webassembly/) and [Blazor Server](https://www.puresourcecode.com/tag/blazor-server/).

My name is Enrico Rossini and you can contact me via:
- [Personal Twitter](https://twitter.com/erossiniuk)
- [LinkedIn](https://www.linkedin.com/in/rossiniuk)
- [Facebook](https://www.facebook.com/puresourcecode)

## Blazor Components

| Component name | Forum | NuGet | Website | Description |
|---|---|---|---|---|
| [Browser Detect for Blazor](https://www.puresourcecode.com/dotnet/blazor/browser-detect-component-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/browser-detect-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.BrowserDetect) | [Demo](https://browserdetect.puresourcecode.com) | Browser detect for Blazor WebAssembly and Blazor Server |
| [ChartJs for Blazor](https://www.puresourcecode.com/dotnet/blazor/blazor-component-for-chartjs/) | [Forum](https://www.puresourcecode.com/forum/chart-js-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Chartjs) | [Demo](https://chartjs.puresourcecode.com/) | Add beautiful graphs based on ChartJs in your Blazor application |
| [Clippy for Blazor](https://www.puresourcecode.com/dotnet/blazor/blazor-component-for-chartjs/) | [Forum](https://www.puresourcecode.com/forum/clippy/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Clippy) | [Demo](https://clippy.puresourcecode.com/) | Do you miss Clippy? Here the implementation for Blazor |
| [CodeSnipper for Blazor](https://www.puresourcecode.com/dotnet/blazor/code-snippet-component-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/codesnippet-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.CodeSnippet) | | Add code snippet in your Blazor pages for 196 programming languages with 243 styles |
| [Copy To Clipboard](https://www.puresourcecode.com/dotnet/blazor/copy-to-clipboard-component-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/copytoclipboard/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.CopyToClipboard) | | Add a button to copy text in the clipboard | 
| [DataTable for Blazor](https://www.puresourcecode.com/dotnet/net-core/datatable-component-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/forum/datatables/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.DataTable) | [Demo](https://datatable.puresourcecode.com/) | DataTable component for Blazor WebAssembly and Blazor Server |
| [Icons and flags for Blazor](https://www.puresourcecode.com/forum/icons-and-flags-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/icons-and-flags-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Icons) | | Library with a lot of SVG icons and SVG flags to use in your Razor pages |
| [Markdown editor for Blazor](https://www.puresourcecode.com/dotnet/blazor/markdown-editor-with-blazor/) | [Forum](https://www.puresourcecode.com/forum/forum/markdown-editor-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.MarkdownEditor) | [Demo](https://markdown.puresourcecode.com/) | This is a Markdown Editor for use in Blazor. It contains a live preview as well as an embeded help guide for users. |
| [Modal dialog for Blazor](https://www.puresourcecode.com/dotnet/blazor/modal-dialog-component-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/forum/modal-dialog-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.ModalDialog) | | Simple Modal Dialog for Blazor WebAssembly |
| [Modal windows for Blazor](https://www.puresourcecode.com/dotnet/blazor/modal-dialog-component-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/forum/modal-dialog-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Modals) | | Modal Windows for Blazor WebAssembly |
| [Quill for Blazor](https://www.puresourcecode.com/dotnet/blazor/create-a-blazor-component-for-quill/) | [Forum](https://www.puresourcecode.com/forum/forum/quill-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Quill) | | Quill Component is a custom reusable control that allows us to easily consume Quill and place multiple instances of it on a single page in our Blazor application |
| [ScrollTabs](https://www.puresourcecode.com/dotnet/blazor/scrolltabs-component-for-blazor/) | | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.ScrollTabs) | | Tabs with nice scroll (no scrollbar) and responsive |
| [Segment for Blazor](https://www.puresourcecode.com/dotnet/blazor/segment-control-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/forum/segments-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Segments) | | This is a Segment component for Blazor Web Assembly and Blazor Server |
| [Tabs for Blazor](https://www.puresourcecode.com/dotnet/blazor/tabs-control-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/forum/tabs-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Tabs) | | This is a Tabs component for Blazor Web Assembly and Blazor Server |
| [Timeline for Blazor](https://www.puresourcecode.com/dotnet/blazor/timeline-component-for-blazor/) | [Forum](https://www.puresourcecode.com/forum/timeline/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Timeline) | | This is a new responsive timeline  for Blazor Web Assembly and Blazor Server |
| [Toast for Blazor](https://www.puresourcecode.com/forum/psc-components-and-source-code/) | [Forum](https://www.puresourcecode.com/forum/psc-components-and-source-code/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Toast) | | Toast notification for Blazor applications |
| [Tours for Blazor](https://www.puresourcecode.com/forum/psc-components-and-source-code/) | [Forum](https://www.puresourcecode.com/forum/psc-components-and-source-code/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.Tours) | | Guide your users in your Blazor applications |
| [WorldMap for Blazor]() | [Forum](https://www.puresourcecode.com/forum/worldmap-for-blazor/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Blazor.Components.WorldMap) | [Demo](https://worldmap.puresourcecode.com/) | Show world maps with your data |

## C# libraries for .NET6

| Component name | Forum | NuGet | Description |
|---|---|---|---|
| [PSC.Evaluator](https://www.puresourcecode.com/forum/psc-components-and-source-code/) | [Forum](https://www.puresourcecode.com/forum/forum/psc-extensions/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Evaluator) | PSC.Evaluator is a mathematical expressions evaluator library written in C#. Allows to evaluate mathematical, boolean, string and datetime expressions. |
| [PSC.Extensions](https://www.puresourcecode.com/dotnet/net-core/a-lot-of-functions-for-net5/) | [Forum](https://www.puresourcecode.com/forum/forum/psc-extensions/) | ![NuGet badge](https://img.shields.io/nuget/v/PSC.Extensions) | A lot of functions for .NET5 in a NuGet package that you can download for free. We collected in this package functions for everyday work to help you with claim, strings, enums, date and time, expressions... |

## More examples and documentation
*   [Write a reusable Blazor component](https://www.puresourcecode.com/dotnet/blazor/write-a-reusable-blazor-component/)
*   [Getting Started With C# And Blazor](https://www.puresourcecode.com/dotnet/net-core/getting-started-with-c-and-blazor/)
*   [Setting Up A Blazor WebAssembly Application](https://www.puresourcecode.com/dotnet/blazor/setting-up-a-blazor-webassembly-application/)
*   [Working With Blazor Component Model](https://www.puresourcecode.com/dotnet/blazor/working-with-blazors-component-model/)
*   [Secure Blazor WebAssembly With IdentityServer4](https://www.puresourcecode.com/dotnet/blazor/secure-blazor-webassembly-with-identityserver4/)
*   [Blazor Using HttpClient With Authentication](https://www.puresourcecode.com/dotnet/blazor/blazor-using-httpclient-with-authentication/)
*   [InputSelect component for enumerations in Blazor](https://www.puresourcecode.com/dotnet/blazor/inputselect-component-for-enumerations-in-blazor/)
*   [Use LocalStorage with Blazor WebAssembly](https://www.puresourcecode.com/dotnet/blazor/use-localstorage-with-blazor-webassembly/)
*   [Modal Dialog component for Blazor](https://www.puresourcecode.com/dotnet/blazor/modal-dialog-component-for-blazor/)
*   [Create Tooltip component for Blazor](https://www.puresourcecode.com/dotnet/blazor/create-tooltip-component-for-blazor/)
*   [Consume ASP.NET Core Razor components from Razor class libraries | Microsoft Docs](https://docs.microsoft.com/en-us/aspnet/core/blazor/components/class-libraries?view=aspnetcore-5.0&tabs=visual-studio)
