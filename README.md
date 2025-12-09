
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitBanner</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <div class="noise"></div>
    
    <!-- GitHub-style light effects -->
    <div class="light-effect light-effect-1"></div>
    <div class="light-effect light-effect-2"></div>
    <div class="light-effect light-effect-3"></div>
    
    <header>
        <div class="logo">
            <svg height="32" aria-hidden="true" viewBox="0 0 16 16" version="1.1" width="32" data-view-component="true" class="octicon octicon-mark-github v-align-middle">
                <path d="M8 0c4.42 0 8 3.58 8 8a8.013 8.013 0 0 1-5.45 7.59c-.4.08-.55-.17-.55-.38 0-.27.01-1.13.01-2.2 0-.75-.25-1.23-.54-1.48 1.78-.2 3.65-.88 3.65-3.95 0-.88-.31-1.59-.82-2.15.08-.2.36-1.02-.08-2.12 0 0-.67-.22-2.2.82-.64-.18-1.32-.27-2-.27-.68 0-1.36.09-2 .27-1.53-1.03-2.2-.82-2.2-.82-.44 1.1-.16 1.92-.08 2.12-.51.56-.82 1.28-.82 2.15 0 3.06 1.86 3.75 3.64 3.95-.23.2-.44.55-.51 1.07-.46.21-1.61.55-2.33-.66-.15-.24-.6-.83-1.23-.82-.67.01-.27.38.01.53.34.19.73.9.82 1.13.16.45.68 1.31 2.69.94 0 .67.01 1.3.01 1.49 0 .21-.15.45-.55.38A7.995 7.995 0 0 1 0 8c0-4.42 3.58-8 8-8Z"></path>
            </svg>
            <span>GitBanner <sup><span style="color: #9e9e9e9c;font-size: small;font-weight: 300;">Beta</span></sup></span>
        </div>
        <nav>
            <a href="#" class="active">Home</a>
            <a href="https://github.com/Saviru/Animated-Profile-Banner-Generator/blob/main/README.md">About</a>
            <a href="https://github.com/Saviru/Animated-Profile-Banner-Generator/issues/new?template=bug_report.md">Bug Report</a>
            <a href="https://github.com/Saviru/Animated-Profile-Banner-Generator/issues/new?template=feature_request.md">Feature Request</a>
        </nav>
    </header>

    <main>
        <div class="hero">
            <div class="glass-card">
                <h1>Animated GitHub Profile Banner Generator</h1>
                <p>Create a unique animated GitHub profile banner with terminal-style loading, glitch effects, and metal textures.</p>
            </div>
        </div>

        <div class="container">
            <div class="glass-card editor">
                <form id="profile-form">
                    <div class="form-group">
                        <label for="input-username">Username</label>
                        <input type="text" id="input-username" placeholder="Enter username" value="Saviru">
                    </div>
                    <div class="form-group">
                        <label for="input-fullname">Full Name</label>
                        <input type="text" id="input-fullname" placeholder="Enter full name" value="Saviru Kashmira Atapattu">
                    </div>
                    <div class="form-group">
                        <label for="input-description">Description</label>
                        <input type="text" id="input-description" placeholder="Enter description" value="Developer | Tech Explorer | Designer">
                    </div>

                    <div class="form-group">
                        <label for="animate-profile">
                            <input type="checkbox" id="animate-profile" disabled>
                            Repeat Animation
                            <span style="font-weight: 200;color: #ff0000b0;">(Not Available)</span>
                        </label>
                    </div>
                    <button type="button" id="generate-button" class="btn-primary">
                        <i class="fa-regular fa-image fa-beat"></i>
                        Generate Preview
                    </button>
                    <button type="button" class="btn-secondary" id="reset-form"><i class="fa-solid fa-square-minus" style="color: #ff0000;"></i> Reset</button>
                </form>
            </div>
        </div>

        <div class="result-preview hidden" id="result-container">
            <div class="glass-card result">
                <h2>Generated Profile</h2>
                <div class="profile-result" id="result-preview">
                    <!-- Preview will be inserted here -->
                </div>
                <div class="button-group">
                    <button id="download-svg" class="btn-download">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path>
                            <polyline points="7 10 12 15 17 10"></polyline>
                            <line x1="12" y1="15" x2="12" y2="3"></line>
                        </svg>
                        Download SVG
                    </button>
                </div>
            </div>
        </div>

        <div class="features" id="about">
            <div class="glass-card feature">
                <div class="feature-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M12 20h9"></path>
                        <path d="M16.5 3.5a2.121 2.121 0 0 1 3 3L7 19l-4 1 1-4L16.5 3.5z"></path>
                    </svg>
                </div>
                <h3>Terminal Animation</h3>
                <p>Animated terminal with loading progress and command-line interface</p>
                <div class="reflect-light"></div>
            </div>
            <div class="glass-card feature">
                <div class="feature-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path>
                        <polyline points="7 10 12 15 17 10"></polyline>
                        <line x1="12" y1="15" x2="12" y2="3"></line>
                    </svg>
                </div>
                <h3>Download SVG</h3>
                <p>Download your customized profile as SVG</p>
                <div class="reflect-light"></div>
            </div>
            <div class="glass-card feature">
                <div class="feature-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M12 3a6.364 6.364 0 0 0 9 9 9 9 0 1 1-9-9Z"></path>
                    </svg>
                </div>
                <h3>Glitch Effects</h3>
                <p>Modern glitch effects with animated welcome text and visual distortions</p>
                <div class="reflect-light"></div>
            </div>
        </div>
    </main>
    
    <footer>
        <p>GitBanner v0.25.9.1 (Beta)</p>
        <p>Copyright &copy; 2025 Saviru Kashmira Atapattu</p>
        <div class="footer-links">
            <a href="https://github.com/Saviru/Animated-Profile-Banner-Generator/blob/main/LICENSE">Terms of Service</a>
            <a href="https://github.com/Saviru">Developer</a>
            <a href="https://github.com/Saviru/Animated-Profile-Banner-Generator">Source Code</a>
        </div>
        <br>
        <p style="font-size: small;">Made with ❤️ for the GitHub community</p>
    </footer>

    <!-- Hidden SVG for generating the profile -->
    <div style="display: none;">

        <img src="profileBanner.svg" id="profile-svg">
        
    </div>

    <script src="script.js"></script>
</body>
</html>

document.addEventListener('DOMContentLoaded', function() {
    // Get form elements
    const form = document.getElementById('profile-form');
    const usernameInput = document.getElementById('input-username');
    const fullnameInput = document.getElementById('input-fullname');
    const descriptionInput = document.getElementById('input-description');
    const animateCheckbox = document.getElementById('animate-profile');
    
    // Get SVG image element
    const profileSvgImg = document.getElementById('profile-svg');
    
    // Reset button and generate button
    const resetButton = document.getElementById('reset-form');
    const generateButton = document.getElementById('generate-button');
    
    // Download button
    const downloadButton = document.getElementById('download-svg');
    
    // Result container
    const resultContainer = document.getElementById('result-container');
    const resultPreview = document.getElementById('result-preview');
    
    // Default values
    const defaults = {
        username: 'Saviru',
        fullname: 'Saviru Kashmira Atapattu',
        description: 'Developer | Tech Explorer | Designer',
        animate: false
    };
    
    
    // Function to show notification
    function showNotification(message, type) {
        // Create notification element
        const notification = document.createElement('div');
        notification.className = `notification ${type}`;
        notification.textContent = message;
        
        // Style the notification
        notification.style.position = 'fixed';
        notification.style.bottom = '20px';
        notification.style.right = '20px';
        notification.style.padding = '12px 24px';
        notification.style.borderRadius = '8px';
        notification.style.zIndex = '1000';
        notification.style.backgroundColor = type === 'success' ? 'rgba(63, 185, 80, 0.9)' : 
                                            type === 'error' ? 'rgba(248, 81, 73, 0.9)' :
                                            'rgba(88, 166, 255, 0.9)';
        notification.style.color = 'white';
        notification.style.backdropFilter = 'blur(10px)';
        notification.style.boxShadow = '0 5px 15px rgba(0, 0, 0, 0.2)';
        notification.style.border = '1px solid rgba(48, 54, 61, 0.5)';
        notification.style.transform = 'translateY(20px)';
        notification.style.opacity = '0';
        notification.style.transition = 'all 0.3s ease';
        
        // Add to DOM
        document.body.appendChild(notification);
        
        // Animate in
        setTimeout(() => {
            notification.style.transform = 'translateY(0)';
            notification.style.opacity = '1';
        }, 10);
        
        // Remove after delay
        setTimeout(() => {
            notification.style.opacity = '0';
            notification.style.transform = 'translateY(20px)';
            
            setTimeout(() => {
                document.body.removeChild(notification);
            }, 300);
        }, 3000);
    }
    
    // Initialize the form with default values
    usernameInput.value = defaults.username;
    fullnameInput.value = defaults.fullname;
    descriptionInput.value = defaults.description;
    animateCheckbox.checked = defaults.animate;
    
    // Variable to track current SVG content and blob URL
    let currentSvgContent = null;
    let currentBlobUrl = null;
    
    // Generate button click handler
    generateButton.addEventListener('click', function() {
        // Show loading state
        generateButton.innerHTML = '<i class="fa-solid fa-spinner fa-spin"></i> Generating...';
        generateButton.disabled = true;
        
        // Fetch the profileBanner.svg file
        fetch('profileBanner.svg')
            .then(response => {
                if (!response.ok) {
                    throw new Error('Could not load profileBanner.svg');
                }
                return response.text();
            })
            .then(svgContent => {
                // Get form values
                const username = usernameInput.value || defaults.username;
                const fullname = fullnameInput.value || defaults.fullname;
                const description = descriptionInput.value || defaults.description;
                
                // Create a modified version of the SVG with user data
                let modifiedSvg = svgContent;
                
                // Replace the actual text content in the SVG
                // Replace the username in the command prompt
                //modifiedSvg = modifiedSvg.replace(/saviru@github/g, username.toLowerCase() + '@github');
                //modifiedSvg = modifiedSvg.replace(/GET profile Saviru --verbose/g, `GET profile ${username} --verbose`);
                //modifiedSvg = modifiedSvg.replace(/Loading Saviru's profile\.\.\./g, `Loading ${username}'s profile...`);
                modifiedSvg = modifiedSvg.replace(/{UsernameCMD}/g, username.toLowerCase());
                modifiedSvg = modifiedSvg.replace(/{Username}/g, username);
                
                
                // Replace the full name (appears twice in the SVG)
                modifiedSvg = modifiedSvg.replace(/{Fullname}/g, fullname);
                
                // Replace the description/tagline
                modifiedSvg = modifiedSvg.replace(/{Tagline}/g, description);
                
                // Store the modified SVG content
                currentSvgContent = modifiedSvg;
                
                // Display the result
                resultPreview.innerHTML = modifiedSvg;
                resultContainer.classList.remove('hidden');
                
                // Scroll to result
                resultContainer.scrollIntoView({ behavior: 'smooth' });
                
                // Show success notification
                showNotification('Profile banner generated successfully!', 'success');
                
                // Reset button state
                generateButton.innerHTML = '<i class="fa-regular fa-image fa-beat"></i> Generate Preview';
                generateButton.disabled = false;
            })
            .catch(error => {
                console.error('Error loading SVG:', error);
                showNotification('Error loading profile banner: ' + error.message, 'error');
                
                // Reset button state
                generateButton.innerHTML = '<i class="fa-regular fa-image fa-beat"></i> Generate Preview';
                generateButton.disabled = false;
            });
    });
    
    // Download button click handler
    downloadButton.addEventListener('click', function() {
        if (!currentSvgContent) {
            showNotification('Please generate a profile banner first!', 'error');
            return;
        }
        
        try {
            // Clean up previous blob URL
            if (currentBlobUrl) {
                URL.revokeObjectURL(currentBlobUrl);
            }
            
            // Create blob from SVG content
            const blob = new Blob([currentSvgContent], { type: 'image/svg+xml' });
            currentBlobUrl = URL.createObjectURL(blob);
            
            // Get username for filename
            const username = usernameInput.value || defaults.username;
            const filename = `${username}-profile-banner.svg`;
            
            // Create download link and trigger download
            const downloadLink = document.createElement('a');
            downloadLink.href = currentBlobUrl;
            downloadLink.download = filename;
            downloadLink.style.display = 'none';
            
            document.body.appendChild(downloadLink);
            downloadLink.click();
            document.body.removeChild(downloadLink);
            
            showNotification(`Downloaded ${filename} successfully!`, 'success');
        } catch (error) {
            console.error('Download error:', error);
            showNotification('Error downloading file: ' + error.message, 'error');
        }
    });
    
    // Clean up blob URLs when page unloads
    window.addEventListener('beforeunload', function() {
        if (currentBlobUrl) {
            URL.revokeObjectURL(currentBlobUrl);
        }
    });
});

:root {
    /* GitHub Home colors */
    --bg-dark: #0d1117;
    --bg-darker: #010409;
    --text-primary: #f0f6fc;
    --text-secondary: #8b949e;
    --accent-blue: #58a6ff;
    --accent-blue-dark: #1f6feb;
    --accent-green: #3fb950;
    --accent-purple: #8957e5;
    --accent-coral: #f85149;
    --border-color: #30363d;
    --card-bg: rgba(22, 27, 34, 0.7);
    --btn-primary-bg: #238636;
    --btn-primary-hover: #2ea043;
    --btn-secondary-bg: #21262d;
    --btn-secondary-hover: #30363d;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
    background-color: var(--bg-dark);
    color: var(--text-primary);
    line-height: 1.5;
    position: relative;
    min-height: 100vh;
    overflow-x: hidden;
}

/* Noise overlay */
.noise {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: url('data:image/png;base64,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');
    opacity: 0.03;
    z-index: -1;
    pointer-events: none;
}

/* GitHub-style Light Effect */
.light-effect {
    position: fixed;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, rgba(255,255,255,0) 70%);
    filter: blur(50px);
    z-index: -1;
    opacity: 0.5;
    pointer-events: none;
}

.light-effect-1 {
    width: 800px;
    height: 800px;
    top: -200px;
    right: -200px;
    animation: move-light-1 30s infinite alternate ease-in-out;
}

.light-effect-2 {
    width: 600px;
    height: 600px;
    bottom: -100px;
    left: -100px;
    animation: move-light-2 25s infinite alternate ease-in-out;
}

.light-effect-3 {
    width: 400px;
    height: 400px;
    top: 40%;
    left: 30%;
    animation: move-light-3 20s infinite alternate ease-in-out;
}

@keyframes move-light-1 {
    0% { transform: translateX(0) translateY(0); opacity: 0.3; }
    50% { transform: translateX(-100px) translateY(100px); opacity: 0.5; }
    100% { transform: translateX(100px) translateY(-100px); opacity: 0.3; }
}

@keyframes move-light-2 {
    0% { transform: translateX(0) translateY(0); opacity: 0.3; }
    50% { transform: translateX(200px) translateY(-50px); opacity: 0.5; }
    100% { transform: translateX(-100px) translateY(100px); opacity: 0.3; }
}

@keyframes move-light-3 {
    0% { transform: translateX(0) translateY(0); opacity: 0.3; }
    50% { transform: translateX(-150px) translateY(50px); opacity: 0.5; }
    100% { transform: translateX(100px) translateY(-150px); opacity: 0.3; }
}

/* Glass Card Effect with Reflection */
.glass-card {
    background-color: var(--card-bg);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    border-radius: 16px;
    border: 1px solid rgba(48, 54, 61, 0.8);
    box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
    padding: 2rem;
    margin-bottom: 2rem;
    position: relative;
    overflow: hidden;
    z-index: 1;
    transition: all 0.3s ease;
}

.glass-card::after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(120deg, rgba(255, 255, 255, 0.05) 0%, transparent 40%);
    z-index: -1;
    pointer-events: none;
}

/* Card reflection effect */
.reflect-light {
    position: absolute;
    top: -100%;
    left: -100%;
    width: 300%;
    height: 300%;
        position: absolute;
    left: 20%;
    width: 60%;
    padding: 30% 0;
    transform: translate(0, -70%) rotate(-45deg);
    background: radial-gradient(circle at left bottom, #e6b7fe57 10%, #4f49c26b 20%, rgba(87, 78, 255, 0) 60%);
    filter: blur(40px);
    animation: reflect-animation 8s linear infinite;
    pointer-events: none;
    z-index: 0;
    opacity: 0.7;
}

@keyframes reflect-animation {
    0% {
        transform: rotate(0) translate(-50%, -50%);
    }
    100% {
        transform: rotate(360deg) translate(-50%, -50%);
    }
}

/* Header */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    border-bottom: 1px solid var(--border-color);
    position: sticky;
    top: 0;
    background-color: rgba(13, 17, 23, 0.8);
    backdrop-filter: blur(16px);
    -webkit-backdrop-filter: blur(16px);
    z-index: 100;
}

.logo {
    display: flex;
    align-items: center;
    gap: 0.75rem;
    font-weight: 600;
    font-size: 1.2rem;
}

.logo svg {
    fill: var(--text-primary);
}

nav {
    display: flex;
    gap: 1.5rem;
}

nav a {
    color: var(--text-secondary);
    text-decoration: none;
    font-weight: 500;
    padding: 0.5rem;
    transition: color 0.2s ease;
    position: relative;
}

nav a:hover, nav a.active {
    color: var(--text-primary);
}

nav a.active::after {
    content: '';
    position: absolute;
    bottom: -1px;
    left: 0;
    width: 100%;
    height: 2px;
    background-color: var(--accent-blue);
    border-radius: 2px;
}

/* Main Content */
main {
    max-width: 1200px;
    margin: 0 auto;
    padding: 2rem;
}

.hero {
    text-align: center;
    margin-bottom: 3rem;
}

.hero .glass-card {
    width: 100%;
    margin: 0 auto;
    background-color: rgba(22, 27, 34, 0.5);
    position: relative;
    overflow: hidden;
}

.hero h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    background: linear-gradient(to right, var(--accent-blue), var(--accent-green));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: gradient-text 8s ease infinite;
    background-size: 200% auto;
}

@keyframes gradient-text {
    0% {
        background-position: 0% center;
    }
    50% {
        background-position: 100% center;
    }
    100% {
        background-position: 0% center;
    }
}

.hero p {
    font-size: 1.1rem;
    color: var(--text-secondary);
}

/* Animated Gradient */
.animate-gradient {
    position: relative;
}

.animate-gradient::before {
    content: '';
    position: absolute;
    top: -2px;
    left: -2px;
    right: -2px;
    bottom: -2px;
    background: linear-gradient(45deg, var(--accent-blue), var(--accent-green), var(--accent-purple), var(--accent-coral));
    z-index: -1;
    border-radius: 18px;
    background-size: 400% 400%;
    animation: gradient-border 15s ease infinite;
    opacity: 0.7;
}

@keyframes gradient-border {
    0% {
        background-position: 0% 50%;
    }
    50% {
        background-position: 100% 50%;
    }
    100% {
        background-position: 0% 50%;
    }
}

/* Container */
.container {
    display: grid;
    grid-template-columns: 1fr;
    gap: 2rem;
}

.editor {
    width: 100%;
    margin: 0 auto;
}

.profile-result {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 2rem;
    border-radius: 12px;
    background-color: rgba(13, 17, 23, 0.5);
    box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.3);
    margin-bottom: 1.5rem;
}

.svg-text {
    fill: var(--text-primary);
    font-family: 'Inter', sans-serif;
}

text.username {
    font-size: 22px;
    font-weight: bold;
    fill: var(--accent-blue);
}

text.fullname {
    font-size: 18px;
    fill: var(--text-primary);
}

text.description {
    font-size: 14px;
    fill: var(--text-secondary);
}

.button-group {
    display: flex;
    justify-content: center;
    gap: 1rem;
    margin-top: 1.5rem;
}

.btn-download {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    background-color: var(--btn-secondary-bg);
    color: var(--text-primary);
    padding: 0.75rem 1.5rem;
    border-radius: 8px;
    border: 1px solid var(--border-color);
    font-weight: 600;
    cursor: pointer;
    transition: all 0.2s ease;
}

.btn-download:hover {
    background-color: var(--btn-secondary-hover);
    border-color: var(--accent-blue);
    box-shadow: 0 0 10px rgba(88, 166, 255, 0.3);
}

/* Form */
form {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}

.form-group {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}

label {
    font-size: 0.9rem;
    font-weight: 500;
    color: var(--text-secondary);
}

input[type="text"] {
    padding: 0.75rem 1rem;
    border-radius: 8px;
    border: 1px solid var(--border-color);
    background-color: rgba(13, 17, 23, 0.5);
    color: var(--text-primary);
    font-family: 'Inter', sans-serif;
    transition: all 0.2s ease;
    width: 100%;
    font-size: 1rem;
}

input[type="color"] {
    width: 100%;
    height: 40px;
    border-radius: 8px;
    border: 1px solid var(--border-color);
    background-color: rgba(13, 17, 23, 0.5);
    cursor: pointer;
    transition: all 0.2s ease;
}

input[type="checkbox"] {
    margin-right: 8px;
}

.gradient-inputs {
    display: flex;
    gap: 1rem;
}

.gradient-inputs input[type="color"] {
    flex: 1;
}

input:focus {
    outline: none;
    border-color: var(--accent-blue);
    box-shadow: 0 0 0 2px rgba(88, 166, 255, 0.2);
}

button {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.75rem;
    padding: 0.75rem 1.5rem;
    border-radius: 8px;
    border: none;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.2s ease;
}

.btn-primary {
    background-color: var(--btn-primary-bg);
    color: white;
    font-size: 1rem;
}

.btn-primary:hover {
    background-color: var(--btn-primary-hover);
    box-shadow: 0 0 10px rgba(63, 185, 80, 0.3);
}

.btn-secondary {
    background-color: var(--btn-secondary-bg);
    color: var(--text-primary);
    margin-top: 0.5rem;
    border: 1px solid var(--border-color);
    font-size: 1rem;
}

.btn-secondary:hover {
    background-color: var(--btn-secondary-hover);
}

/* Result Preview */
.result-preview {
    margin-top: 3rem;
}

.result-preview.hidden {
    display: none;
}

.result {
    text-align: center;
}

.result h2 {
    margin-bottom: 2rem;
    font-size: 1.8rem;
    color: var(--accent-blue);
}

/* Features */
.features {
    margin-top: 4rem;
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    gap: 2rem;
}

.feature {
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1rem;
}

.feature-icon {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    background-color: rgba(88, 166, 255, 0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    color: var(--accent-blue);
    margin-bottom: 1rem;
    transition: transform 0.3s ease;
}

.feature:hover .feature-icon {
    transform: translateY(-5px);
    background-color: rgba(88, 166, 255, 0.2);
}

.feature h3 {
    color: var(--text-primary);
    font-size: 1.2rem;
}

.feature p {
    color: var(--text-secondary);
    font-size: 0.9rem;
}

/* Footer */
footer {
    border-top: 1px solid var(--border-color);
    padding: 2rem;
    text-align: center;
    margin-top: 4rem;
    background-color: var(--bg-darker);
    color: var(--text-secondary);
}

.footer-links {
    display: flex;
    justify-content: center;
    gap: 2rem;
    margin-top: 1rem;
}

.footer-links a {
    color: var(--text-secondary);
    text-decoration: none;
    font-size: 0.9rem;
}

.footer-links a:hover {
    color: var(--accent-blue);
    text-decoration: underline;
}

/* Responsive */
@media (max-width: 768px) {
    header {
        flex-direction: column;
        gap: 1rem;
        padding: 1rem;
    }
    
    nav {
        gap: 1rem;
    }

    .gradient-inputs {
        flex-direction: column;
        gap: 0.5rem;
    }
    
    .button-group {
        flex-direction: column;
    }
}

/* Hidden class */
.hidden {
    display: none;
}


<p align="center">
  <img
    src="https://user-gen-media-assets.s3.amazonaws.com/gemini_images/f1639d33-5d04-4665-b6a3-6afb01158281.png"
    alt="Saikat Das - Aspiring Data Scientist"
    width="1000"
  />
</p>

</p>
 <img align="right" alt="GIF" src="https://media.giphy.com/media/836HiJc7pgzy8iNXCn/giphy.gif" />
<br>
## Welcome to my world <img src="https://github.com/TheDudeThatCode/TheDudeThatCode/blob/master/Assets/Earth.gif" width="24px"><br>- 🔭 I'm currently working on — **Data Science & Machine Learning**.  <br>- 🌱 I'm currently learning — **Deep Learning, NLP, Computer Vision & Full‑Stack Web Development**.  <br>- 🤝 I've recently worked with communities such as **Postman Community and Samarth Community as Graphic Designer**.<br>-Comtributed in Open Source Communities such as HacktoberFest2024 and Social Summer of Code .<br>- 🚀 My GitHub focus — **Building end‑to‑end ML projects, production‑ready APIs, and insightful dashboards**.  <br>- 💬 Ask me about — **Python, ML pipelines, model deployment, and data visualization**.  <br>- ⚡ Words that describe me — **Self‑motivated, Focused, Curious, Hardworking & Detail‑oriented**.  <br><br>---<br>


# 📊 GitHub Stats:
<img src="https://github-readme-streak-stats-eight.vercel.app?user=SaikatDash&theme=radical&hide_border=true" alt="GitHub Streak" />



## 🌐 Socials:
[![Discord](https://img.shields.io/badge/Discord-%237289DA.svg?logo=discord&logoColor=white)](https://discord.gg/641501920644694018) [![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/saikat9714) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/linkedin.com/in/saikat-das-318a6a216) [![X](https://img.shields.io/badge/X-black.svg?logo=X&logoColor=white)](https://x.com/@ProgramerGeek42) [![email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:sd449420@gmail.com) 

# 💻 Tech Stack:
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white) ![Riot Games](https://img.shields.io/badge/riotgames-D32936.svg?style=for-the-badge&logo=riotgames&logoColor=white) ![Epic Games](https://img.shields.io/badge/epicgames-%23313131.svg?style=for-the-badge&logo=epicgames&logoColor=white) ![Steam](https://img.shields.io/badge/steam-%23000000.svg?style=for-the-badge&logo=steam&logoColor=white) ![Xbox](https://img.shields.io/badge/xbox-%23107C10.svg?style=for-the-badge&logo=xbox&logoColor=white) ![Unreal Engine](https://img.shields.io/badge/unrealengine-%23313131.svg?style=for-the-badge&logo=unrealengine&logoColor=white) ![Ubisoft](https://img.shields.io/badge/Ubisoft-%23F5F5F5.svg?style=for-the-badge&logo=Ubisoft&logoColor=black) ![nVIDIA](https://img.shields.io/badge/nVIDIA-%2376B900.svg?style=for-the-badge&logo=nVIDIA&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white) ![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black) ![Meta](https://img.shields.io/badge/Meta-%230467DF.svg?style=for-the-badge&logo=Meta&logoColor=white) ![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white) ![Adobe Creative Cloud](https://img.shields.io/badge/Adobe%20Creative%20Cloud-DA1F26.svg?style=for-the-badge&logo=Adobe%20Creative%20Cloud&logoColor=white)

---
[![](https://visitcount.itsvg.in/api?id=SaikatDash&icon=0&color=0)](https://visitcount.itsvg.in)

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
