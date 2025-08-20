# Macro-Friendly-Restaurant-App
App to help macro trackers and fitness enthusiasts find macro friendly restaurants with ease in their area or while travelling.  

---

## 🚀 Goal
- **Problem:** Eating out while tracking macros is hard.
- **Audience:** Fitness enthusiasts, athletes, and anyone tracking calories/macros.
- **Solution:** An app that lists restaurants with macro-friendly options and nutrition info.

## 🧱 Tech Stack
- **Platform:** React Native (Expo)
- **Language:** JavaScript/TypeScript
- **Backend (future):** Node.js/Express + MongoDB or Firebase

## 📱 Core Features (MVP)
- [ ] Search restaurants nearby
- [ ] Filter meals by macro targets
- [ ] Save favorite restaurants
- [ ] User accounts (basic auth)

### Future Ideas
- [ ] Integration with MyFitnessPal
- [ ] Travel mode (suggest restaurants in other cities)
- [ ] Reviews and community recommendations

## 🗺️ Roadmap (Beginner-Friendly)

### Phase 1: Foundation (Weeks 1–2)
- [x] Set up GitHub repo ✅
- [ ] Install tools: Node.js, VS Code, Expo CLI, Expo Go
- [ ] Scaffold project with `npx create-expo-app`
- [ ] Push starter code to GitHub
- [ ] Write README with goals + roadmap
- [ ] Document setup steps in `/docs/journal/week-01.md`

---

### Phase 2: First Feature & UI Basics (Weeks 3–4)
- [ ] Learn basics of React Native: components, props, state
- [ ] Add a **home screen** with app title/logo
- [ ] Create simple navigation (tab or stack navigation)
- [ ] Add a placeholder **search bar** (not functional yet)
- [ ] Push code weekly, update journal with what you learned

---

### Phase 3: Core MVP (Weeks 5–7)
- [ ] Connect to a **mock data file** (JSON with restaurant info)
- [ ] Display a list of restaurants with macros (dummy data)
- [ ] Add filter options (high-protein, low-calorie, etc.)
- [ ] Allow user to “favorite” a restaurant (save in local storage)
- [ ] Journal weekly progress (blockers + wins)

---

### Phase 4: Polishing (Weeks 8–9)
- [ ] Improve UI: colors, fonts, icons
- [ ] Add a splash screen & app icon
- [ ] Test on both iOS + Android (Expo makes this easy)
- [ ] Share screenshots in README

---

### Phase 5: Stretch Goals (Weeks 10–12+)
- [ ] Connect to a real API (e.g., Yelp API for restaurants)
- [ ] Add simple user login (Firebase Auth is beginner-friendly)
- [ ] Deploy a beta version via Expo so others can test
- [ ] Write a blog post (Hashnode/Dev.to) summarizing your MVP

---

## ⏱️ Realistic Timeline
- **Month 1:** Setup + Hello World  
- **Month 2:** First screens + navigation  
- **Month 3:** Core restaurant list & filtering  
- **Month 4:** Favorites, polish, screenshots  
- **Month 5+:** APIs, auth, publish beta  

---

## 📒 Developer Habits
- Commit to GitHub often (small commits > big dumps)  
- Update **Dev Journal** (`/docs/journal/`) once a week  
- Open **Issues** for each feature/bug  
- Use a **Project Board** (*Backlog → In Progress → Done*)  


## 🧪 Running the App
### React Native (Expo)
```bash
npm create expo-app@latest
cd Macro-Friendly-Restaurant-App
npm install
npx expo start
