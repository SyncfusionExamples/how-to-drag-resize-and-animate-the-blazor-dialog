# How to Drag, Resize, and Animate the Blazor Dialog Control

## Overview

This sample demonstrates the Syncfusion [Blazor Dialog](https://www.syncfusion.com/blazor-components/blazor-modal-dialog) component in a Blazor WebAssembly application. The application showcases common dialog interaction scenarios including dragging, resizing, positioning, animation effects, custom dialog creation, and displaying multiple dialogs.

These capabilities help developers create flexible popup experiences that improve usability and allow end users to interact with dialogs more efficiently. The sample serves as a practical reference for implementing interactive dialog behavior in modern Blazor applications.

## Key Features

- Uses the Syncfusion Blazor `SfDialog` component to display a newsletter subscription form.
- Enables dialog dragging through the `AllowDragging="true"` property, allowing users to reposition the dialog within the target container.
- Supports dialog resizing using `EnableResize="true"` and `ResizeHandles`, configured with `ResizeDirection.All` for resizing from any edge or corner.
- Positions the primary dialog in the top-left area of the target container using `DialogPositionData` with `X="Left"` and `Y="Top"`.
- Applies dialog opening and closing animations through `DialogAnimationSettings` using the `DialogEffect.FlipXUp` animation effect.
- Uses dialog header, content, and footer customization through `DialogTemplates`.
- Integrates an `SfTextBox` component with two-way data binding using `@bind-Value` to collect subscriber email input.
- Uses an `SfButton` component to trigger subscription actions through the `SubscribeButtonClick` event handler.
- Displays a secondary confirmation dialog using a second `SfDialog` component.
- Controls dialog visibility dynamically through `@bind-Visible="SuccessDialogVisibility"`.
- Implements dialog button actions using `DialogButton` and the `CloseButtonClick` event handler.
- Clears the textbox value and closes the confirmation dialog after a successful close action.
- Demonstrates interaction between multiple dialog instances within the same page.
- Includes custom styling for dialog headers, content, footer layout, buttons, and dialog appearance using page-level CSS.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open `DragResizeAndAnimation.sln`.
3. Restore the NuGet packages.
4. Set `DragResizeAndAnimation.Server` as the startup project if it is not already selected.
5. Build the solution.
6. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Open the repository folder.
2. Navigate to the server project directory.

```bash
cd Server
dotnet restore
dotnet run
```

3. Open the local application URL displayed in the terminal output.

## Project Structure

`Pages/Index.razor` - Main sample page that demonstrates draggable, resizable, and animated Syncfusion Dialog components, including newsletter subscription and success confirmation dialogs.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Syncfusion Dialog documentation: https://blazor.syncfusion.com/documentation/dialog/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.