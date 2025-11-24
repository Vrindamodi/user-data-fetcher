# User Data Fetcher - Task 7 Documentation

##  Project Overview

A responsive web application that fetches and displays user data from the JSONPlaceholder public API using JavaScript's Fetch API. The application demonstrates asynchronous JavaScript, API integration, JSON parsing, error handling, and modern web design.

---

##  Objectives Completed

✅ Fetch data from public API using JavaScript Fetch API  
✅ Parse JSON response data  
✅ Display user information dynamically  
✅ Implement error handling with try-catch  
✅ Add reload functionality  
✅ Create responsive, professional UI  
✅ Test network error scenarios  

---

##  Technologies Used

- **HTML5** - Structure and semantic markup
- **CSS3** - Styling with modern features (Grid, Flexbox, Animations)
- **JavaScript (ES6+)** - Fetch API, Async/Await, DOM manipulation
- **JSONPlaceholder API** - Public REST API for testing

---

##  Features Implemented

### 1. **Data Fetching**
- Uses `fetch()` API to retrieve data from `https://jsonplaceholder.typicode.com/users`
- Implements async/await for clean asynchronous code
- Automatically loads data on page load

### 2. **JSON Parsing**
- Parses JSON response using `response.json()`
- Extracts user details including name, email, address, phone, website, and company

### 3. **Dynamic Display**
- Loops through user array and creates individual user cards
- Displays comprehensive information:
  - Name and username
  - Email address
  - Phone number
  - Complete address with coordinates
  - Website
  - Company details with catchphrase

### 4. **Error Handling**
- Try-catch block for network errors
- HTTP status code validation
- User-friendly error messages
- Graceful degradation

### 5. **User Interface**
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Card Layout**: Grid-based responsive layout
- **Loading States**: Spinner animation while fetching
- **Hover Effects**: Interactive card animations
- **Professional Styling**: Modern gradient background, clean typography

### 6. **Reload Functionality**
- Button to refetch data
- Button state management (disabled during loading)
- Dynamic button text updates

---

##  How to Use

### Setup Instructions:

1. **Save the HTML file**
   - Copy the code to a file named `index.html`

2. **Open in browser**
   - Double-click the file, or
   - Right-click → Open with → Chrome/Firefox/Edge

3. **Test the application**
   - Page automatically loads user data on start
   - Click "Reload Users" to refetch data
   - Disable internet to test error handling

### Testing Error Handling:

1. Open browser DevTools (F12)
2. Go to Network tab
3. Select "Offline" mode
4. Click "Reload Users"
5. Observe error message display

---

##  Code Structure

```
index.html
├── HTML Structure
│   ├── Header with title
│   ├── Controls (Load button)
│   └── Content container (dynamic)
│
├── CSS Styling
│   ├── Responsive grid layout
│   ├── Card design system
│   ├── Loading animations
│   ├── Error states
│   └── Media queries
│
└── JavaScript Logic
    ├── fetchUsers() - Main API call
    ├── displayUsers() - Render user cards
    ├── displayError() - Show error messages
    └── Event handlers
```

---

##  Key JavaScript Concepts Demonstrated

### 1. **Async/Await Pattern**
```javascript
async function fetchUsers() {
    const response = await fetch(API_URL);
    const users = await response.json();
}
```

### 2. **Error Handling**
```javascript
try {
    // API call
} catch (error) {
    // Display error
}
```

### 3. **DOM Manipulation**
```javascript
contentDiv.innerHTML = html;
```

### 4. **JSON Parsing**
```javascript
const users = await response.json();
```

### 5. **Array Iteration**
```javascript
users.forEach(user => {
    // Create cards
});
```

---

## API Endpoint Details

**URL:** `https://jsonplaceholder.typicode.com/users`

**Method:** GET

**Response:** Array of 10 user objects

**User Object Structure:**
```json
{
    "id": 1,
    "name": "Leanne Graham",
    "username": "Bret",
    "email": "Sincere@april.biz",
    "address": {
        "street": "Kulas Light",
        "suite": "Apt. 556",
        "city": "Gwenborough",
        "zipcode": "92998-3874",
        "geo": {
            "lat": "-37.3159",
            "lng": "81.1496"
        }
    },
    "phone": "1-770-736-8031 x56442",
    "website": "hildegard.org",
    "company": {
        "name": "Romaguera-Crona",
        "catchPhrase": "Multi-layered client-server neural-net",
        "bs": "harness real-time e-markets"
    }
}
```

---

##  Design Features

- **Color Scheme**: Purple gradient background with white cards
- **Typography**: Segoe UI font family for readability
- **Spacing**: Generous padding and margins
- **Shadows**: Depth with box-shadows
- **Animations**: Fade-in effects and hover transitions
- **Icons**: Emoji icons for visual context

---

## ✅ Learning Outcomes Achieved

1. ✅ Understanding of asynchronous JavaScript
2. ✅ Working with REST APIs
3. ✅ JSON data parsing and manipulation
4. ✅ Error handling in API calls
5. ✅ DOM manipulation and dynamic content
6. ✅ Responsive web design
7. ✅ Modern CSS techniques (Grid, Flexbox)
8. ✅ User experience considerations (loading states, error messages)

---

##  Browser Compatibility

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)




**Created as Task 7: Fetch and Display Data from Public API**  
**Tools Used:** VS Code, Chrome Browser  
**Deliverable:** Complete functional webpage with user data display
