<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ficha RPG - Sistema Automatizado v5</title>
    <style>
        :root {
            --bg: #0d1117; --card: #161b22; --primary: #58a6ff; --text: #c9d1d9; --accent: #238636; --border: #30363d; --mana: #79c0ff; --danger: #f85149; --gold: #f1e05a;
        }
        body { font-family: 'Segoe UI', sans-serif; background: var(--bg); color: var(--text); margin: 0; padding: 10px; display: flex; justify-content: center; }
        .wrapper { width: 100%; max-width: 950px; background: var(--card); border-radius: 12px; padding: 25px; box-shadow: 0 8px 32px rgba(0,0,0,0.5); border: 1px solid var(--border); }
        
        h2 { text-align: center; color: var(--primary); text-transform: uppercase; letter-spacing: 3px; margin: 10px 0; }
        .section-title { border-left: 4px solid var(--primary); padding-left: 12px; margin: 40px 0 15px; color: var(--primary); font-size: 1.1em; font-weight: bold; text-transform: uppercase; }
        
        .grid-header { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 15px; }
        .field-group { margin-bottom: 15px; }
        label { display: block; font-size: 0.75em; color: #8b949e; margin-bottom: 5px; font-weight: bold; text-transform: uppercase; }
        input, select, textarea { width: 100%; padding: 12px; background: #010409; border: 1px solid var(--border); color: white; border-radius: 6px; box-sizing: border-box; font-size: 1em; }
        
        /* Status Boxes */
        .status-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 15px; margin: 15px 0; }
        .status-box { background: #0d1117; padding: 15px; border-radius: 10px; border: 2px solid var(--border); text-align: center; }
        .val-display { font-size: 1.8em; font-weight: bold; display: block; }

        /* Atributos */
        .attr-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 12px; }
        .attr-box { background: #0d1117; padding: 12px; border-radius: 8px; border: 1px solid var(--border); display: flex; flex-direction: column; align-items: center; }
        .total-val { font-size: 2.2em; font-weight: bold; color: #fff; margin: 5px 0; }
        .attr-controls { display: flex; gap: 20px; align-items: center; }
        .btn-attr { width: 45px; height: 45px; border: none; border-radius: 8px; cursor: pointer; color: white; font-weight: bold; font-size: 1.6em; transition: 0.1s; }

        /* Cards Dinâmicos (Equips e Magias) */
        .card-container { display: flex; flex-direction: column; gap: 15px; }
        .dynamic-card { background: #0d1117; border: 1px solid var(--border); border-radius: 10px; padding: 15px; }
        .card-header { display: grid; grid-template-columns: 2fr 1fr 1fr 1fr 45px; gap: 10px; margin-bottom: 10px; }
        .skill-header { display: grid; grid-template-columns: 1fr 45px; gap: 10px; margin-bottom: 8px; }
        
        /* Textareas Grandes */
        .ta-aparencia { min-height: 150px; }
        .ta-historia { min-height: 400px; line-height: 1.6; }

        .calc-box { display: flex; gap: 8px; }
        .btn-calc { background: var(--primary); color: #000; border: none; padding: 0 20px; border-radius: 6px; cursor: pointer; font-weight: bold; }
        
        .xp-bar-bg { background: #30363d; height: 12px; border-radius: 6px; margin-top: 8px; overflow: hidden; }
        .xp-bar-fill { background: var(--accent); height: 100%; transition: 0.4s; width: 0; }

        .btn-add { background: var(--primary); color: #000; border: none; padding: 12px 25px; border-radius: 6px; cursor: pointer; font-weight: bold; margin: 15px 0; font-size: 0.9em; }
        .btn-del { background: var(--danger); color: white; border: none; border-radius: 6px; cursor: pointer; font-weight: bold; }
    </style>
</head>
<body>

<div class="wrapper">
    <h2>📜 FICHA DE PERSONAGEM</h2>

    <div style="text-align: right; margin-bottom: 15px; display: flex; justify-content: flex-end; gap: 10px;">
        <button onclick="exportarFicha()" style="cursor:pointer; background:#21262d; color:white; border:1px solid #444; padding:10px; border-radius:5px;">📥 SALVAR PERSONAGEM</button>
        <button onclick="document.getElementById('file-input').click()" style="cursor:pointer; background:#21262d; color:white; border:1px solid #444; padding:10px; border-radius:5px;">📤 CARREGAR ARQUIVO</button>
        <input type="file" id="file-input" style="display:none" onchange="importarFicha(event)">
    </div>

    <!-- CABEÇALHO -->
    <div class="grid-header">
        <div class="field-group"><label>NOME</label><input type="text" id="nome" oninput="salvar()"></div>
        <div class="field-group"><label>IDADE</label><input type="text" id="idade" oninput="salvar()"></div>
        <div class="field-group"><label>ALTURA</label><input type="text" id="altura" oninput="salvar()"></div>
    </div>

    <div class="grid-header">
        <div class="field-group">
            <label>RAÇA</label>
            <select id="raca" onchange="salvar()">
                <option value="HUMANO">HUMANO</option>
                <option value="ELFO">ELFO</option>
                <option value="ANÃO">ANÃO</option>
                <option value="SEMI-HUMANO">SEMI-HUMANO</option>
            </select>
        </div>
        <div class="field-group">
            <label>CLASSE</label>
            <select id="classe" onchange="salvar()">
                <option value="Guerreiro">Guerreiro</option>
                <option value="Mago">Mago</option>
                <option value="Arqueiro">Arqueiro</option>
                <option value="Clérigo">Clérigo</option>
                <option value="Necromante">Necromante</option>
                <option value="Bardo">Bardo</option>
                <option value="Assassino">Assassino</option>
                <option value="Paladino">Paladino</option>
                <option value="Bárbaro">Bárbaro</option>
                <option value="Monge">Monge</option>
            </select>
        </div>
        <div class="field-group">
            <label>AFINIDADE</label>
            <select id="afinidade" onchange="salvar()">
                <option value="Água 💧">Água 💧</option><option value="Fogo 🔥">Fogo 🔥</option>
                <option value="Terra 🌋">Terra 🌋</option><option value="Vento 💨">Vento 💨</option>
                <option value="Luz ✨">Luz ✨</option><option value="Trevas 🌑">Trevas 🌑</option>
            </select>
        </div>
    </div>

    <div class="status-grid">
        <div class="status-box" style="border-color: var(--danger);">
            <label>💖 VIDA (ATUAL / MÁX)</label>
            <div style="display:flex; align-items:center; justify-content:center; gap:10px; margin-top:5px;">
                <input type="number" id="vida-atual" value="50" style="width:100px; text-align:center; font-size:2em; border:none; background:transparent; color:white; font-weight:bold;">
                <span class="val-display">/ <span id="vida-max">50</span></span>
            </div>
        </div>
        <div class="status-box" style="border-color: var(--mana);">
            <label>✨ MANA TOTAL</label>
            <span class="val-display" id="mana-display">0</span>
        </div>
        <div class="status-box" style="border-color: var(--gold);">
            <label>💰 OURO TOTAL</label>
            <span class="val-display" id="ouro-total">0</span>
        </div>
    </div>

    <div class="grid-header">
        <div class="field-group">
            <label>💰 CALCULADORA DE OURO</label>
            <div class="calc-box">
                <input type="text" id="ouro-input" placeholder="Ex: +100 ou 1000">
                <button class="btn-calc" onclick="executarCalculo('ouro')">OK</button>
            </div>
        </div>
        <div class="field-group">
            <label>✨ CALCULADORA DE XP</label>
            <div class="calc-box">
                <input type="text" id="xp-input" placeholder="Ex: +500 ou 200">
                <button class="btn-calc" onclick="executarCalculo('xp')">OK</button>
            </div>
        </div>
    </div>
    <div class="xp-bar-bg"><div class="xp-bar-fill" id="xp-fill"></div></div>
    <div style="display:flex; justify-content:space-between; font-size:0.9em; margin-top:8px; margin-bottom: 20px;">
        <span>Nível: <b id="lvl-show" style="color:var(--primary)">1</b> | XP no Nível: <b id="xp-no-lvl">0</b> / <b id="xp-req">500</b></span>
        <span>Total Acumulado: <b id="xp-total-show">0</b></span>
    </div>

    <div class="section-title">📊 ATRIBUTOS (Base + Bônus)</div>
    <div id="pts-painel" style="background:#21262d; padding:15px; border-radius:6px; text-align:center; margin-bottom:15px; border: 1px solid var(--primary);">
        PONTOS BÔNUS DISPONÍVEIS: <strong id="pts-disp" style="color:var(--primary); font-size:1.5em">8</strong>
    </div>
    <div class="attr-grid" id="attr-grid"></div>

    <div class="section-title">⚔️ ARMAS & EQUIPAMENTOS</div>
    <div class="card-container" id="lista-equips"></div>
    <button class="btn-add" onclick="addEquip()">+ ADICIONAR NOVO ITEM</button>

    <div class="section-title">🪄 MAGIAS & HABILIDADES</div>
    <div class="card-container" id="lista-magias"></div>
    <button class="btn-add" onclick="addMagia()">+ ADICIONAR NOVA MAGIA</button>

    <div class="section-title">🎨 APARÊNCIA DO PERSONAGEM</div>
    <textarea id="aparencia" class="ta-aparencia" placeholder="Descreva as características físicas, roupas e acessórios..." oninput="salvar()"></textarea>

    <div class="section-title">📜 HISTÓRIA E ORIGEM</div>
    <textarea id="historia" class="ta-historia" placeholder="Escreva a trajetória, clã, objetivos e passado do seu herói..." oninput="salvar()"></textarea>

    <div class="section-title">🧬 HABILIDADE DE RAÇA</div>
    <textarea id="hab-raca" placeholder="Poderes e traços raciais..." oninput="salvar()"></textarea>

    <button onclick="resetar()" style="background:var(--danger); color:white; border:none; width:100%; padding:20px; border-radius:8px; margin-top:40px; cursor:pointer; font-weight:bold; font-size: 1.1em;">LIMPAR TODA A FICHA</button>
</div>

<script>
    const racas = {
        HUMANO: { FOR: 3, AGI: 3, VIT: 2, INT: 3, DEF: 2, PER: 3, FUR: 2, CAR: 2 },
        ELFO: { FOR: 2, AGI: 3, VIT: 4, INT: 4, DEF: 1, PER: 2, FUR: 2, CAR: 2 },
        ANÃO: { FOR: 4, AGI: 1, VIT: 3, INT: 3, DEF: 4, PER: 2, FUR: 1, CAR: 2 },
        "SEMI-HUMANO": { FOR: 3, AGI: 4, VIT: 2, INT: 1, DEF: 2, PER: 3, FUR: 3, CAR: 2 }
    };

    let bonusAtrib = { FOR: 0, AGI: 0, VIT: 0, INT: 0, DEF: 0, PER: 0, FUR: 0, CAR: 0 };
    let xpTotalGlobal = 0;
    let ouroTotalGlobal = 0;

    function renderAtributos() {
        const grid = document.getElementById('attr-grid');
        const racaAtu = document.getElementById('raca').value;
        const base = racas[racaAtu];
        grid.innerHTML = '';
        Object.keys(base).forEach(a => {
            const total = base[a] + bonusAtrib[a];
            grid.innerHTML += `
                <div class="attr-box">
                    <label style="color:var(--primary); font-size:0.9em">${a}</label>
                    <span class="total-val">${total}</span>
                    <div style="font-size:0.75em; color:#8b949e; margin-bottom:12px;">Base ${base[a]} | Bônus +${bonusAtrib[a]}</div>
                    <div class="attr-controls">
                        <button class="btn-attr" style="background:var(--danger)" onclick="modStat('${a}', -1)">-</button>
                        <button class="btn-attr" style="background:var(--accent)" onclick="modStat('${a}', 1)">+</button>
                    </div>
                </div>`;
        });
        const totalBonus = Object.values(bonusAtrib).reduce((a, b) => a + b, 0);
        document.getElementById('pts-disp').innerText = 8 - totalBonus;
    }

    function modStat(stat, val) {
        const totalBonus = Object.values(bonusAtrib).reduce((a, b) => a + b, 0);
        if (val > 0) {
            if (totalBonus >= 8) return;
            if (bonusAtrib[stat] >= 2) return;
            bonusAtrib[stat]++;
        } else {
            if (bonusAtrib[stat] <= 0) return;
            bonusAtrib[stat]--;
        }
        salvar();
    }

    function executarCalculo(tipo) {
        const campo = document.getElementById(tipo + '-input');
        let raw = campo.value.trim().replace(/\s/g, '');
        if (!raw) return;
        raw = raw.replace(/\b0+(\d+)/g, '$1');
        try {
            let atual = (tipo === 'xp') ? xpTotalGlobal : ouroTotalGlobal;
            let expressao = /^[0-9]/.test(raw) ? (atual + "+" + raw) : (atual + raw);
            let resultado = Function('"use strict";return (' + expressao + ')')();
            if (tipo === 'xp') xpTotalGlobal = Math.max(0, resultado);
            else ouroTotalGlobal = Math.max(0, resultado);
            campo.value = "";
            salvar();
        } catch(e) { alert("Erro no cálculo!"); }
    }

    function addEquip(n="", hp=0, dmg=0, def=0) {
        const container = document.getElementById('lista-equips');
        const div = document.createElement('div');
        div.className = 'dynamic-card';
        div.innerHTML = `
            <div class="card-header">
                <input type="text" value="${n}" placeholder="Nome do Item..." oninput="salvar()">
                <input type="number" value="${hp}" placeholder="+HP" oninput="salvar()" class="eq-hp">
                <input type="number" value="${dmg}" placeholder="+Dmg" oninput="salvar()">
                <input type="number" value="${def}" placeholder="+Def" oninput="salvar()">
                <button class="btn-del" onclick="this.parentElement.parentElement.remove(); salvar()">X</button>
            </div>
        `;
        container.appendChild(div);
        salvar();
    }

    function addMagia(n="", d="") {
        const container = document.getElementById('lista-magias');
        const div = document.createElement('div');
        div.className = 'dynamic-card';
        div.innerHTML = `
            <div class="skill-header">
                <input type="text" value="${n}" placeholder="Nome da Magia/Habilidade..." oninput="salvar()">
                <button class="btn-del" onclick="this.parentElement.parentElement.remove(); salvar()">X</button>
            </div>
            <textarea placeholder="Efeito e detalhes da magia..." oninput="salvar()" style="min-height: 80px;">${d}</textarea>
        `;
        container.appendChild(div);
        salvar();
    }

    function salvar() {
        let nivel = 1, ac = 0;
        while(xpTotalGlobal >= ac + (nivel * 500)) { ac += (nivel * 500); nivel++; }
        
        const racaSel = document.getElementById('raca').value;
        const vitTotal = racas[racaSel].VIT + bonusAtrib.VIT;
        const intTotal = racas[racaSel].INT + bonusAtrib.INT;
        const classeSel = document.getElementById('classe').value;

        let bonusHP = 0;
        document.querySelectorAll('.eq-hp').forEach(i => bonusHP += parseInt(i.value) || 0);
        const vidaMax = (vitTotal * 10) + bonusHP;
        
        const magicClasses = ["Mago", "Clérigo", "Bardo", "Necromante"];
        const mult = magicClasses.includes(classeSel) ? 4 : 2;
        const manaFinal = (mult * nivel) + intTotal;

        const ficha = {
            nome: document.getElementById('nome').value,
            idade: document.getElementById('idade').value,
            vidaAtual: document.getElementById('vida-atual').value,
            altura: document.getElementById('altura').value,
            raca: racaSel, classe: classeSel, afinidade: document.getElementById('afinidade').value,
            aparencia: document.getElementById('aparencia').value,
            historia: document.getElementById('historia').value,
            habRaca: document.getElementById('hab-raca').value,
            xpTotalGlobal, ouroTotalGlobal, bonusAtrib,
            equips: Array.from(document.querySelectorAll('#lista-equips > div')).map(card => {
                const inputs = card.querySelectorAll('input');
                return { n: inputs[0].value, hp: inputs[1].value, dmg: inputs[2].value, def: inputs[3].value };
            }),
            magias: Array.from(document.querySelectorAll('#lista-magias > div')).map(card => {
                return { n: card.querySelector('input').value, d: card.querySelector('textarea').value };
            })
        };

        localStorage.setItem('ficha_amigo_v5', JSON.stringify(ficha));

        document.getElementById('vida-max').innerText = vidaMax;
        document.getElementById('mana-display').innerText = manaFinal;
        document.getElementById('ouro-total').innerText = ouroTotalGlobal;
        document.getElementById('lvl-show').innerText = nivel;
        document.getElementById('xp-no-lvl').innerText = xpTotalGlobal - ac;
        document.getElementById('xp-req').innerText = nivel * 500;
        document.getElementById('xp-total-show').innerText = xpTotalGlobal;
        document.getElementById('xp-fill').style.width = Math.min(((xpTotalGlobal - ac) / (nivel * 500) * 100), 100) + "%";
        renderAtributos();
    }

    function carregar() {
        const salvo = JSON.parse(localStorage.getItem('ficha_amigo_v5'));
        if(!salvo) { renderAtributos(); return; }
        document.getElementById('nome').value = salvo.nome || "";
        document.getElementById('idade').value = salvo.idade || "";
        document.getElementById('vida-atual').value = salvo.vidaAtual || 40;
        document.getElementById('altura').value = salvo.altura || "";
        document.getElementById('raca').value = salvo.raca || "HUMANO";
        document.getElementById('classe').value = salvo.classe || "Guerreiro";
        document.getElementById('afinidade').value = salvo.afinidade || "Água 💧";
        document.getElementById('aparencia').value = salvo.aparencia || "";
        document.getElementById('historia').value = salvo.historia || "";
        document.getElementById('hab-raca').value = salvo.habRaca || "";
        xpTotalGlobal = salvo.xpTotalGlobal || 0;
        ouroTotalGlobal = salvo.ouroTotalGlobal || 0;
        bonusAtrib = salvo.bonusAtrib || bonusAtrib;
        
        document.getElementById('lista-equips').innerHTML = "";
        (salvo.equips || []).forEach(e => addEquip(e.n, e.hp, e.dmg, e.def));
        
        document.getElementById('lista-magias').innerHTML = "";
        (salvo.magias || []).forEach(m => addMagia(m.n, m.d));
        
        salvar();
    }

    function exportarFicha() {
        const blob = new Blob([localStorage.getItem('ficha_amigo_v5')], {type: 'application/json'});
        const a = document.createElement('a');
        a.href = URL.createObjectURL(blob);
        a.download = `ficha_${document.getElementById('nome').value || 'heroi'}.json`;
        a.click();
    }

    function importarFicha(e) {
        const reader = new FileReader();
        reader.onload = ev => { localStorage.setItem('ficha_amigo_v5', ev.target.result); carregar(); };
        reader.readAsText(e.target.files[0]);
    }

    function resetar() { if(confirm("Apagar tudo?")) { localStorage.clear(); location.reload(); } }
    window.onload = carregar;
</script>
</body>
</html>
