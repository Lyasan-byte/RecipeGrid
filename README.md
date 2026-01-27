# 🥘 RecipeGrid  
*A clean, modern recipe manager built with SwiftUI*

![SwiftUI](https://img.shields.io/badge/SwiftUI-FFAC45?style=flat&logo=swift&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=flat&logo=apple&logoColor=white)
![Swift 5.9+](https://img.shields.io/badge/Swift-5.9%2B-orange?style=flat)

**RecipeGrid** is a personal iOS app designed to help users collect, organize, and manage their favorite recipes. Built entirely in **SwiftUI**, it combines a sleek, dark-themed interface with practical functionality — from image selection to local data persistence.

> This project was created as a learning exercise to deepen my understanding of modern SwiftUI patterns, data flow, and user experience design.

---

## ✨ Features

- **Add & Edit Recipes**: Create new recipes or update existing ones with title, summary, category, and custom image.
- **Image Support**: Select photos from your library using `PhotosPicker` (iOS 16+) and save them locally.
- **Local Persistence**:
  - Recipe metadata (title, category, etc.) stored in **UserDefaults** via `Codable`.
  - Recipe images saved to the app’s **caches directory** using `FileManager`.
- **Smart Filtering & Sorting**:
  - Filter by food category (Main, Appetizer, Salad, Dessert).
  - Search by title or category.
  - Sort alphabetically by name.
- **Responsive UI**:
  - Adaptive grid layout (`LazyVGrid`).
  - Liquid Glass buttons and cards.
  - Smooth navigation and sheet-based forms.

---

## 🛠️ Tech Stack

| Layer | Technology |
|------|------------|
| **UI Framework** | SwiftUI (iOS 16+) |
| **State Management** | `@Observable` (Swift 5.9), `@Bindable` |
| **Data Storage** | `UserDefaults` (for structured data), `FileManager` (for images) |
| **Image Handling** | `PhotosPicker`, `UIImage`, PNG encoding |
| **Architecture** | MVVM-inspired (View ↔ ViewModel ↔ Local Storage) |
| **Utilities** | Custom file manager, reusable components (`CategoryPicker`, `InputTitle`, etc.) |

---

## 📱 Screenshots

<div align="center">
  <img src="assets/mainScreen.png" width="250" alt="Recipes List" />
  <img src="detailScreen.png" width="250" alt="Recipe detail screen" />
  <br>
  <em>From left to right: Recipe grid, detail view</em>
</div>

---

## 🚀 How to Run

1. Clone the repository  
   ```bash
   git clone https://github.com/Lyasan-byte/RecipeGrid.git
