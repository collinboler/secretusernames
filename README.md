<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css">
    <title>Cool Username Generator</title>
    <script>
        function copyToClipboard(text, buttonId) {
            navigator.clipboard.writeText(text).then(() => {
                const button = document.getElementById(buttonId);
                button.textContent = 'Copied!';
                button.style.backgroundColor = '#4CAF50'; // Change color to indicate success
                setTimeout(() => {
                    button.style.backgroundColor = '#007BFF'; // Change back to blue
                    if (buttonId === 'copyButton') {
                        button.textContent = 'Invisible'; // Change text back to 'Invisible'
                    } else if (buttonId === 'specialButton') {
                        button.textContent = '   @⃝꙰⃝꙰⃝꙰⃝꙰⃝꙰⃝꙰⃝꙰⃝꙰⃝꙰⃝ '; // Special Button Text
                    } else if (buttonId === 'extraButton') {
                        button.textContent = '𓆉'; // Extra Button Text
                    } else if (buttonId.includes('newButton')) {
                        button.textContent = button.getAttribute('data-text'); // New Button Texts
                    }
                }, 1000); // Revert after 1 second
            });
        }
    </script>
    <style>
        .buttonContainer {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
        }

        .sideBySideButtons {
            display: flex;
            justify-content: center;
            gap: 10px;
        }

        .followButton, .copyButton {
            padding: 8px 16px;
            color: white;
            border: none;
            text-align: center;
            cursor: pointer;
            font-size: medium;
        }

        .fuchsiaButton {
            background-color: fuchsia;
        }

        .tealButton {
            background-color: teal;
        }

        .copyButton {
            background-color: #007BFF; /* Blue */
        }

        .discordButton {
            background-color: #7289d9;
            color: white;
            border: none;
            padding: 10px 15px;
            text-align: center;
            display: inline-block;
            margin: 4px 2px;
            cursor: pointer;
            font-size: medium;
        }

        h2 {
            font-size: 4em;
            font-weight: bold;
            color: inherit;
        }
    </style>
</head>
<body>
    <nav class="container-fluid">
        <ul>
            <li><strong>Cool Username Generator</strong></li>
        </ul>
        <ul>
            <li><a href="https://discord.gg/fzgfJAWhxz" target="_blank" class="discordButton">Join Discord</a></li>
        </ul>
    </nav>
    <main class="container">
        <div class="grid">
            <section>
                <hgroup>
                    <h2>Welcome to the Cool Username Generator</h2>
                </hgroup>
                <p>Use the buttons below to copy the usernames to your clipboard</p>
                <div class="buttonContainer">
                    <div class="sideBySideButtons">
                        <button class="followButton fuchsiaButton" onclick="window.location.href='https://www.tiktok.com/@fuchsiawtf?_t=8k5f1oNU907&_r=1'">Follow @fuchsia wtf on TikTok :)</button>
                        <button class="followButton tealButton" onclick="window.location.href='https://www.tiktok.com/@tealwtf?_t=8k5fC6gDSFa&_r=1'">Follow @tealwtf on TikTok :)</button>
                    </div>
                    <button id="newButton1" class="copyButton" data-text="𓆈" onclick="copyToClipboard('𓆈', 'newButton1')">𓆈</button>
                    <button id="newButton2" class="copyButton" data-text="𓆣" onclick="copyToClipboard('𓆣', 'newButton2')">𓆣</button>
                    <button id="newButton3" class="copyButton" data-text="⋆｡°✩"
