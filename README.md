# MacroMap – Macro Tracking Restaurant App

**Version:** 1.0  
**Date:** August 20, 2025  
**Owner:** [Zara Zolkos / ZZ Fit]  

---

## 📖 Overview

**MacroMap** helps health-conscious users find restaurants and meals that fit their nutritional goals. It provides local restaurant discovery, full menu with macro breakdowns, filtering tools, and the ability to save favorites.

### Goals
- Allow users to easily discover **macro-friendly restaurants** in their local area.  
- Provide **detailed nutritional breakdowns** of menu items (calories, protein, carbs, fats, fiber).  
- Enable **filtering and personalization** based on users’ macro goals.  
- Provide a **seamless, engaging user experience** with quick search, filtering, and favorites.  

### Success Metrics
- % of users who successfully search and view at least 1 restaurant per session.  
- Average number of menu items viewed per user.  
- Favorites added per user.  
- 30-day retention rate.  

---

## 🎯 Target Audience
- **Demographic:** Fitness enthusiasts, athletes, dieters, and health-conscious individuals (18–40).  
- **Primary Need:** Quickly find dining options that align with calorie and macro goals.  
- **Pain Points Solved:** Lack of transparency in menus, time wasted searching for “healthy” meals, tracking meals when eating out.  

---

## 🚀 Features

### Core Features (MVP)
1. **Restaurant Discovery**  
   - Location-based search (map + list).  
   - Tags like *High-Protein*, *Low-Calorie*, *Low-Carb*.  

2. **Menu & Macros**  
   - Full menu with kcal, protein, carbs, fat, fiber.  
   - Pull from database or nutrition API.  
   - Fallback: AI-based estimation for missing data.  

3. **Favorites**  
   - Save favorite restaurants and menu items.  
   - Synced to user profile.  

4. **Filtering & Sorting**  
   - Filters: calories, protein min, fat max, carbs max.  
   - Presets: “Under 500 kcal,” “Over 30g protein,” “Low Carb.”  
   - Sort by distance, protein per calorie, rating.  

### Future Features (Phase 2+)
- User profile with macro goals.  
- Progress % per meal vs daily goals.  
- User reviews & photos.  
- Coach picks / featured meals.  
- Push notifications for nearby options.  

---

## 🗄️ Data & Integrations

### Database (Supabase Recommended)
- **restaurants**: id, name, cuisine, address, lat/lng, rating, tags, photo.  
- **menu_items**: id, restaurant_id, name, kcal, protein, carbs, fat, fiber, verified.  
- **favorites**: user_id, restaurant_id/menu_item_id.  
- **users_profile**: user_id, macro goals, dietary tags.  

### APIs
- **Google Places API** → restaurant discovery, photos.  
- **Nutritionix API** → nutrition data for menu items.  
- **Supabase** → authentication, storage, database.  

---

## 🔄 User Flow

**Example: Find a Macro-Friendly Meal**  
1. User opens app → location permission granted.  
2. Nearby restaurants shown (list + map).  
3. User taps restaurant → menu items + macros displayed.  
4. User applies filters (e.g., Protein >30g, Calories <500).  
5. User saves meal/restaurant to Favorites.  

---

## 🎨 Design

- **UI Style:** Clean, fitness-focused, modern.  
- **Navigation:** Bottom tab bar (Home, Search, Favorites, Profile).  
- **Components:**  
  - Restaurant cards (photo, rating, tags).  
  - Menu item rows (name, macros, add to favorites).  
  - Filter chips & progress bars.  
- **Images:**  
  - Restaurants → Google Places photos.  
  - Menu items → Nutritionix / placeholders.  

---

## ⚙️ Technical Stack

- **Frontend:** React Native (Expo).  
- **Backend:** Supabase (Postgres + Auth + Storage).  
- **Auth:** Email & password (social login later).  
- **Caching:** Offline last search.  
- **Deployment:** Expo EAS → iOS + Android.  

---

## ⚠️ Risks & Constraints

- API coverage gaps (not all restaurants/menus available).  
- Menus change frequently → background sync or user submissions needed.  
- Nutrition estimates may be approximate.  

---

## 🔮 Future Enhancements

- AI-powered meal recommendations.  
- Barcode scanner for packaged meals.  
- Subscription model (Pro tier with advanced filters).  
- Partnerships with restaurants for verified macro menus.  

---

## 📌 Status

This PRD defines **Version 1.0 (MVP)** scope. Future iterations will expand features based on user adoption and feedback.
