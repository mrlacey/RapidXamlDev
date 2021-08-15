---
layout: post
title: XAML Generation
summary: Accelerate XAML app development by generating XAML from your ViewModel.
featured-img: generation
permalink: generation
---

Instantly generate XAML from your ViewModels (or any other class.) Select the class, property, or group of properties then right-click and select Rapid XAML > **Copy as XAML**.

![Copy as XAML context menu](./assets/img/posts/copy-as-xaml-menu.png)

You can then paste the generated XAML where you want it.

Or generate XAML for the entire class by **dragging the file** onto the XAML editor.

![Example of dragging and dropping a ViewModel onto the editor](./assets/img/posts/drag-drop-generation.gif)

Whether you're building a **WPF**, **UWP**, or **Xamarin.Forms**, it's pre-configured with a number of options but can also be configured to produce the XAML you would write yourself.

[Configurable options](https://github.com/mrlacey/Rapid-XAML-Toolkit/blob/main/docs/configuration.md) allow you to map classes, properties, and methods and the XAML to generate based on types, names, accessibility, and attributes.

![Mappings configuration screen](./assets/img/posts/edit-profile.png)

---

This functionality is [included when you **install the Toolkit**](https://marketplace.visualstudio.com/items?itemName=MattLaceyLtd.RapidXamlToolkit) but is also available [separately](https://marketplace.visualstudio.com/items?itemName=MattLaceyLtd.RapidXamlGeneration).

---

This extension includes some functionality that is dependent upon the [Common functionality](./common).
