
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Rebelde Live - Graduados 80K+</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800;900&display=swap" rel="stylesheet" />
  <style>
    :root {
      --primary: #FE2C55;
      --secondary: #25F4EE;
      --green: #00E676;
      --gold: #FFD700;
      --purple: #A855F7;
      --bg-base: #050505;
      --bg-surface: #121212;
      --border-color: rgba(255, 255, 255, 0.1);
      --text-main: #F3F4F6;
      --text-muted: #9CA3AF;
    }

    body {
      background-color: var(--bg-base); 
      color: var(--text-main); 
      font-family: 'Inter', sans-serif;
      margin: 0; 
      padding: 20px 15px 50px 15px; 
      max-width: 600px;
      margin-left: auto;
      margin-right: auto;
      -webkit-font-smoothing: antialiased;
    }

    /* HEADER */
    .header-container { text-align: center; margin-bottom: 25px; }
    h1 {
      color: var(--text-main); font-weight: 900; font-size: 2em; margin: 0 0 5px 0;
      text-transform: uppercase; letter-spacing: -0.5px;
    }
    h1 span { 
      background: linear-gradient(to right, var(--gold), #FFA000);
      -webkit-background-clip: text; -webkit-text-fill-color: transparent; 
    }
    .subtitle { 
      font-size: 0.9em; color: var(--secondary); font-weight: 600;
      text-transform: uppercase; letter-spacing: 2px;
    }

    /* TARJETAS GLOBALES */
    .card {
      background: var(--bg-surface); border: 1px solid var(--border-color);
      border-radius: 12px; padding: 20px; margin-bottom: 20px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
    }

    /* RECORDATORIO IMPORTANTE */
    .important-reminder {
      background: linear-gradient(145deg, rgba(255, 215, 0, 0.08), rgba(255, 215, 0, 0.02));
      border: 1px solid rgba(255, 215, 0, 0.3); border-left: 4px solid var(--gold);
    }
    .reminder-title {
      color: var(--gold); font-weight: 800; font-size: 0.9em; text-transform: uppercase;
      margin-bottom: 8px; display: flex; align-items: center; gap: 5px;
    }
    .reminder-text { font-size: 0.85em; line-height: 1.6; color: #E5E7EB; }
    .reminder-text strong { color: var(--gold); }
    
    .referral-box {
      background: rgba(37, 244, 238, 0.1); border: 1px dashed var(--secondary);
      border-radius: 8px; padding: 12px; margin-top: 15px; font-weight: 600; font-size: 0.9em;
      color: var(--text-main); text-align: center;
    }
    .referral-box span { color: var(--secondary); font-weight: 800; font-size: 1.1em;}

    /* TIPS Y AMOR REBELDE */
    .tips-card {
      background: linear-gradient(135deg, rgba(254, 44, 85, 0.1), rgba(37, 244, 238, 0.05));
      border: 1px solid rgba(254, 44, 85, 0.3); border-radius: 12px; padding: 20px; margin-bottom: 20px;
    }
    .tips-title { color: var(--primary); font-weight: 900; font-size: 1.1em; margin-bottom: 12px; display: flex; align-items: center; gap: 8px;}
    .tip-item { font-size: 0.85em; line-height: 1.5; margin-bottom: 10px; color: #E5E7EB; display: flex; gap: 8px;}
    .tip-item span { color: var(--secondary); }
    
    .motivational-quote {
      font-size: 1.05em; font-weight: 800; color: var(--gold); text-align: center;
      margin: 20px 0 10px 0; font-style: italic; line-height: 1.4;
    }

    .tips-footer { margin-top: 15px; font-size: 0.9em; font-weight: 700; color: var(--text-main); text-align: center; border-top: 1px dashed rgba(255,255,255,0.2); padding-top: 15px;}
    .tips-footer span { color: var(--secondary); font-style: italic;}

    /* TICKET MOTIVACIONAL */
    .motivational-card {
      background: linear-gradient(145deg, rgba(37, 244, 238, 0.08), rgba(0,0,0,0));
      border: 1px solid rgba(37, 244, 238, 0.2);
    }
    .m-greeting { font-size: 1.2em; font-weight: 800; margin-bottom: 5px; }
    .m-greeting span { color: var(--secondary); }
    .m-subtitle { color: var(--text-muted); font-size: 0.85em; margin-bottom: 15px; }
    
    .m-list { margin: 10px 0; padding: 0; list-style: none; display: flex; flex-direction: column; gap: 8px;}
    .m-list li { font-size: 0.9em; display: flex; align-items: center; background: rgba(255,255,255,0.03); padding: 8px 12px; border-radius: 6px; font-weight: 500;}
    
    .m-bonus { 
      background: rgba(0, 230, 118, 0.1); border: 1px solid rgba(0, 230, 118, 0.3); 
      padding: 15px; border-radius: 8px; margin-top: 15px; font-weight: 800; 
      color: var(--green); font-size: 1.2em; text-align: center;
    }
    .m-bonus small { display: block; font-size: 0.65em; font-weight: 500; color: #aaa; margin-top: 5px;}
    
    .m-alert-gold { 
      background: rgba(255, 215, 0, 0.15); padding: 12px; border-radius: 8px; margin-top: 10px; 
      font-size: 0.95em; border: 1px solid var(--gold); font-weight: 800; color: var(--gold); 
      text-align: center; box-shadow: 0 0 20px rgba(255, 215, 0, 0.2); animation: pulse 2s infinite;
    }
    .m-alert-purple { 
      background: rgba(168, 85, 247, 0.15); padding: 12px; border-radius: 8px; margin-top: 10px; 
      font-size: 0.95em; border: 1px solid var(--purple); font-weight: 800; color: var(--purple); 
      text-align: center; box-shadow: 0 0 20px rgba(168, 85, 247, 0.2); animation: pulse 2s infinite;
    }
    @keyframes pulse { 0% { transform: scale(1); } 50% { transform: scale(1.02); } 100% { transform: scale(1); } }

    /* CALENDARIO CONTROLES */
    .controls { display: flex; justify-content: space-between; align-items: center; margin-bottom: 15px; }
    .btn-icon { background-color: var(--bg-surface); color: var(--text-main); border: 1px solid var(--border-color); padding: 8px 15px; border-radius: 8px; cursor: pointer; transition: 0.2s; font-weight: bold;}
    .btn-icon:hover { border-color: var(--secondary); color: var(--secondary);}
    #monthDisplay { font-size: 1em; font-weight: 800; letter-spacing: 0.5px; text-transform: uppercase; }

    /* GRILLA CALENDARIO */
    .grid { display: grid; grid-template-columns: repeat(7, 1fr); gap: 6px; margin-bottom: 10px;}
    .day-name { font-weight: 700; color: var(--text-muted); font-size: 0.75em; text-align: center; text-transform: uppercase;}
    .day { background-color: var(--bg-surface); border: 1px solid var(--border-color); min-height: 65px; border-radius: 8px; padding: 6px; display: flex; flex-direction: column; cursor: pointer; transition: all 0.2s; }
    .day:hover:not(.empty) { border-color: var(--secondary); }
    .day.empty { background-color: transparent; border: none; cursor: default; }
    .date-num { font-size: 0.8em; font-weight: 800; color: var(--text-muted); margin-bottom: auto;}
    .task { font-size: 0.7em; font-weight: 700; text-align: center; line-height: 1.3;}
    .task-h { color: var(--text-main); }
    .task-d { color: var(--primary); }
    .cumplido { border-color: rgba(37, 244, 238, 0.4); background: linear-gradient(180deg, var(--bg-surface), rgba(37, 244, 238, 0.05)); }
    .cumplido .date-num { color: var(--secondary); }
    .invalid-day { border-color: rgba(254, 44, 85, 0.4); opacity: 0.7; }

    /* INGRESO MANUAL */
    .manual-section { border: 1px dashed var(--secondary); }
    .manual-inputs { display: flex; gap: 10px; margin: 15px 0; }
    .m-input-group { flex: 1; display: flex; flex-direction: column; }
    .m-input-group label { font-size: 0.75em; color: var(--text-muted); margin-bottom: 5px; font-weight: 700; text-transform: uppercase;}
    .input-modern { padding: 12px; border-radius: 8px; border: 1px solid var(--border-color); background: var(--bg-base); color: var(--text-main); width: 100%; box-sizing: border-box; text-align: center; font-size: 1em; font-weight: 700; font-family: 'Inter', sans-serif; transition: all 0.3s; }
    .input-modern:focus { outline: none; border-color: var(--secondary); box-shadow: 0 0 0 2px rgba(37,244,238,0.2); }
    .btn-outline { width: 100%; background-color: transparent; color: var(--secondary); border: 1px solid var(--secondary); padding: 14px; border-radius: 8px; font-weight: 700; cursor: pointer; transition: 0.2s; text-transform: uppercase;}
    .btn-outline:hover { background: var(--secondary); color: #000; }

    /* BARRAS DE PROGRESO */
    .dash-title { color: var(--text-main); font-size: 1.1em; margin-bottom: 20px; font-weight: 800; display: flex; align-items: center; gap: 8px; text-transform: uppercase;}
    .dash-title::before { content: ''; display: block; width: 4px; height: 18px; background: var(--primary); border-radius: 2px;}
    .stat-row { margin-bottom: 18px; }
    .stat-header { display: flex; justify-content: space-between; font-size: 0.85em; font-weight: 700; color: var(--text-muted); margin-bottom: 8px;}
    .stat-value { color: var(--text-main); font-weight: 800;}
    .stat-value span { color: var(--secondary); }
    .progress-bar-bg { width: 100%; background-color: #222; border-radius: 20px; height: 12px; overflow: hidden; border: 1px solid #333; }
    .progress-fill { height: 100%; width: 0%; transition: width 1s cubic-bezier(0.4, 0, 0.2, 1); border-radius: 20px; }
    .fill-days { background: linear-gradient(90deg, #25F4EE, #00B4D8); }
    .fill-hours { background: linear-gradient(90deg, #A855F7, #D946EF); }
    .fill-diamonds { background: linear-gradient(90deg, #FE2C55, #FF4B6E); }

    /* FORMULARIO CALIDAD & MODAL */
    .report-section { border-top: 1px solid var(--border-color); padding-top: 25px; margin-top: 10px;}
    .question-box { background: var(--bg-base); padding: 15px; border-radius: 8px; margin-bottom: 12px; border: 1px solid var(--border-color); text-align: center;}
    .radio-group { display: flex; gap: 20px; justify-content: center; margin-top: 10px;}
    .radio-group label { font-size: 0.9em; display: flex; align-items: center; gap: 8px; cursor: pointer; font-weight: 600;}
    .btn-whatsapp { width: 100%; background: linear-gradient(135deg, #25D366, #128C7E); color: white; border: none; padding: 16px; font-size: 1em; border-radius: 8px; margin-top: 10px; font-weight: 800; cursor: pointer; box-shadow: 0 4px 15px rgba(37, 211, 102, 0.2); text-transform: uppercase; }

    #modalOverlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.9); display: none; justify-content: center; align-items: center; z-index: 1000; }
    .modal-content { background: var(--bg-surface); padding: 25px; border-radius: 12px; border: 1px solid var(--border-color); width: 90%; max-width: 320px; }
    .btn-primary { width: 100%; background: var(--secondary); color: #000; padding: 12px; border: none; border-radius: 8px; font-weight: 800; cursor: pointer;}
  </style>
</head>
<body>

  <div class="header-container">
    <h1>Rebelde <span>Graduados</span></h1>
    <div class="subtitle">Tracker Élite (80K+ Diamantes)</div>
  </div>

  <div class="card important-reminder">
    <div class="reminder-title">⚠️ REGLAS EXCLUSIVAS DESDE 80K</div>
    <div class="reminder-text">
      Esta herramienta calcula tus bonos proporcionales <strong>únicamente a partir de los 80,000 diamantes</strong>. Al llegar a 80K (con 22 días y 90 hrs) aseguras <strong>$55 USD</strong>, y si es tu primera vez, ganas el <strong>Aro Pro</strong>. Además, ¡si llegas a 150K por primera vez te llevas una <strong>Silla Gamer</strong>!
    </div>
    <div class="referral-box">
      🤝 REFIERE Y GANA:<br>
      Si traes un streamer y es aprobado por la agencia, te llevas <span>$200.000 COP</span> de inmediato.
    </div>
  </div>

  <div class="tips-card">
    <div class="tips-title">💡 Tips de Crecimiento Rebelde</div>
    <div class="tip-item"><span>✦</span> <strong>Conecta desde el corazón:</strong> Tus seguidores son tu familia virtual. Saluda a cada persona por su nombre, hazlos sentir en casa.</div>
    <div class="tip-item"><span>✦</span> <strong>La constancia es tu mejor talento:</strong> Cumplir tus horarios sagradamente hace que tu audiencia sepa siempre cuándo encontrarte.</div>
    <div class="tip-item"><span>✦</span> <strong>Agradece siempre:</strong> Cada diamante representa cariño y esfuerzo de quien te lo envía. Un "gracias" sincero vale oro.</div>
    
    <div class="motivational-quote">
      "Ya demostraste de qué estás hecho(a). Superar los 80K no es suerte, es constancia y talento. ¡Ahora es el momento de romper tus propios límites! Vamos por más."
    </div>

    <div class="tips-footer">
      Recuerda que estamos aquí para verte brillar y acompañarte en cada paso de tu crecimiento.<br><br>
      <span>Att: Team Rebelde - 3 años creando sueños ✨</span>
    </div>
  </div>

  <div id="motivationalCard" class="card motivational-card"></div>

  <!-- CALENDARIO -->
  <div class="controls">
    <button id="prevBtn" class="btn-icon">&lt;</button>
    <div id="monthDisplay"></div>
    <button id="nextBtn" class="btn-icon">&gt;</button>
  </div>
  <div class="grid" id="calendarDays"></div>

  <!-- INGRESO MANUAL -->
  <div class="card manual-section">
    <div class="dash-title" style="font-size: 0.9em; margin-bottom: 5px; color: var(--secondary);">⚡ Carga Rápida (Fin de Mes)</div>
    <p style="font-size: 0.75em; color: var(--text-muted); margin: 0 0 10px 0;">Ingresa tus métricas totales si usaste el filtro de 15 días de TikTok:</p>
    <div class="manual-inputs">
      <div class="m-input-group"><label>Días:</label><input type="number" id="manualDays" class="input-modern" placeholder="0" min="0" /></div>
      <div class="m-input-group"><label>Horas:</label><input type="number" id="manualHours" class="input-modern" placeholder="0" min="0" step="0.1" /></div>
      <div class="m-input-group"><label>Diamantes:</label><input type="number" id="manualDiamonds" class="input-modern" placeholder="0" min="0" /></div>
    </div>
    <button class="btn-outline" onclick="applyManualStats()">Calcular Dinero Exacto</button>
  </div>

  <!-- DASHBOARD -->
  <div class="card dashboard">
    <div class="dash-title">Métricas de Rendimiento</div>
    
    <div class="stat-row">
      <div class="stat-header"><span>Días Válidos (Meta: 22)</span><span class="stat-value" id="statDays">0</span></div>
      <div class="progress-bar-bg"><div class="progress-fill fill-days" id="barDays"></div></div>
    </div>
    
    <div class="stat-row">
      <div class="stat-header"><span>Horas Live (Meta: 90)</span><span class="stat-value" id="statHours">0</span></div>
      <div class="progress-bar-bg"><div class="progress-fill fill-hours" id="barHours"></div></div>
    </div>

    <div class="stat-row" style="margin-bottom: 0;">
      <div class="stat-header"><span>Diamantes (Mín 80k - Max 1M)</span><span class="stat-value" id="statDiamonds">0</span></div>
      <div class="progress-bar-bg"><div class="progress-fill fill-diamonds" id="barDiamonds"></div></div>
    </div>
    
    <div class="report-section">
      <div class="dash-title" style="justify-content: center; font-size: 0.9em; margin-bottom: 15px;">Check Final de Calidad</div>
      <div class="question-box">
        <div style="font-weight: 700; font-size: 0.85em; margin-bottom: 10px;">¿Infracciones o Lives estáticos este mes?</div>
        <div class="radio-group">
          <label><input type="radio" name="sanciones" value="Sí" /> Sí (Invalida bono)</label>
          <label><input type="radio" name="sanciones" value="No" checked /> No (Todo Limpio)</label>
        </div>
      </div>
      <input type="text" id="creatorName" class="input-modern" style="margin: 10px 0;" placeholder="Firma: Nombre/Usuario TikTok" onkeyup="updateName()" />
      <button class="btn-whatsapp" onclick="sendWhatsApp()">Enviar Reporte Oficial</button>
    </div>
  </div>

  <!-- MODAL DE REGISTRO DÍA -->
  <div id="modalOverlay">
    <div class="modal-content">
      <h3 id="modalDateTitle" style="margin:0 0 10px 0;">Día X</h3>
      <div style="font-size: 0.75em; color: var(--primary); margin-bottom: 15px;">Mínimo 60 min de corrido.</div>
      <label style="font-size: 0.8em; font-weight: bold;">Horas de hoy:</label>
      <input type="number" id="inputHours" class="input-modern" style="margin-bottom: 10px;" placeholder="Ej. 2.5" min="0" step="0.1" />
      <label style="font-size: 0.8em; font-weight: bold;">Diamantes hoy:</label>
      <input type="number" id="inputDiamonds" class="input-modern" style="margin-bottom: 15px;" placeholder="Ej. 5000" min="0" />
      <input type="hidden" id="editingDateKey" />
      <div style="display: flex; gap: 10px;">
        <button class="btn-outline" style="border-color: #444; color: #888;" onclick="closeModal()">Cancelar</button>
        <button class="btn-primary" onclick="saveDay()">Guardar</button>
      </div>
    </div>
  </div>

  <script>
    const monthNames = ["Enero", "Febrero", "Marzo", "Abril", "Mayo", "Junio", "Julio", "Agosto", "Septiembre", "Octubre", "Noviembre", "Diciembre"];
    let currentDate = new Date(); 
    let globalStats = { validDays: 0, hours: 0, diamonds: 0, pocketMoney: 0.00, aroUnlocked: false, sillaUnlocked: false, today: new Date().getDate() };
    let userName = localStorage.getItem('rebelde_creator_name') || 'Creador(a)';

    window.onload = () => {
      if (userName !== 'Creador(a)') document.getElementById('creatorName').value = userName;
      renderCalendar();
    };

    function updateName() {
      userName = document.getElementById('creatorName').value || 'Creador(a)';
      localStorage.setItem('rebelde_creator_name', userName);
      updateMotivationalCard();
    }

    // FÓRMULA MATEMÁTICA ESTRICTA (GRADUADOS 80K+)
    function computeMonetization(tDays, tHours, tDiamonds) {
      let isAroUnlocked = false;
      let isSillaUnlocked = false;
      let finalBonus = 0;

      // SOLO SE CALCULA SI TIENEN 80,000 DIAMANTES O MÁS
      if (tDiamonds >= 80000) {
        
        let dCap = Math.min(tDiamonds, 1000000); 
        let daysFactor = Math.min(tDays / 22, 1.0); 
        let hoursFactor = Math.min(tHours / 90, 1.0);
        
        // Fórmula: Inicia en $55 USD a los 80K, y sube hasta $200 USD al llegar al Millón.
        let diamondBonus = 55.00 + ((dCap - 80000) / 920000) * 145.00;

        // Castigo si faltan días u horas (multiplica hacia abajo)
        finalBonus = diamondBonus * daysFactor * hoursFactor;

        // Desbloqueo oficial del Aro Pro (Requiere cumplir TODO el mínimo)
        if (tDays >= 22 && tHours >= 90) {
          isAroUnlocked = true;
        }

        // Desbloqueo de la Silla Gamer (150K)
        if (tDiamonds >= 150000 && tDays >= 22 && tHours >= 90) {
          isSillaUnlocked = true;
        }
      }

      return { pocketMoney: finalBonus, aroUnlocked: isAroUnlocked, sillaUnlocked: isSillaUnlocked };
    }

    function renderCalendar() {
      const year = currentDate.getFullYear();
      const month = currentDate.getMonth();
      document.getElementById('monthDisplay').innerText = `${monthNames[month]} ${year}`;

      const firstDayIndex = new Date(year, month, 1).getDay();
      const startDay = firstDayIndex === 0 ? 6 : firstDayIndex - 1; 
      const daysInMonth = new Date(year, month + 1, 0).getDate();

      const calendarDays = document.getElementById('calendarDays');
      calendarDays.innerHTML = `<div class="day-name">Lun</div><div class="day-name">Mar</div><div class="day-name">Mié</div><div class="day-name">Jue</div><div class="day-name">Vie</div><div class="day-name">Sáb</div><div class="day-name">Dom</div>`;

      let savedData = JSON.parse(localStorage.getItem('rebelde_data')) || {};

      for (let i = 0; i < startDay; i++) { calendarDays.innerHTML += '<div class="day empty"></div>'; }

      for (let i = 1; i <= daysInMonth; i++) {
        const dateKey = `${year}-${month + 1}-${i}`;
        const dayData = savedData[dateKey] || { hours: 0, diamonds: 0 };
        
        let displayHtml = ''; let classes = 'day';
        if (dayData.hours > 0 || dayData.diamonds > 0) {
          displayHtml = `<span class="task-h">${dayData.hours}h</span><br><span class="task-d">${dayData.diamonds >= 1000 ? (dayData.diamonds/1000).toFixed(1)+'k' : dayData.diamonds}</span>`;
          if (dayData.hours >= 1) classes += ' cumplido'; else classes += ' invalid-day'; 
        }

        calendarDays.innerHTML += `<div class="${classes}" onclick="openModal('${dateKey}', ${i}, ${dayData.hours}, ${dayData.diamonds})"><span class="date-num">${i}</span><span class="task">${displayHtml}</span></div>`;
      }
      calculateStats(year, month + 1, daysInMonth);
    }

    function calculateStats(year, month, daysInMonth) {
      let savedData = JSON.parse(localStorage.getItem('rebelde_data')) || {};
      let tHours = 0, tDiamonds = 0, tDays = 0;

      for (let i = 1; i <= daysInMonth; i++) {
        const key = `${year}-${month}-${i}`;
        if (savedData[key]) {
          tHours += savedData[key].hours;
          tDiamonds += savedData[key].diamonds;
          if (savedData[key].hours >= 1) tDays++;
        }
      }

      let mon = computeMonetization(tDays, tHours, tDiamonds);
      globalStats = { validDays: tDays, hours: tHours, diamonds: tDiamonds, pocketMoney: mon.pocketMoney, aroUnlocked: mon.aroUnlocked, sillaUnlocked: mon.sillaUnlocked, today: (year === new Date().getFullYear() && month === new Date().getMonth() + 1) ? new Date().getDate() : daysInMonth };
      updateUI();
    }

    function applyManualStats() {
      const tDays = parseInt(document.getElementById('manualDays').value) || 0;
      const tHours = parseFloat(document.getElementById('manualHours').value) || 0;
      const tDiamonds = parseInt(document.getElementById('manualDiamonds').value) || 0;

      if (tDays === 0 && tHours === 0 && tDiamonds === 0) { alert("Agrega al menos una métrica para calcular."); return; }

      let mon = computeMonetization(tDays, tHours, tDiamonds);
      globalStats = { validDays: tDays, hours: tHours, diamonds: tDiamonds, pocketMoney: mon.pocketMoney, aroUnlocked: mon.aroUnlocked, sillaUnlocked: mon.sillaUnlocked, today: new Date().getDate() };
      
      updateUI();
      document.querySelector('.dashboard').scrollIntoView({ behavior: 'smooth' });
    }

    function updateUI() {
      let dDisplay = globalStats.diamonds >= 1000 ? (globalStats.diamonds/1000).toFixed(1) + 'k' : globalStats.diamonds;
      
      document.getElementById('statDays').innerHTML = `<span>${globalStats.validDays}</span> / 22`;
      document.getElementById('statHours').innerHTML = `<span>${globalStats.hours.toFixed(1)}</span> / 90`;
      document.getElementById('statDiamonds').innerHTML = `<span>${dDisplay}</span> / 1M`;

      setTimeout(() => {
        document.getElementById('barDays').style.width = `${Math.min((globalStats.validDays / 22) * 100, 100)}%`;
        document.getElementById('barHours').style.width = `${Math.min((globalStats.hours / 90) * 100, 100)}%`;
        
        // Bar starts visually loading after 80k to reflect exclusivity
        let dPercent = globalStats.diamonds < 80000 ? 0 : Math.min((globalStats.diamonds / 1000000) * 100, 100);
        document.getElementById('barDiamonds').style.width = `${dPercent}%`;
      }, 50);

      updateMotivationalCard();
    }

    function updateMotivationalCard() {
      const card = document.getElementById('motivationalCard');
      let currentDDisp = globalStats.diamonds >= 1000 ? (globalStats.diamonds/1000).toFixed(1) + 'k' : globalStats.diamonds;

      let aroHtml = globalStats.aroUnlocked 
        ? `<div class="m-alert-gold">🌟 ¡ARO PRO DESBLOQUEADO!<br><span style="font-size:0.8em; font-weight:500; color:#eee;">Meta base de 80K superada exitosamente. (Aplica por 1ra vez)</span></div>` 
        : '';
        
      let sillaHtml = globalStats.sillaUnlocked 
        ? `<div class="m-alert-purple">🎮 ¡SILLA GAMER DESBLOQUEADA!<br><span style="font-size:0.8em; font-weight:500; color:#eee;">Lograste los 150.000 diamantes. (Aplica por 1ra vez)</span></div>` 
        : '';
        
      let missingMsg = (globalStats.diamonds < 80000) 
        ? `<small style="color:var(--primary); font-size:0.7em; display:block; margin-top:5px;">⚠️ Necesitas alcanzar mínimo 80,000 diamantes para activar este bono.</small>` 
        : `<small>(Calculado proporcionalmente según reglas de topes)</small>`;

      card.innerHTML = `
        <div class="m-greeting">Hola, <span>${userName}</span></div>
        <div class="m-subtitle">Reporte de progreso (Día ${globalStats.today} del ciclo)</div>
        
        <ul class="m-list">
          <li>Días Válidos: <span style="margin-left:auto; color:var(--secondary);">${globalStats.validDays}/22</span></li>
          <li>Horas Totales: <span style="margin-left:auto; color:var(--secondary);">${globalStats.hours.toFixed(1)}/90</span></li>
          <li>Diamantes: <span style="margin-left:auto; color:var(--primary);">${currentDDisp}</span></li>
        </ul>

        <div class="m-bonus">
          BONO A PAGAR: $${globalStats.pocketMoney.toFixed(2)} USD
          ${missingMsg}
        </div>
        ${aroHtml}
        ${sillaHtml}
      `;
    }

    function openModal(dateKey, dayNum, currentHours, currentDiamonds) {
      document.getElementById('modalDateTitle').innerText = `Día ${dayNum}`;
      document.getElementById('inputHours').value = currentHours || '';
      document.getElementById('inputDiamonds').value = currentDiamonds || '';
      document.getElementById('editingDateKey').value = dateKey;
      document.getElementById('modalOverlay').style.display = 'flex';
    }

    function closeModal() { document.getElementById('modalOverlay').style.display = 'none'; }

    function saveDay() {
      const dateKey = document.getElementById('editingDateKey').value;
      const hours = parseFloat(document.getElementById('inputHours').value) || 0;
      const diamonds = parseInt(document.getElementById('inputDiamonds').value) || 0;

      let savedData = JSON.parse(localStorage.getItem('rebelde_data')) || {};
      savedData[dateKey] = { hours: hours, diamonds: diamonds };
      
      localStorage.setItem('rebelde_data', JSON.stringify(savedData));
      closeModal();
      document.getElementById('manualDays').value = ''; document.getElementById('manualHours').value = ''; document.getElementById('manualDiamonds').value = '';
      renderCalendar();
    }

    function sendWhatsApp() {
      if (userName === 'Creador(a)' || !userName.trim()) { alert("Ingresa tu Nombre en la firma oficial antes de enviar."); return; }
      
      const sanciones = document.querySelector('input[name="sanciones"]:checked').value;
      const mes = document.getElementById('monthDisplay').innerText;
      const miNumero = "573114835387"; 
      
      let premioExtra = "";
      if (globalStats.aroUnlocked) premioExtra += "%0A🎁 *Premio Físico:* ¡Aro Pro Ganado (1ra vez)! 🌟";
      if (globalStats.sillaUnlocked) premioExtra += "%0A🎁 *Premio Físico:* ¡Silla Gamer Ganada (1ra vez)! 🎮";
      
      // Si el creador marca que SÍ tuvo sanciones, el sistema lo informa y anula el pago en el texto
      let finalUSD = sanciones === "Sí" ? 0.00 : globalStats.pocketMoney;
      let avisoSancion = sanciones === "Sí" ? "%0A❌ _BONO INVALIDADO POR SANCIONES DE TIKTOK_" : "";

      const text = `🎓 *REPORTE CREADORES GRADUADOS* 🎓%0A`
        + `Creador(a): *${userName}*%0A`
        + `Ciclo: ${mes}%0A%0A`
        + `📊 *MÉTRICAS OFICIALES:*%0A`
        + `├ Días: ${globalStats.validDays} (Meta 22)%0A`
        + `├ Horas: ${globalStats.hours.toFixed(1)} (Meta 90)%0A`
        + `└ Diamantes: ${globalStats.diamonds.toLocaleString('en-US')}%0A%0A`
        + `💰 *BONO CALCULADO:* *$${finalUSD.toFixed(2)} USD*`
        + avisoSancion
        + premioExtra
        + `%0A%0A🛑 *CONTROL DE CALIDAD:*%0A`
        + `└ ¿Infracciones/Lives estáticos?: ${sanciones}%0A%0A`
        + `_Enviado para auditoría y pago en Rebelde Live._%0A`
        + `_Att: Team Rebelde - 3 años creando sueños_ ✨`;
      
      window.open(`https://wa.me/${miNumero}?text=${text}`, '_blank');
    }

    document.getElementById('prevBtn').addEventListener('click', () => { currentDate.setMonth(currentDate.getMonth() - 1); renderCalendar(); });
    document.getElementById('nextBtn').addEventListener('click', () => { currentDate.setMonth(currentDate.getMonth() + 1); renderCalendar(); });
  </script>
</body>
</html>
