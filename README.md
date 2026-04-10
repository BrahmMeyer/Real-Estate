<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Agent Marketing Kit — Rod2Reel</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet">
<style>
body { background: #074213; font-family: 'Inter', sans-serif; color: white; text-align: center; padding: 40px 20px; }
.kit-card { max-width: 400px; margin: 0 auto; background: rgba(255,255,255,0.1); padding: 30px; border-radius: 20px; border: 1px solid rgba(255,255,255,0.2); }
.qr-preview { position: relative; background: white; padding: 15px; border-radius: 15px; display: inline-block; margin: 20px 0; }
.qr-preview img { width: 200px; height: 200px; display: block; }
.dl-icon { position: absolute; bottom: -15px; right: -15px; background: #ffffff; color: #0A5C1A; width: 45px; height: 45px; border-radius: 50%; display: flex; align-items: center; justify-content: center; box-shadow: 0 4px 10px rgba(0,0,0,0.3); text-decoration: none; font-size: 20px; border: 2px solid #0A5C1A; }
h1 { font-size: 22px; margin-bottom: 10px; }
p { font-size: 14px; opacity: 0.8; margin-bottom: 20px; }
.btn-preview { display: block; text-decoration: none; color: white; border: 1px solid white; padding: 12px; border-radius: 8px; margin-top: 20px; font-size: 13px; font-weight: 600; }
</style>
</head>
<body>
    <div class="kit-card">
        <h1>PREVIEW PROPERTY LISTING</h1>
        <p>Your cinematic marketing kit is ready.</p>
        <div class="qr-preview">
            <img id="qrImg" src="">
            <a href="" id="qrDl" download="Property_QR.png" class="dl-icon">💾</a>
        </div>
        <p style="font-size:12px;">Tap the icon to save QR to your phone</p>
        <a href="" id="reelLink" class="btn-preview">VIEW LIVE REEL PAGE</a>
    </div>
    <script>
        const p = new URLSearchParams(window.location.search);
        const qrUrl = p.get('logo'); // Adjusting to your current Make.com mapping
        document.getElementById('qrImg').src = qrUrl;
        document.getElementById('qrDl').href = qrUrl;
        document.getElementById('reelLink').href = `reel.html?${p.toString()}`;
    </script>
</body>
</html>
