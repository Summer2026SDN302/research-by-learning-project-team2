# Smart Household Food Management System

> A Research by Learning (RBL) project for building a mobile system that helps households manage food inventory, track expiration dates, receive storage suggestions, generate meal plans, estimate calories, and create shopping lists.

---

## 1. Project Information

| Item | Description |
|---|---|
| Course | SDN302 |
| Class | SE19B05 |
| Semester | SU26 |
| Group | 2 |
| Topic | Smart Household Food Management System |
| Repository | https://github.com/Summer2026SDN302/research-by-learning-project-team2 |
| Repository FE| https://github.com/huynguyen1807/Front-end |
| Repository BE| https://github.com/huynguyen1807/Back-end |
| Jira | https://thangkhaiyt24.atlassian.net/jira/software/projects/SCRUM/boards/1 |

---

## 2. Team Members

| No. | Student ID | Full Name | GitHub Username | Role |
|---:|---|---|---|---|
| 1 | DE180054 | Trần Đức Thắng | thangdepzai12-dev | Leader | 
| 2 | DE180154 | Võ Phạm Mỹ | vophammy24 | Member | 
| 3 | DE180005 | Lê Đình Nhật Nam | LeDinhNhatNam | Member | 
| 4 | DE190487 | Nguyễn Đức Huy | huynguyen1807 | Member | 
| 5 | DE180396 | Nguyễn Minh Thông | minhthong-git | Member |

---

## 3. Project Overview

The Smart Household Food Management System is a mobile application designed to help families manage food at home more effectively. Many households buy food from both supermarkets and traditional markets, but they often forget expiration dates, store food in the wrong place, or do not know what meals to cook with the available ingredients.

This system aims to reduce food waste and support better meal planning by providing these core functions:

- Add and organize household food items.
- Classify food by source: supermarket or traditional market.
- Scan supermarket food to recognize barcode or expiration information.
- Estimate expiry dates for market food using AI support.
- Allow users to manually input or edit expiration dates.
- Track food expiration status and send alerts.
- Suggest suitable storage methods.
- Recommend daily meals based on available food.
- Estimate calories for meals.
- Extract recipe information from online videos.
- Create shopping lists based on missing ingredients.

---

## 4. Research by Learning (RBL) Focus

This project applies the Research by Learning approach. The team does not only build an application, but also studies academic papers and practical technologies to support design decisions.

### 4.1 Main RBL Focus

The research focus of this project includes four main areas:

| RBL Area | Focus in This Project |
|---|---|
| Problem Research | Study household food waste, food storage behavior, food source impact, and user decision-making. |
| Algorithm / Logic | Study expiry prediction, meal recommendation, calorie estimation, ingredient substitution, and missing ingredient suggestion. |
| System Architecture | Design a modular React Native mobile system with clear separation between screens, components, services, hooks, types, and utilities. |
| Technology Research | Explore barcode/OCR scanning, AI recommendation, notification service, recipe extraction, and structured food data management. |

### 4.2 Main Research Questions

The project is guided by these research questions:

1. How can a mobile application help households reduce food waste?
2. How should food from supermarkets and traditional markets be handled differently?
3. How can AI support expiry prediction, storage suggestion, meal planning, and calorie estimation?
4. How can recipe recommendation use available food inventory instead of only user preference?
5. How should notification messages be designed so that users take useful actions?

### 4.3 RBL Output

The expected RBL outputs include:

- Paper review and evaluation.
- Use case diagram and use case descriptions.
- ERD and database design.
- Screen flow and UI design.
- React Native folder structure and base components.
- System architecture proposal.
- Prototype implementation.
- Testing and evaluation notes.

---

## 5. Literature Review Summary

The project research is based on papers related to household food waste, food recommendation, nutrition recommendation, barcode scanning, and smart home feedback design.

Key insights from the research:

- Household food waste often happens because users forget food items, store food incorrectly, buy more than needed, or do not use leftovers effectively.
- Food inventory should be the center of the system. Meal plans, alerts, storage suggestions, and shopping lists should depend on the inventory.
- AI can support meal planning, calorie estimation, recipe adaptation, and ingredient substitution, but AI results should be treated as estimated and should be supported by structured data.
- Food source is important. Supermarket food can use barcode/OCR scanning, while traditional market food may need AI expiry prediction or manual input.
- Notifications should be action-based, such as “Use spinach today” or “Suggested recipe: vegetable soup,” instead of only showing generic warnings.

---

## 6. Main Features

| Feature ID | Feature Name | Description |
|---|---|---|
| FE-01 | Food Inventory | Add, update, delete, and view household food items. |
| FE-02 | Food Source Classification | Classify food as supermarket food or market food. |
| FE-03 | Expiry Recognition and Prediction | Scan supermarket food or estimate market food expiry using AI support. |
| FE-04 | Expiration Tracking | Track food status such as safe, near expiry, expired, or need check. |
| FE-05 | Notification Alert | Send alerts when food is near expiry or expired. |
| FE-06 | Storage Suggestion | Suggest suitable storage methods based on food type and location. |
| FE-07 | Meal Recommendation | Generate daily meal plans based on available food and user preferences. |
| FE-08 | Calorie Estimation | Estimate calories for meals or meal plans. |
| FE-09 | Video Recipe Extraction | Extract recipe information from online video links. |
| FE-10 | Shopping List | Create a shopping list based on missing ingredients or user needs. |

---

## 7. Actors

| Actor | Description |
|---|---|
| User | Main user who manages food inventory, receives alerts, views suggestions, generates meal plans, and creates shopping lists. |
| Administrator | Maintains system data such as food categories, storage rules, nutrition data, recipes, and AI-generated data review. |
| Scanning Service | External service that supports barcode and expiration date recognition for supermarket food. |
| AI Recommendation Service | External AI service that supports expiry prediction, storage suggestion, meal planning, calorie estimation, and recipe extraction. |
| Notification Service | External service that sends expiration alerts and storage warnings to users. |
| External Video Platform | External platform such as YouTube, TikTok, or Facebook that provides video content or recipe information. |

---

## 8. Main Use Cases

Use case names are written in the form of verb + object.

| Use Case ID | Use Case Name | Primary Actor | Description |
|---|---|---|---|
| UC-01 | Register Account | User | User creates an account to use the application. |
| UC-02 | Log In Account | User | User logs in to access personal food data. |
| UC-03 | View Food Inventory | User | User views all food items currently stored at home. |
| UC-04 | Add Food Item | User | User adds a new food item with source, quantity, expiry date, and storage location. |
| UC-05 | Scan Supermarket Food | User, Scanning Service | User scans barcode or expiration date from supermarket food. |
| UC-06 | Predict Market Food Expiry | User, AI Recommendation Service | AI estimates expiry date for food bought from traditional markets. |
| UC-07 | Input Expiry Date Manually | User | User manually enters or edits the expiry date. |
| UC-08 | View Expiration Status | User | User checks if food is safe, near expiry, expired, or needs checking. |
| UC-09 | Receive Expiration Alert | User, Notification Service | User receives alerts about near-expiry or expired food. |
| UC-10 | View Storage Suggestion | User, AI Recommendation Service | User views recommended storage methods. |
| UC-11 | Generate Daily Meal Plan | User, AI Recommendation Service | System suggests meals based on inventory, preference, and calorie goals. |
| UC-12 | Calculate Meal Calories | User, AI Recommendation Service | System estimates meal calories. |
| UC-13 | Extract Recipe from Video | User, AI Recommendation Service, External Video Platform | System extracts recipe information from a video link. |
| UC-14 | Create Shopping List | User | User creates a shopping list based on missing ingredients or personal needs. |
| UC-15 | Configure Storage Rule | Administrator | Admin configures storage rules for food categories. |
| UC-16 | Update Nutrition Data | Administrator | Admin updates calorie and nutrition data. |
| UC-17 | Review AI-generated Data | Administrator | Admin reviews AI-generated rules or suggestions before official use. |

---

## 9. Proposed Technology Stack

| Layer | Technology |
|---|---|
| Mobile App | React Native, Expo, TypeScript |
| Navigation | Expo Router / React Navigation |
| State Management | React Context, Redux Toolkit, or Zustand |
| UI Styling | React Native StyleSheet, shared theme constants |
| Backend API | Node.js with Express.js or NestJS |
| Database | MongoDB or PostgreSQL |
| Authentication | JWT-based authentication |
| Scanning | Barcode scanner, OCR support |
| AI Service | AI recommendation API / custom recommendation service |
| Notification | Firebase Cloud Messaging or local notification service |
| Version Control | Git and GitHub |

---

## 10. React Native Folder Structure

```text
src/
│
├── app/
│   ├── navigation/
│   │   ├── AppNavigator.tsx
│   │   ├── AuthNavigator.tsx
│   │   ├── MainNavigator.tsx
│   │   └── navigationTypes.ts
│   │
│   ├── providers/
│   │   ├── AppProvider.tsx
│   │   ├── AuthProvider.tsx
│   │   └── ThemeProvider.tsx
│   │
│   └── store/
│       ├── index.ts
│       ├── rootReducer.ts
│       └── hooks.ts
│
├── assets/
│   ├── images/
│   ├── icons/
│   ├── fonts/
│   └── animations/
│
├── components/
│   ├── common/
│   │   ├── Button.tsx
│   │   ├── Input.tsx
│   │   ├── Loading.tsx
│   │   ├── EmptyState.tsx
│   │   └── ModalConfirm.tsx
│   │
│   ├── layout/
│   │   ├── ScreenContainer.tsx
│   │   ├── Header.tsx
│   │   └── Card.tsx
│   │
│   └── form/
│       ├── FormInput.tsx
│       ├── FormSelect.tsx
│       └── FormError.tsx
│
├── features/
│   ├── auth/
│   │   ├── screens/
│   │   │   ├── LoginScreen.tsx
│   │   │   └── RegisterScreen.tsx
│   │   ├── components/
│   │   │   └── LoginForm.tsx
│   │   ├── services/
│   │   │   └── authApi.ts
│   │   ├── store/
│   │   │   └── authSlice.ts
│   │   ├── hooks/
│   │   │   └── useAuth.ts
│   │   └── types.ts
│   │
│   ├── home/
│   ├── food/
│   ├── meal/
│   ├── shopping/
│   ├── notification/
│   ├── profile/
│   └── admin/
│
├── services/
│   ├── apiClient.ts
│   ├── endpoints.ts
│   ├── storageService.ts
│   └── notificationService.ts
│
├── hooks/
│   ├── useDebounce.ts
│   ├── useKeyboard.ts
│   └── useNetworkStatus.ts
│
├── utils/
│   ├── constants.ts
│   ├── helpers.ts
│   ├── validators.ts
│   ├── formatDate.ts
│   └── permissions.ts
│
├── theme/
│   ├── colors.ts
│   ├── spacing.ts
│   ├── typography.ts
│   └── index.ts
│
├── types/
│   ├── api.ts
│   ├── user.ts
│   ├── food.ts
│   ├── meal.ts
│   ├── shopping.ts
│   └── common.ts
│
└── config/
    ├── env.ts
    └── appConfig.ts
```

---

## 11. Screen Flow

```text
Login Screen
    ↓
Landing Page / Home Dashboard
    ├── Food Inventory Screen
    │       ├── Add Food Screen
    │       ├── Scan Supermarket Food Screen
    │       └── Food Detail Screen
    ├── Expiration Alert Screen
    ├── Meal Recommendation Screen
    │       └── Meal Detail / Calorie Detail Screen
    ├── Video Recipe Extraction Screen
    │       └── Extracted Recipe Detail Screen
    ├── Shopping List Screen
    └── Profile / Settings Screen
```

---

## 12. Base UI Components

| Component | Purpose |
|---|---|
| Button | Reusable button for main actions. |
| Input | Reusable text input for forms. |
| Header | Top navigation header. |
| BottomNavbar | Bottom navigation between main screens. |
| Card | Reusable container for food, meal, alert, and shopping items. |
| FoodCard | Shows food name, quantity, storage location, expiry date, and status. |
| MealCard | Shows meal name, calories, cooking time, and ingredients. |
| AlertCard | Shows expiration or storage warning. |
| ShoppingItemRow | Shows one item in the shopping list with purchase status. |
| EmptyState | Shows message when no data is available. |
| Loading | Shows loading status while fetching data. |

---

## 13. Data Model Overview

Main entities:

- User
- FoodItem
- FoodCategory
- StorageLocation
- StorageSuggestion
- Notification
- Recipe
- RecipeIngredient
- MealPlan
- MealPlanDetail
- ShoppingList
- ShoppingListItem
- VideoRecipeSource

Important relationships:

- One User has many FoodItems.
- One User has many ShoppingLists.
- One User has many MealPlans.
- One FoodItem belongs to one FoodCategory.
- One FoodItem has one StorageLocation.
- One FoodItem can trigger many Notifications.
- One Recipe has many RecipeIngredients.
- One MealPlan includes many Recipes through MealPlanDetail.
- One ShoppingList contains many ShoppingListItems.

---

## 14. Installation Guide

### 14.1 Prerequisites

Install the following tools:

- Node.js LTS
- npm or yarn
- Expo CLI
- Git
- Android Studio or Expo Go app

### 14.2 Clone Repository

```bash
git clone <repository-url>
cd research-by-learning-project-team2
```

### 14.3 Install Dependencies

```bash
npm install
```

or

```bash
yarn install
```

### 14.4 Run the Application

```bash
npx expo start
```

To clear cache:

```bash
npx expo start --clear
```

To run with tunnel:

```bash
npx expo start --tunnel
```

---

## 15. Git Workflow

### 15.1 Branch Naming

```text
main                         Stable version for submission

develop                      Integrated development branch

feature/<member-name>         Individual feature branches

fix/<bug-name>                Bug fixing branches
```

Examples:

```bash
git checkout -b feature/vophammy
```

```bash
git checkout -b feature/minhthong
```

### 15.2 Basic Workflow

```bash
git checkout develop
git pull origin develop
git checkout -b feature/<your-name>
```

After coding:

```bash
git add .
git commit -m "feat: add food inventory screen"
git push origin feature/<your-name>
```

Then create a Pull Request from your feature branch to `develop`.

### 15.3 Commit Message Convention

| Type | Meaning |
|---|---|
| feat | Add new feature |
| fix | Fix bug |
| docs | Update documentation |
| style | Update UI/style only |
| refactor | Improve code structure without changing behavior |
| test | Add or update tests |
| chore | Update config or dependencies |

Examples:

```bash
git commit -m "feat: add login screen"
git commit -m "fix: correct food expiry status logic"
git commit -m "docs: update README research section"
```

---

## 16. Testing Plan

| Test Area | Example Test Case |
|---|---|
| Authentication | User can log in with valid information. |
| Food Inventory | User can add, update, delete, and view food items. |
| Expiry Tracking | System correctly marks food as safe, near expiry, or expired. |
| Scanning | System can receive barcode or OCR result from Scanning Service. |
| AI Prediction | System can display estimated expiry date for market food. |
| Meal Plan | System can suggest meals from available food. |
| Shopping List | User can add and mark items as purchased. |
| Notification | System can send alert for near-expiry food. |

---

## 17. Expected Outcome

The expected outcome is a working mobile application prototype that demonstrates:

- Food inventory management.
- Expiration tracking and alerting.
- Storage suggestion.
- Meal recommendation.
- Calorie estimation.
- Video recipe extraction concept.
- Shopping list creation.
- Clear modular React Native project structure.
- RBL-based explanation of why the system is needed and how research supports the design.

---

## 18. Project Status

Current status: Planning and prototype development.

Completed items:

- Project topic definition.
- Literature review direction.
- Actor and use case identification.
- Initial UI screen flow.
- React Native folder structure proposal.
- README structure.

Next steps:

- Finalize use case diagram.
- Finalize ERD and database design.
- Build UI screens.
- Implement food inventory flow.
- Implement notification and meal recommendation prototype.
- Write final report and demo script.

---

## 19. License

This project is developed for academic purposes in the SDN302 course.
