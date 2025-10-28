# 🖼️ Photo Viewer

A **menu-driven photo management application** built using **Object-Oriented Programming (OOP)** principles. The program enables users to efficiently manage their photo collections with features like viewing, deleting, restoring, and marking photos as favorites.

---

## 🧠 Overview

The **Photo Viewer** program provides a user-friendly interface for managing photos.
Users can:

* Display photos
* Add to favorites
* Delete photos
* Restore from recently deleted photos
* Permanently delete photos after 30 days

This project demonstrates the implementation of **OOP concepts** such as inheritance, composition, and encapsulation through a **Doubly Linked List** structure.

---

## 🧩 Program Structure

### **1. Base Class**

#### `DoubleLinkedList.cpp`

* Handles the creation, linking, and manipulation of nodes.
* Supports traversing, displaying, and searching within the list.

### **2. Derived Classes**

#### `Gallery.cpp`

* Inherits from `DoubleLinkedList`.
* Manages the main photo gallery, including editing, deleting, and favoriting photos.

#### `RecentDelete.cpp`

* Inherits from `DoubleLinkedList`.
* Manages recently deleted photos, allowing users to restore or permanently delete them.

#### `Favourite.cpp`

* Inherits from `DoubleLinkedList`.
* Handles the favorite photos list and allows for deletion from both favorite and main galleries.

### **3. Composition**

* `Gallery` contains instances of `RecentDelete` and `Favourite` to manage deleted and favorite photos cohesively.
* `Favourite` also contains a `RecentDelete` instance to manage photos deleted from favorites.

---

## 🌟 Features

* **Add Photo** – Insert new photos into the gallery.
* **Display Photos** – View all photos in the gallery.
* **Delete Photo** – Move photos to the recently deleted section.
* **Restore Photo** – Recover photos from the recently deleted list.
* **Favorite Management** – Add or remove photos from favorites.
* **Automatic Cleanup** – Photos in the recently deleted list are purged after 30 days.

---

## ⚙️ How It Works

The system uses a **Doubly Linked List** as the core data structure, allowing efficient insertion and deletion of photos from any position.
Through OOP:

* **Inheritance** ensures reusability and extension of common methods.
* **Composition** allows managing linked components (gallery, favorites, deleted photos).
* **Encapsulation** ensures that data manipulation is done safely via class methods.

---

## 💻 Technologies Used

* **Language:** Python
* **Paradigm:** Object-Oriented Programming (OOP)
* **Data Structure:** Doubly Linked List

*(Originally conceptualized in C++ but implemented here in Python for clarity and testing ease.)*

---

## 🚀 Getting Started

### **1. Clone this repository**

```bash
git clone https://github.com/yourusername/photo-viewer.git
cd photo-viewer
```

### **2. Run the program**

```bash
python Photo\ Viewer.py
```

### **3. Follow the on-screen menu**

You’ll be prompted to:

* Add new photos
* View gallery
* Manage favorites
* Restore or permanently delete photos

---

## 🧪 Example Usage

```
Photo Viewer Menu:
1. Add Photo
2. View Gallery
3. View Favorites
4. View Recently Deleted
5. Exit

Enter your choice: 2
→ Displaying all photos in gallery...
```

---



---

