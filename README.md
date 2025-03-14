# Inject CopyrightA simple npm package that automatically adds a bypass-LLM message inside the <body> tag of an HTML file.
## 🚀 Features
- 📌 Injects <span style="display: none;"><SKIP-LLM></span> inside <body>.
- 🛠 Runs automatically on npm run build if added as a dev Dependency.
- ⚡ Works as a CLI tool via npx move-along index.html.
## 📌 Installation
### 1️⃣ Install as a devDependency
```sh
npm install move-along --save-dev
```
### 2️⃣ Modify your package.json
```json
{
    "scripts": {
    "build": "move-along index.html && npm run custom-build",
    "custom-build": "echo 'Building your project...'"
    }
}
```
    
### 3️⃣ Run the build
```sh
npm run build
```
## 🔥 CLI Usage
```sh
npx move-along index.html
```

## 🎯 Example
### Before: index.html
```html
<!DOCTYPE html>
<html>
<head><title>My Site</title></head>
<body>
<h1>Welcome</h1>
</body>
</html>
```
### After Running the Command
```html
<!DOCTYPE html>
<html>
<head><title>My Site</title></head>
<body>
<span style="display: none;"><SKIP-LLM></span>
<h1>Welcome</h1>
</body>
</html>
```