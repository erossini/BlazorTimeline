# Timeline for Blazor

This is a new component for [Blazor WebAssembly](https://www.puresourcecode.com/tag/blazor-webassembly/) and [Blazor Server](https://www.puresourcecode.com/tag/blazor-server/). The components is build with .NET6.

The timeline is responsive and easy to customize. The `Timeline` is configuration with the colors, icon and HTML code. Each `TimelineItem` has properties for changing colors and more features.

<img width="410" alt="Timeline" src="https://user-images.githubusercontent.com/9497415/220400235-903db41b-ef8e-4bd6-b740-ed5c026f9402.png">

For more details about this component, please see this post on [PureSourceCode.com](). 
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
