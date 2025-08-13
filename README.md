# سنقوم بإنشاء ملف HTML + CSS بسيط مشابه لفكرة موقع meowlyva.com
# مع الخلفية والصورة المصغرة التي رفعها المستخدم والروابط التي قدمها

background_path = "/mnt/data/❀.jfif"
thumbnail_path = "/mnt/data/ChatGPT Image Aug 8, 2025, 04_41_21 PM.png"

html_content = f"""
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nerzom Links</title>
    <style>
        body {{
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background: url('{background_path}') no-repeat center center fixed;
            background-size: cover;
            text-align: center;
            color: white;
        }}
        .container {{
            background-color: rgba(0, 0, 0, 0.5);
            padding: 20px;
            border-radius: 15px;
            display: inline-block;
            margin-top: 50px;
        }}
        img.profile {{
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 3px solid white;
        }}
        h1 {{
            margin: 15px 0;
        }}
        a {{
            display: block;
            margin: 10px auto;
            padding: 10px 20px;
            background-color: #ff4081;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            width: 200px;
            transition: background 0.3s;
        }}
        a:hover {{
            background-color: #e91e63;
        }}
    </style>
</head>
<body>
    <div class="container">
        <img src="{thumbnail_path}" alt="Profile" class="profile">
        <h1>Nerzom</h1>
        <a href="https://discord.gg/qBsdX5BBGt" target="_blank">Discord</a>
        <a href="https://roblox.com/users/8701213333/profile" target="_blank">Roblox</a>
        <a href="https://open.spotify.com/user/31ygsm5fxf2nz5jes3bvyur3fs3m" target="_blank">Spotify</a>
        <a href="https://www.tiktok.com/@_nerzom_" target="_blank">TikTok</a>
        <a href="https://www.youtube.com/@NERZO-u6d" target="_blank">YouTube</a>
    </div>
</body>
</html>
"""

# حفظ الموقع في ملف HTML
html_file_path = "/mnt/data/nerzom_links.html"
with open(html_file_path, "w", encoding="utf-8") as f:
    f.write(html_content)

html_file_path
