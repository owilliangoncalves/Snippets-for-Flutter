# Snippets for Flutter

[![Downloads](https://img.shields.io/visual-studio-marketplace/d/WillianGoncalves.snippets-for-flutter?color=blue&label=Downloads)](https://marketplace.visualstudio.com/items?itemName=WillianGoncalves.snippets-for-flutter)
[![Version](https://img.shields.io/visual-studio-marketplace/v/WillianGoncalves.snippets-for-flutter?color=brightgreen&label=Extension%20Version)](https://marketplace.visualstudio.com/items?itemName=WillianGoncalves.snippets-for-flutter)
![Flutter Version](https://img.shields.io/badge/Flutter-%E2%89%A53.24-blue)
![Dart Version](https://img.shields.io/badge/Dart-%E2%89%A53.5-blue)

**Snippets for Flutter** provides a collection of clean and reusable code templates designed to help you build Flutter apps faster and more efficiently.  
This extension includes ready-to-use snippets for both **Stateless** and **Stateful Widgets**, with and without `AdaptativeScaffold`, making your development process smoother and more productive.

---

## ✨ Features

- 🚀 Quickly generate Flutter widget boilerplates with a few keystrokes.  
- 🧱 Support for:
  - `StatelessWidget` (with or without `AdaptativeScaffold`)
  - `StatefulWidget` (with private or public state)
  - Scaffold or AdaptativeScaffold base
- 🪄 Automatic **PascalCase** class naming based on the file name (e.g. `home_page.dart` → `HomePage`).
- ✨ Clean indentation and code formatting.
- 🧭 Consistent structure that aligns with Flutter best practices.

---

## 💻 Snippet Examples

Typing `fstless` in a Dart file will generate:

```dart
class HomePage extends StatelessWidget {
	const HomePage({super.key});

	@override
	Widget build(BuildContext context){
		return Scaffold(
			body: Center(child: Text('Hello World')),
		);
	}
}
```

Typing `fpastful` in a Dart file will generate:

```dart
class HomePage extends StatefulWidget {
	const HomePage({ super.key });

	@override
	State<HomePage> createState() => _HomePageState();
}

class _HomePageState extends State<HomePage> {
	@override
	Widget build(BuildContext context) {
		return AdaptativeScaffold(
			body: Center(child: Text('Hello World')),
		);
	}
}
```
---
## 🧩 Requirements

✅ Flutter SDK installed and configured
✅ Dart extension installed in VS Code
✅ A valid Flutter project

| Prefix     | Description                                                |
| ---------- | ---------------------------------------------------------- |
| `fstless`  | Stateless widget without AdaptativeScaffold                |
| `fastless` | Stateless widget with AdaptativeScaffold                   |
| `fstful`   | Stateful widget (public state) without AdaptativeScaffold  |
| `fastful`  | Stateful widget (public state) with AdaptativeScaffold     |
| `fpstful`  | Stateful widget (private state) without AdaptativeScaffold |
| `fpastful` | Stateful widget (private state) with AdaptativeScaffold    |
