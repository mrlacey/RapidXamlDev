---
layout: post
title: Roslyn Analyzers
summary: Roslyn analyzers to help with XAML app development.
featured-img: roslyn
permalink: roslyn-analyzers
---

This extension includes "Roslyn analyzers" to help write apps that use XAML.

The following helpers are provided. They are not intended to find and fix problems with the code, instead make it easier to change existing code if that is needed.

## Convert auto-properties to ones that call `OnPropertyChanged` or similar

If the auto-property is in a class that implements `INotifyPropertyChanged` or inherits from a class that does, an option to convert the property will be provided. The setter of the expanded property will call `OnPropertyChanged`. Additionally, if the (base) class has helper methods for `Set` or `SetProperty` options that call these methods are presented too.

![Visual Studio editor showing suggested actions for changing the property definition](#)

## Convert auto-property to `DependencyProperty` or `BindableProperty`

If you have an existing property but need to turn it into a `DependencyProperty` or `BindableProperty`, it can be hard to remember how and be more work (keystrokes) than you should expend on such a task. You could delete it and use a snippet to generate a new one with the same name, but that can feel counter-intuitive.
This "fix" is offered for any auto-property in a class that inherits from `DependencyObject` or `BindableObject`.

![Visual Studio editor showing suggested actions for changing to a dependency property](./assets/img/posts/to-dependency-property.png)

**Note.** These analyzers are currently only available for C#.

---

This functionality is [included when you **install the Toolkit**](https://marketplace.visualstudio.com/items?itemName=MattLaceyLtd.RapidXamlToolkit) but is also available [separately](https://marketplace.visualstudio.com/items?itemName=MattLaceyLtd.RapidXamlRoslynAnalyzers).
