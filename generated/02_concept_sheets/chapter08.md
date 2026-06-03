# Chapter 8: Implementation Support — Concept Sheet

---

## Windowing Systems & Toolkits

| Term | Definition |
|------|------------|
| **Windowing system** | Software that manages windows, input devices, and screen display on a graphical user interface. |
| **X Window System** | A network-transparent windowing system for bitmap displays, widely used on Unix/Linux. |
| **Wayland** | A modern display server protocol replacing X11 on Linux, emphasizing simplicity and security. |
| **macOS Window Server** | Apple's proprietary windowing system managing graphical display on macOS. |
| **Desktop Window Manager (DWM)** | Microsoft's compositing window manager for Windows, handling visual effects and window rendering. |
| **Toolkit** | A library of reusable UI components (buttons, menus, text fields) for building graphical interfaces. |
| **Widget** | A UI component within a toolkit, providing specific functionality (e.g., button, slider, list). |
| **Motif** | An older X11-based toolkit defining the look-and-feel of many Unix GUIs. |
| **Qt** | A cross-platform C++ toolkit for creating GUI and non-GUI applications. |
| **GTK** | A cross-platform toolkit originally for the GIMP, now widely used in GNOME-based Linux desktops. |
| **Swing/JavaFX** | Java-based toolkits for building cross-platform desktop GUIs. |
| **WPF (Windows Presentation Foundation)** | Microsoft's UI framework for building Windows desktop applications using XAML and .NET. |

---

## UI Architecture Models

| Term | Definition |
|------|------------|
| **UIMS (User Interface Management System)** | A system that separates the user interface from the application logic, enabling independent development and modification. |
| **MVC (Model-View-Controller)** | An architectural pattern separating an application into Model (data), View (display), and Controller (input handling). |
| **Model** | The component in MVC representing the application's data and business logic. |
| **View** | The component in MVC responsible for rendering the user interface. |
| **Controller** | The component in MVC that handles user input and updates the model. |
| **PAC (Presentation-Abstraction-Control)** | An agent-based architecture where each UI component is an agent with Presentation (display), Abstraction (data/logic), and Control (coordination) components. |
| **Seeheim model** | A UIMS reference architecture with three layers: Presentation (display), Dialog Control (interaction logic), and Application Interface (application logic). |
| **Presentation layer** | The outermost layer handling direct display and input device interaction. |
| **Dialog control** | The middle layer managing the sequence and structure of user-system interaction. |
| **Application interface** | The innermost layer bridging the UI and the application's core functionality. |
| **Agent-based architecture** | An architecture where autonomous software agents represent UI components and coordinate through messages. |

---

## Modern Implementation Approaches

| Term | Definition |
|------|------------|
| **Web framework** | A software framework designed for building web applications (e.g., React, Angular, Vue.js). |
| **Component-based architecture** | An approach where UIs are built from self-contained, reusable components with defined interfaces. |
| **Reactive programming** | A programming paradigm where the UI automatically updates in response to changes in underlying data. |
| **Declarative UI** | Defining what the UI should look like given a certain state, rather than how to construct it step by step. |
| **Data binding** | Automatically synchronizing data between UI elements and data sources. |
| **Two-way data binding** | Data binding where changes in the UI update the data and changes in the data update the UI. |
| **Single Page Application (SPA)** | A web application that loads a single HTML page and dynamically updates content without full page reloads. |
| **Progressive Web App (PWA)** | A web app that uses modern APIs to deliver app-like features (offline support, push notifications). |
| **Cross-platform development** | Building applications that run on multiple platforms (Windows, macOS, Linux, mobile) from a single codebase. |
| **Responsive design** | Designing web interfaces that adapt to different screen sizes and orientations. |
