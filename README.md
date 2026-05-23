# Juanchostrap.dev.apk.-1.0-
The newest roblox inyector 
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>JuanchoStrap Mobile</title>
    <style>
        :root {
            --bg: #020617;
            --panel: rgba(15, 23, 42, 0.9);
            --accent: #38bdf8;
            --text: #f8fafc;
        }

        body {
            margin: 0;
            background: linear-gradient(180deg, #0f172a 0%, #020617 100%);
            color: var(--text);
            font-family: 'Segoe UI', sans-serif;
            padding: 20px;
            min-height: 100vh;
        }

        .header { text-align: center; margin-bottom: 25px; }
        .header h1 { color: var(--accent); margin: 0; font-size: 28px; letter-spacing: 2px; }
        .header p { color: #64748b; font-size: 14px; margin-top: 5px; }

        .card {
            background: var(--panel);
            border: 1px solid rgba(56, 189, 248, 0.2);
            border-radius: 40px; /* Bordes extra redondos */
            padding: 25px;
            backdrop-filter: blur(15px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            margin-bottom: 20px;
        }

        .section-title { font-size: 18px; margin-bottom: 15px; display: flex; align-items: center; gap: 10px; }

        .toggle-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
            border-bottom: 1px solid rgba(255,255,255,0.05);
        }

        .switch { width: 50px; height: 25px; background: #1e293b; border-radius: 20px; position: relative; cursor: pointer; }
        .switch.active { background: var(--accent); }
        .switch::after { content: ''; position: absolute; width: 21px; height: 21px; background: white; border-radius: 50%; top: 2px; left: 2px; transition: 0.3s; }
        .switch.active::after { left: 27px; }

        .json-area {
            width: 100%;
            height: 180px;
            background: #000;
            border: 2px solid #334155;
            border-radius: 20px;
            color: var(--accent);
            padding: 15px;
            box-sizing: border-box;
            font-family: monospace;
            font-size: 14px;
            resize: none;
            outline: none;
        }

        .btn-main {
            width: 100%;
            background: linear-gradient(90deg, var(--accent), #6366f1);
            border: none;
            padding: 20px;
            border-radius: 20px;
            color: white;
            font-size: 18px;
            font-weight: bold;
            margin-top: 20px;
            box-shadow: 0 5px 15px rgba(56, 189, 248, 0.3);
        }
    </style>
</head>
<body>

    <div class="header">
        <h1>JUANCHOSTRAP</h1>
        <p>MOBILE INJECTOR V1.0</p>
    </div>

    <div class="card">
        <div class="section-title">⚙️ FFlags Settings</div>
        <div class="toggle-row">
            <span>New Tech Stack</span>
            <div class="switch active" onclick="this.classList.toggle('active')"></div>
        </div>
        <div class="toggle-row">
            <span>Graphics Disable</span>
            <div class="switch" onclick="this.classList.toggle('active')"></div>
        </div>
        <div class="toggle-row">
            <span>Collision Fix</span>
            <div class="switch active" onclick="this.classList.toggle('active')"></div>
        </div>
    </div>

    <div class="card">
        <div class="section-title">📝 JSON Configuration</div>
        <textarea class="json-area">
{
  "FFlagEnableNewTechStack": true,
  "FFlagDebugDisableGraphics": false,
  "FFlagFixCollisionPerformance": true
}
        </textarea>
        <button class="btn-main">INJECT FLAGS</button>
    </div>

</body>
</html>
