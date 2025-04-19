# Travel Activity Recommender – Daily Development Tracker

## Day 1 – Geolocation and Places Fetching

### Objective  
Set up the foundational frontend environment, enable user location input (via browser or manual entry), and fetch a list of nearby places using a third-party Places API.

---

## 1. Environment Setup

- [x] Set up a new React project using Vite or CRA
- [x] Initialize Git repository and make the first commit
- [x] Install dependencies
- [x] Create the following folder structure:
  ```
  /src
    /components
    /api
    /hooks
    App.jsx
    main.jsx
  ```

---

## 2. Create Location Input Feature

- [ ] Create a `LocationInput.jsx` component
- [ ] Implement browser geolocation via `navigator.geolocation.getCurrentPosition()`
- [ ] Handle errors and show loading states
- [ ] Add fallback manual text input for city/address
- [ ] Use Geocoding API to convert text to coordinates
- [ ] Store all coordinates (manual or geolocation) in component or global state

---

## 3. Set Up Places API Integration

- [ ] Register and obtain API key for:
  - Google Places API: https://developers.google.com/maps/documentation/places/web-service/overview  
  _or_
  - Foursquare Places API: https://developer.foursquare.com/docs/places-api/
- [ ] Create `.env` file to store API key securely
- [ ] Build `api/fetchPlaces.js`:
  - Accept lat/lng as input
  - Return list of nearby places (e.g. name, address, rating)
  - Handle loading and error states
- [ ] Add fallback mock data in case of rate limit/API failure

---

## 4. Display Raw Place Results

- [ ] Create `PlaceList.jsx` component
- [ ] Render a simple list of fetched places (just names for now)
- [ ] Wire up `LocationInput` to trigger the place fetch function
- [ ] Add a loading indicator while fetching places

---

## 5. Testing & Wrap-Up

- [ ] Verify that both geolocation and manual input flow work
- [ ] Ensure places API is returning usable results
- [ ] Confirm results display correctly in the frontend
- [ ] Make a second Git commit with all Day 1 work
- [ ] Write a brief daily log:
  - What was completed
  - What needs follow-up
  - Any blockers or notes

---

## Notes  
> Use this section to record bugs, side ideas, or improvements for later.
