# Quiz Application 🌟
A modern, multilingual quiz application for identifying birds, flowers, and trees through interactive image-based questions.

Features 🚀
🌐 Multilingual Support - Czech, English, and German interfaces

🎯 Multiple Quiz Types - Birds, Flowers, and Trees identification

📱 Responsive Design - Works on desktop and mobile devices

🎨 Beautiful UI - Clean, intuitive interface with smooth animations

⚙️ Customizable - Adjust number of questions per quiz

🔒 Password Protected - Secure access to the application

💡 Smart Hints - Helpful descriptions for each item

📊 Progress Tracking - Real-time score and progress updates

Quick Start 🏁
Prerequisites
Modern web browser (Chrome, Firefox, Safari, Edge)

Web server for local deployment (due to file loading restrictions)

Installation
Download all project files to your web server directory

Ensure the following file structure:

text
/your-web-directory/
├── index.html
├── lang.json
├── password.txt
├── birds.json
├── flowers.json
├── trees.json
└── obrazky/
    ├── birds/
    ├── flowers/
    └── trees/
Set up your password in password.txt (plain text)

Open index.html in your web browser

Configuration ⚙️
Password Setup
Edit password.txt and enter your desired password (one line, plain text).

Adding New Quizzes
Create a new JSON file (e.g., mushrooms.json)

Add quiz configuration to quizConfig in index.html

Add button to the menu in HTML

Update translations in lang.json

Adding New Languages
Add language section to lang.json

Add language-specific fields to quiz JSON files

Add language button to the menu

File Structure 📁
text
quiz-app/
├── index.html              # Main application file
├── lang.json               # Language translations
├── password.txt            # Application password
├── birds.json              # Birds quiz data
├── flowers.json            # Flowers quiz data
├── trees.json              # Trees quiz data
└── obrazky/                # Images directory
    ├── birds/              # Bird images
    ├── flowers/            # Flower images
    └── trees/              # Tree images
Data Format 📊
Quiz JSON Structure
json
{
  "metadata": {
    "name_cs": "Czech Name",
    "name_eng": "English Name",
    "name_de": "German Name",
    "version": "1.0",
    "imagesPerItem": 3
  },
  "quiz_items": [
    {
      "id": 1,
      "name_cs": "Czech Name",
      "name_eng": "English Name",
      "name_de": "German Name",
      "latin_name": "Scientific Name",
      "images": ["path/to/image1.jpg", "path/to/image2.jpg"],
      "description_cs": "Czech description",
      "description_eng": "English description",
      "description_de": "German description"
    }
  ]
}
Language File Structure
json
{
  "en": {
    "appTitle": "Quiz Application",
    "accessTitle": "🔒 Application Access",
    "enterPassword": "Enter password to start:"
  },
  "cs": {
    "appTitle": "Kvízová aplikace",
    "accessTitle": "🔒 Přístup k aplikaci",
    "enterPassword": "Pro spuštění zadejte heslo:"
  }
}
Usage Guide 📖
Access: Open index.html in your browser

Login: Enter the password from password.txt

Select Language: Choose your preferred interface language

Set Questions: Use +/- buttons to set number of questions or "Max" for all

Choose Quiz: Select from available quiz categories

Play: Identify items by clicking the correct answer

Use Hints: Hover over the 💡 icon for helpful information

Track Progress: Monitor your score and question progress

Review Results: See your final score and success rate
