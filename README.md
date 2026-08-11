# ⌨️ Typing Speed Tester

A simple and interactive **Typing Speed Tester** built using **HTML, CSS, and JavaScript**.

The application allows users to test their typing speed, accuracy, and number of typing errors within a 60-second typing challenge.

## 🚀 Features

* ⏱️ 60-second typing test
* ⚡ Real-time WPM calculation
* 🎯 Real-time accuracy calculation
* ❌ Error tracking
* 📝 Random typing passages
* 🟢 Correct character highlighting
* 🔴 Incorrect character highlighting
* 🔵 Current character indicator
* 🏆 Best WPM score tracking
* 💾 Best score saved using Local Storage
* 🔄 Restart test functionality
* 📱 Responsive design
* 🎨 Clean and simple user interface

## 🛠️ Technologies Used

* HTML5
* CSS3
* JavaScript
* DOM Manipulation
* Browser Local Storage

## 📂 Project Structure

```text
typing-speed-tester/
│
├── index.html
├── style.css
├── script.js
└── README.md
```

## ⚙️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/typing-speed-tester.git
```

### 2. Open the project

Navigate to the project directory:

```bash
cd typing-speed-tester
```

### 3. Run the project

Open `index.html` in your browser.

You can also use **VS Code Live Server** for a better development experience.

## 🎮 How to Use

1. Open the application.
2. Click **Start Test**.
3. Start typing the displayed passage.
4. Type as accurately and quickly as possible.
5. The timer will count down from 60 seconds.
6. Your WPM, accuracy, and errors will update in real time.
7. After the test finishes, your final score will be displayed.
8. Your highest WPM score is automatically saved in the browser.

## 📊 How WPM Is Calculated

The application uses the standard typing-speed calculation:

```text
WPM = Correct Characters / 5 / Time in Minutes
```

For example, if a user types 250 correct characters in 1 minute:

```text
WPM = 250 / 5 / 1
    = 50 WPM
```

## 🎯 Accuracy Calculation

Accuracy is calculated using:

```text
Accuracy = Correct Characters / Total Typed Characters × 100
```

## 🏆 Best Score

The highest WPM score is stored using the browser's:

```javascript
localStorage
```

This means the best score remains available even after refreshing the page.

## 🔮 Future Improvements

Possible features that can be added in future versions:

* [ ] Difficulty levels
* [ ] Multiple test durations
* [ ] Custom passages
* [ ] Dark mode
* [ ] Typing history
* [ ] WPM performance graph
* [ ] Leaderboard
* [ ] User profiles
* [ ] Sound effects
* [ ] Keyboard visualization
* [ ] Multiplayer typing competition
* [ ] More typing passages
* [ ] Mobile-friendly virtual keyboard

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a new branch.

```bash
git checkout -b feature/new-feature
```

3. Make your changes.
4. Commit your changes.

```bash
git commit -m "Add new feature"
```

5. Push the branch.

```bash
git push origin feature/new-feature
```

6. Open a Pull Request.

## 📄 License

This project is open-source and available under the MIT License.

## 👨‍💻 Author

**Ronak Sharma**

If you found this project useful, consider giving the repository a ⭐ on GitHub!
