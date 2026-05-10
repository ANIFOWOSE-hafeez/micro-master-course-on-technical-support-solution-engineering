# Basic JavaScript

> Learn JavaScript as a practical startup skill for support dashboards, web tools, browser automation, and API-driven workflows.

JavaScript is one of the most useful languages in modern technical environments because it powers:
- websites
- dashboards
- browser logic
- frontend interactions
- SaaS tools
- API requests
- internal support portals
- automation in web applications

For Technical Support and Solution Engineering, JavaScript matters because many startup tools live in the browser and many internal tools are web-based.

This lesson teaches JavaScript from a beginner, support-engineer-friendly point of view.

---

# Learning Goals

By the end of this lesson, learners should understand:

- what JavaScript is
- where JavaScript runs
- variables and data types
- conditions
- loops
- functions
- arrays and objects
- browser-based logic
- DOM basics
- events
- simple API requests
- why JavaScript matters in startup environments

---

# What Is JavaScript?

JavaScript is a programming language used to make web pages and web applications interactive.

It is used for:
- buttons
- forms
- dashboards
- data display
- browser interaction
- client-side validation
- API calls
- frontend behavior

---

# Why JavaScript Matters for Support and Solution Engineering

A support engineer or solution engineer may interact with JavaScript when:
- working on internal portals
- debugging web apps
- testing forms
- building support dashboards
- integrating SaaS platforms
- understanding frontend issues
- helping users when something in the browser breaks

---

# Real Startup Examples

JavaScript can help build:
- an internal help desk dashboard
- a ticket submission form
- a password reset portal
- a knowledge base search tool
- a support analytics dashboard
- a simple status page
- a client-side validation workflow

---

# Where JavaScript Runs

JavaScript runs in:
- browsers
- web apps
- Node.js servers
- frontend frameworks
- internal tools

For beginners, the most important place is the browser.

---

# Your First JavaScript Code

```javascript
console.log("Welcome to Technical Support Engineering");
```

`console.log()` prints output to the browser console or terminal.

---

# How to Open the Browser Console

In most browsers:
- right click
- inspect
- go to Console

You can then run JavaScript directly there.

---

# Variables

Variables store data.

---

# Example

```javascript
let username = "hafeez";
let ticketCount = 12;
let systemOnline = true;
```

---

# Variable Keywords

| Keyword | Meaning |
|---|---|
| `let` | value can change |
| `const` | value should not change |
| `var` | older JavaScript style |

---

# Best Practice

Use:
- `let` for values that may change
- `const` for values that stay constant

Example:
```javascript
const companyName = "Startup Ops";
let openTickets = 18;
```

---

# Data Types

JavaScript has several important data types.

---

# String

Text data.

```javascript
let name = "Support Team";
```

---

# Number

Numeric values.

```javascript
let cpuUsage = 92;
```

---

# Boolean

True/false values.

```javascript
let serverOnline = true;
```

---

# Array

Stores multiple items.

```javascript
let servers = ["api-1", "db-1", "auth-1"];
```

---

# Object

Stores structured data.

```javascript
let ticket = {
  user: "alice",
  priority: "high",
  status: "open"
};
```

---

# Why Objects Matter

Objects are extremely important because APIs often return data in object-like formats.

Example:
```json
{
  "status": "open",
  "priority": "high"
}
```

---

# Comments

Comments explain code.

```javascript
// Check ticket priority
```

---

# Why Comments Matter

In startup teams, code must often be understood quickly by:
- support engineers
- developers
- product teams
- new hires

Clear comments improve collaboration.

---

# Basic Operators

---

# Arithmetic Operators

| Operator | Meaning |
|---|---|
| `+` | add |
| `-` | subtract |
| `*` | multiply |
| `/` | divide |
| `%` | remainder |

Example:
```javascript
let total = 5 + 3;
```

---

# Comparison Operators

| Operator | Meaning |
|---|---|
| `==` | equal |
| `===` | strictly equal |
| `!=` | not equal |
| `>` | greater than |
| `<` | less than |
| `>=` | greater or equal |
| `<=` | less or equal |

Example:
```javascript
if (cpuUsage > 90) {
  console.log("High CPU alert");
}
```

---

# Conditions

Conditions allow decision-making.

```javascript
let diskUsage = 92;

if (diskUsage > 85) {
  console.log("Disk space is getting low");
}
```

---

# Real Startup Example

A support dashboard may show:
- red alert if CPU is too high
- yellow alert if memory is moderate
- green status if everything is fine

---

# Else If

```javascript
let priority = "high";

if (priority === "critical") {
  console.log("Escalate immediately");
} else if (priority === "high") {
  console.log("Fast response required");
} else {
  console.log("Normal handling");
}
```

---

# Loops

Loops repeat actions.

---

# For Loop

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

---

# Real Startup Example

```javascript
let servers = ["api", "db", "auth"];

for (let i = 0; i < servers.length; i++) {
  console.log("Checking " + servers[i]);
}
```

---

# While Loop

```javascript
let count = 0;

while (count < 3) {
  console.log(count);
  count++;
}
```

---

# Functions

Functions organize reusable logic.

---

# Example

```javascript
function greet() {
  console.log("Welcome");
}
```

Call it:
```javascript
greet();
```

---

# Functions With Parameters

```javascript
function greetUser(name) {
  console.log("Hello " + name);
}
```

---

# Return Values

```javascript
function add(a, b) {
  return a + b;
}
```

---

# Why Functions Matter

Functions help you write:
- cleaner code
- reusable logic
- manageable automation
- maintainable support tooling

---

# Arrays

Arrays store ordered lists.

Example:
```javascript
let tickets = ["VPN issue", "Login issue", "Printer issue"];
```

---

# Useful Array Methods

```javascript
tickets.push("Password reset");
```

```javascript
tickets.length
```

```javascript
tickets[0]
```

---

# Objects

Objects group related data.

Example:
```javascript
let user = {
  name: "Alice",
  team: "Support",
  active: true
};
```

---

# Access Object Properties

```javascript
console.log(user.name);
console.log(user.team);
```

---

# Real Startup Example

A support portal may store ticket data like this:

```javascript
let ticket = {
  id: "TCK-1001",
  subject: "VPN not working",
  priority: "high",
  assignedTeam: "network"
};
```

---

# DOM Basics

DOM means Document Object Model.

The DOM is how JavaScript interacts with HTML on a web page.

---

# Why DOM Matters

Support dashboards, forms, and internal tools often need:
- button clicks
- live updates
- form validation
- showing/hiding content
- status changes

---

# Example HTML

```html
<button id="checkButton">Check Status</button>
<p id="statusText"></p>
```

---

# Example JavaScript DOM Interaction

```javascript
const button = document.getElementById("checkButton");
const statusText = document.getElementById("statusText");

button.addEventListener("click", function () {
  statusText.textContent = "System check started";
});
```

---

# Why This Is Useful

A startup support portal may use this to:
- submit a ticket
- show validation errors
- update dashboard metrics
- trigger a search result
- refresh status cards

---

# Events

Events are actions that happen in the browser.

Examples:
- click
- submit
- hover
- keypress
- change

---

# Event Listener Example

```javascript
button.addEventListener("click", function () {
  console.log("Button clicked");
});
```

---

# Forms

JavaScript is often used to validate forms.

Example:
```javascript
const form = document.getElementById("supportForm");

form.addEventListener("submit", function (event) {
  event.preventDefault();
  console.log("Form submitted");
});
```

---

# Real Startup Example

A ticket submission form may:
- validate required fields
- check email format
- display errors
- send data to an API

---

# Working With APIs

JavaScript can call APIs using `fetch()`.

Example:
```javascript
fetch("https://api.github.com")
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error(error));
```

---

# Why API Calls Matter

Modern startup tools often connect to:
- ticketing systems
- identity platforms
- status pages
- monitoring services
- knowledge bases

JavaScript is commonly used in browser-based integrations.

---

# Real Startup Use Case

A support dashboard may:
- fetch live ticket counts
- display uptime status
- load user account data
- update support metrics

---

# JSON and JavaScript

JavaScript works naturally with JSON.

Example:

```javascript
let ticket = {
  subject: "VPN not working",
  priority: "high"
};
```

This is similar to JSON used by APIs.

---

# Basic Error Handling

```javascript
try {
  console.log(missingValue);
} catch (error) {
  console.log("Something went wrong");
}
```

---

# Why Error Handling Matters

Startup systems must fail gracefully:
- API outages
- missing data
- invalid user input
- broken dashboards

---

# Console Debugging

The browser console is a support engineer’s friend.

Examples:
```javascript
console.log("Debug message");
console.warn("Warning message");
console.error("Error message");
```

---

# Beginner Debugging Mindset

A beginner should always ask:
- Did the event fire?
- Did the data load?
- Did the API respond?
- Is the DOM element available?
- Is the browser showing an error?

---

# Real Startup Example

A user says:
> "The support form does not submit."

Possible JavaScript causes:
- validation failed
- button event not attached
- API request failed
- browser error occurred
- form ID is wrong

---

# JavaScript for Support Engineers

Useful applications include:

| Use Case | Example |
|---|---|
| Ticket forms | Validation |
| Dashboards | Live updates |
| Internal tools | Button interactions |
| Help portals | Search and filters |
| Status pages | Dynamic data display |
| API testing | Fetch requests |

---

# Example: Simple Ticket Counter

```javascript
let openTickets = 14;

if (openTickets > 10) {
  console.log("Support backlog is high");
} else {
  console.log("Support load is manageable");
}
```

---

# Example: Queue Routing Display

```javascript
let team = "network";

if (team === "network") {
  console.log("Route to Tier 2 Network");
}
```

---

# Example: Status Indicator

```javascript
let systemHealthy = true;

if (systemHealthy) {
  console.log("System online");
} else {
  console.log("System down");
}
```

---

# Startup Engineering Mindset

Good JavaScript code should be:
- clear
- readable
- reusable
- easy to debug
- useful for users
- easy to maintain

---

# Common Beginner Mistakes

| Mistake | Better Approach |
|---|---|
| Using `var` everywhere | Prefer `let` and `const` |
| Forgetting semicolons is okay sometimes | Keep code consistent |
| Ignoring console errors | Read them carefully |
| Hardcoding everything | Use variables |
| Writing messy logic | Use functions |
| Not checking null values | Validate carefully |

---

# Mini Exercises

---

# Exercise 1 — Greeting Message

```javascript
let name = "Hafeez";
console.log("Welcome " + name);
```

---

# Exercise 2 — Priority Check

```javascript
let priority = "high";

if (priority === "high") {
  console.log("Handle quickly");
}
```

---

# Exercise 3 — Ticket Loop

```javascript
let tickets = ["VPN", "Login", "Printer"];

for (let i = 0; i < tickets.length; i++) {
  console.log(tickets[i]);
}
```

---

# Exercise 4 — Support Form Button

Create a button that displays:
> Ticket submitted

when clicked.

---

# Exercise 5 — API Request

Use `fetch()` to load data from a public API and display the result in the console.

---

# Beginner Project Idea

## Support Dashboard Interaction Demo

Build a simple browser-based page that:
- shows ticket count
- changes status colors
- handles button clicks
- loads mock API data
- demonstrates support workflow logic

---

# Real Skills Built Here

This lesson develops:
- frontend thinking
- browser logic
- API awareness
- debugging skills
- user interface reasoning
- startup tool familiarity

These skills matter later for:
- support dashboards
- internal portals
- customer tools
- solution demos
- SaaS integrations

---

# Key Takeaways

- JavaScript powers interactive web applications
- It is important for support dashboards and internal tools
- DOM and event handling are essential
- APIs and JSON are central to modern applications
- Debugging in the browser is a valuable skill
- Clean code helps startup teams move faster

---

# Next Lesson

Continue to:

```bash
git-and-github.md
```

The next lesson explains:
- version control
- repository management
- commits
- branches
- pull requests
- professional GitHub workflows
- how engineers collaborate in startups
