---
layout: post
title: Custom XAML Analyzers
summary: Create your own XAML Analyzers.
featured-img: customanalysis
permalink: custom-analysis
---

Create your own analyzers to check that the controls in your XAML files are used the way you want and need them to be.

![Custom warnings displayed for a custom XAML control](./assets/img/posts/example-custom-errors.png)

If you say how an issue should be addressed, integration with Visual Studio handles display actions and making changes to the document.

![List of Quick Actions displayed in the Visual Studio XAML editor](./assets/img/posts/example-custom-quickaction.png)

There are [full details on creating custom analyzers](https://github.com/mrlacey/Rapid-XAML-Toolkit/blob/main/docs/custom-analysis.md) on GitHub.

This functionality is provided through a [NuGet package](https://www.nuget.org/packages/RapidXamlCustomAnalysis) that must be referenced separately to installing the toolkit.

---

To make use of your custom analyzers, you need the [XAML Analysis tool](./analysis) installed which you get as [part of the Toolkit](https://marketplace.visualstudio.com/items?itemName=MattLaceyLtd.RapidXamlToolkit). [Project and item templates](./templates) also exist to make authoring custom analyzers easy.
