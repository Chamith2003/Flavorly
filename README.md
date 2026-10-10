# 🍽️ Flavorly

A modern recipe discovery app built with React. Search for recipes, browse results, and view detailed information including ingredients, instructions, nutritional labels, and more — all powered by the [Spoonacular API](https://spoonacular.com/food-api).

---

## ✨ Features

- **Recipe Search** — Instantly search thousands of recipes by keyword
- **Recipe Details** — View full recipe information including:
  - 🖼️ Recipe image
  - ⏱️ Preparation time
  - 👨‍👩‍👧‍👦 Serving size
  - 🥕 Vegetarian / 🐮 Vegan indicators
  - 💲 Price per serving
- **Ingredients List** — See all required ingredients with images and amounts
- **Step-by-Step Instructions** — Follow clear, ordered cooking instructions
- **Responsive Layout** — Clean split-panel design with search results and recipe details side by side

---

## 🛠️ Tech Stack

| Technology | Purpose |
| --- | --- |
| [React 19](https://react.dev/) | UI library |
| [Vite 8](https://vite.dev/) | Build tool & dev server |
| [CSS Modules](https://github.com/css-modules/css-modules) | Scoped, component-level styling |
| [Spoonacular API](https://spoonacular.com/food-api) | Recipe data source |

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- A free [Spoonacular API key](https://spoonacular.com/food-api/console#Dashboard)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/Chamith2003/Flavorly.git
   cd flavorly
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure environment variables**

   Create a `.env` file in the project root:

   ```env
   VITE_API_KEY=your_spoonacular_api_key_here
   ```

4. **Start the development server**

   ```bash
   npm run dev
   ```

   The app will be available at `http://localhost:5173`.

---

## 📁 Project Structure

```
flavorly/
├── index.html                  # HTML entry point
├── .env                        # Environment variables (API key)
├── package.json
├── vite.config.js
└── src/
    ├── main.jsx                # React entry point
    ├── App.jsx                 # Root component
    ├── App.css                 # Global styles
    └── components/
        ├── Nav.jsx             # Navigation bar
        ├── Search.jsx          # Search input with API fetching
        ├── Container.jsx       # Main layout wrapper
        ├── InnerContainer.jsx  # Inner panel wrapper
        ├── FoodList.jsx        # Renders list of search results
        ├── FoodItem.jsx        # Individual recipe card
        ├── FoodDetails.jsx     # Full recipe detail view
        ├── ItemList.jsx        # Ingredients list
        ├── Item.jsx            # Individual ingredient
        └── *.module.css        # Component-scoped CSS modules
```

---

## 📜 Available Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Vite development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run ESLint for code quality checks |

---

## 🔑 API Reference

This app uses the [Spoonacular Food API](https://spoonacular.com/food-api). The following endpoints are used:

| Endpoint | Purpose |
| --- | --- |
| `GET /recipes/complexSearch?query={query}` | Search recipes by keyword |
| `GET /recipes/{id}/information` | Get full recipe details |

> **Note:** The free tier allows **50 requests per day**. See the [Spoonacular pricing page](https://spoonacular.com/food-api/pricing) for more details.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
