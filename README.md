<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Bible Verse</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; padding: 50px; }
        #verseBox { font-size: 24px; font-weight: bold; margin-top: 20px; }
    </style>
</head>
<body>

    <h1>Welcome! Here’s Your Bible Verse for Today:</h1>
    <div id="verseBox"></div>

    <script>
        const verses = [
            "Philippians 4:13 - I can do all things through Christ who strengthens me.",
            "Jeremiah 29:11 - For I know the plans I have for you, declares the Lord...",
            "Psalm 23:1 - The Lord is my shepherd; I shall not want.",
            "Matthew 6:33 - But seek first the kingdom of God and His righteousness...",
            "Isaiah 40:31 - But those who hope in the Lord will renew their strength...",
        ];

        function getRandomVerse() {
            const randomIndex = Math.floor(Math.random() * verses.length);
            document.getElementById("verseBox").innerText = verses[randomIndex];
        }

        window.onload = getRandomVerse;
    </script>

</body>
</html>
