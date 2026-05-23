# Room MVVM Demo 📝

Une application Android de démonstration illustrant l'implémentation de la bibliothèque de persistance **Room** couplée à l'architecture **MVVM (Model-View-ViewModel)**.

## 🚀 Présentation du Projet
Ce projet a pour objectif de présenter les meilleures pratiques de développement Android moderne. Il met en œuvre une gestion fluide et réactive d'une base de données locale SQLite, tout en garantissant une séparation claire des responsabilités pour une maintenance et une testabilité optimales.

## ✨ Fonctionnalités Clés
- **Persistance des Données** : Utilisation de Room pour un stockage local robuste.
- **Gestion des Notes** : Ajout, consultation et suppression de notes de manière intuitive.
- **Interface Réactive** : Mise à jour instantanée de l'UI grâce à `LiveData`.
- **Architecture Moderne** : Utilisation du `ViewModel` pour gérer les données en respectant le cycle de vie Android.
- **Expérience Utilisateur** : Affichage optimisé avec `RecyclerView` et design moderne via `CardView` et `Material Components`.

## 🏗️ Architecture Technique
L'application suit scrupuleusement les recommandations architecturales de Google (Jetpack) :
- **Entity (`Note`)** : Représente la structure des données (table SQLite).
- **DAO (`NoteDao`)** : Interface définissant les opérations d'accès aux données (CRUD).
- **Room Database (`NoteDatabase`)** : Point d'accès principal à la base de données.
- **Repository (`NoteRepository`)** : Abstraction des sources de données pour le reste de l'application.
- **ViewModel (`NoteViewModel`)** : Gère la logique métier et prépare les données pour la vue.
- **UI (`MainActivity`, `NoteAdapter`)** : Gère l'affichage et les interactions utilisateur.

## 🛠️ Stack Technique
- **Langage** : Java
- **Base de données** : [Room Persistence Library](https://developer.android.com/training/data-storage/room)
- **Composants d'Architecture** : LiveData, ViewModel, Lifecycle
- **Composants UI** : RecyclerView, CardView, Material Design
- **Gestionnaire de dépendances** : Gradle

## 📂 Structure du Code
- `data/local/` : Entités, DAOs et configuration de la base de données.
- `data/` : Le Repository centralisant la logique de données.
- `viewmodel/` : Logique de présentation et gestion d'état.
- `ui/` : Activités et adaptateurs pour l'interface utilisateur.

## ⚙️ Installation
1. Cloner le dépôt :
   ```bash
   git clone https://github.com/Sultan-zd/Lab19-RoomMVVMDemo.git
   ```
2. Ouvrir le projet dans **Android Studio**.
3. Synchroniser les fichiers **Gradle**.
4. Lancer l'application sur un terminal ou un émulateur.

---
*Projet développé à des fins pédagogiques pour illustrer la puissance des composants d'architecture Android.*
