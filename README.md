<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Полина Страхова — портфолио</title>
<style>html,body{margin:0;background:#fff4ec}</style>
</head>
<body>

<style>
.ps-root{--ink:#241f31;--mute:#6d6680;--coral:#ff6b57;--violet:#6a5cff;--card:rgba(255,255,255,.9);
  position:relative;width:100%;height:100vh;height:100svh;min-height:600px;overflow:hidden;
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;color:var(--ink);
  background:#fff4ec;-webkit-font-smoothing:antialiased;box-sizing:border-box}
.ps-root *{box-sizing:border-box}
.ps-root a{color:var(--violet);text-decoration:none;border-bottom:1px solid rgba(106,92,255,.35)}
.ps-root a:hover{border-bottom-color:var(--violet)}
.ps-root button{font:inherit;color:inherit;cursor:pointer}

/* обои */
.ps-wall{position:absolute;inset:0;overflow:hidden;z-index:0}
.ps-wall i{position:absolute;border-radius:50%;filter:blur(60px);opacity:.85;animation:ps-drift 22s ease-in-out infinite alternate}
.ps-wall i:nth-child(1){width:46vmax;height:46vmax;left:-10vmax;top:-12vmax;background:#ffcdbf}
.ps-wall i:nth-child(2){width:40vmax;height:40vmax;right:-8vmax;top:-6vmax;background:#cdc4ff;animation-duration:28s}
.ps-wall i:nth-child(3){width:44vmax;height:44vmax;right:10vmax;bottom:-22vmax;background:#b9ecff;animation-duration:25s}
.ps-wall i:nth-child(4){width:30vmax;height:30vmax;left:20vmax;bottom:-12vmax;background:#ffe6a8;animation-duration:31s}
@keyframes ps-drift{to{transform:translate(4vmax,3vmax) scale(1.08)}}

/* верхняя панель */
.ps-menubar{position:absolute;left:0;right:0;top:0;height:36px;z-index:50;display:flex;align-items:center;justify-content:space-between;
  padding:0 16px;background:rgba(255,255,255,.55);backdrop-filter:blur(14px);-webkit-backdrop-filter:blur(14px);font-size:13px;font-weight:600}
.ps-brand{display:flex;align-items:center;gap:8px}
.ps-brand b{width:14px;height:14px;border-radius:50%;background:linear-gradient(135deg,var(--coral),var(--violet))}
.ps-right{display:flex;align-items:center;gap:12px;font-weight:500}
.ps-pill{display:inline-flex;align-items:center;gap:6px;background:#e8fff1;color:#13663a;padding:3px 10px;border-radius:99px;font-size:12px;font-weight:600}
.ps-pill:before{content:"";width:7px;height:7px;border-radius:50%;background:#26c46a;box-shadow:0 0 0 0 rgba(38,196,106,.6);animation:ps-pulse 2s infinite}
@keyframes ps-pulse{70%{box-shadow:0 0 0 7px rgba(38,196,106,0)}100%{box-shadow:0 0 0 0 rgba(38,196,106,0)}}

/* иконки рабочего стола */
.ps-desktop{position:absolute;inset:0;z-index:1;padding:56px 18px 96px;display:grid;grid-auto-flow:column;
  grid-template-rows:repeat(4,minmax(0,110px));grid-auto-columns:104px;gap:6px 8px;align-content:start;justify-content:start}
.ps-icon{position:relative;display:flex;flex-direction:column;align-items:center;gap:6px;background:none;border:0;padding:8px 4px;border-radius:12px;
  color:var(--ink);text-align:center;transition:background .15s,transform .15s}
.ps-icon:hover,.ps-icon:focus-visible{background:rgba(255,255,255,.55);outline:none;transform:translateY(-2px)}
.ps-icon svg{width:62px;height:52px;color:var(--c,#ffb85c);filter:drop-shadow(0 6px 8px rgba(36,31,49,.18))}
.ps-icon.ps-file svg{width:46px;height:56px}
.ps-icon span{font-size:12px;line-height:1.2;font-weight:600;text-shadow:0 1px 0 rgba(255,255,255,.7)}
.ps-badge{position:absolute;top:2px;right:12px;font-style:normal;font-size:10px;font-weight:700;color:#fff;background:var(--coral);padding:2px 6px;border-radius:99px}
.ps-badge.soon{background:var(--violet)}

/* стикер */
.ps-note{position:absolute;right:5vw;top:76px;z-index:1;width:250px;padding:20px 20px 22px;background:#fff3a8;transform:rotate(2.5deg);
  box-shadow:0 14px 24px rgba(36,31,49,.16);border-radius:4px 4px 18px 4px;font-size:15px;line-height:1.45}
.ps-note:before{content:"";position:absolute;left:50%;top:-10px;width:70px;height:20px;transform:translateX(-50%) rotate(-3deg);background:rgba(255,255,255,.6)}
.ps-note h2{margin:0 0 6px;font-size:22px;line-height:1.15}
.ps-note p{margin:0 0 10px}
.ps-note small{color:#7a6a14;font-weight:600}

/* окна */
.ps-windows{position:absolute;inset:0;z-index:20;pointer-events:none}
.ps-win{position:absolute;pointer-events:auto;display:flex;flex-direction:column;max-height:calc(100% - 140px);background:var(--card);
  backdrop-filter:blur(18px);-webkit-backdrop-filter:blur(18px);border:1px solid rgba(255,255,255,.9);border-radius:16px;
  box-shadow:0 30px 60px -12px rgba(36,31,49,.3),0 0 0 1px rgba(36,31,49,.06);animation:ps-pop .22s ease-out}
@keyframes ps-pop{from{opacity:0;transform:scale(.94) translateY(8px)}}
.ps-bar{display:flex;align-items:center;gap:10px;padding:11px 14px;cursor:grab;user-select:none;touch-action:none;border-bottom:1px solid rgba(36,31,49,.08)}
.ps-bar:active{cursor:grabbing}
.ps-dots{display:flex;gap:7px}
.ps-dots i,.ps-dots button{width:13px;height:13px;border-radius:50%;border:0;padding:0;background:#ffbd2e;display:block}
.ps-dots button{background:#ff5f57;position:relative}
.ps-dots button:hover:after{content:"×";position:absolute;inset:0;font-size:12px;line-height:13px;font-weight:700;color:#7a1d17}
.ps-dots i:last-child{background:#28c840}
.ps-ttl{flex:1;text-align:center;font-size:13px;font-weight:700;color:var(--mute);margin-right:46px}
.ps-body{padding:20px 22px 24px;overflow:auto;font-size:14.5px;line-height:1.55}
.ps-body h3{margin:0 0 4px;font-size:21px;line-height:1.2}
.ps-body h4{margin:18px 0 8px;font-size:12px;letter-spacing:.08em;text-transform:uppercase;color:var(--mute)}
.ps-body p{margin:0 0 10px}
.ps-body ul{margin:0 0 6px;padding-left:20px}
.ps-body li{margin:0 0 5px}
.ps-lead{color:var(--mute);margin-bottom:14px!important}
.ps-tags{display:flex;flex-wrap:wrap;gap:6px;margin-top:6px}
.ps-tag{background:#fff;border:1px solid rgba(36,31,49,.12);padding:3px 10px;border-radius:99px;font-size:12px;font-weight:600}
.ps-tag.hot{background:var(--coral);border-color:var(--coral);color:#fff}
.ps-nda{margin-top:16px;padding:10px 12px;border-radius:10px;background:#f2efff;color:#4a3fc4;font-size:13px}
.ps-btns{display:flex;flex-wrap:wrap;gap:8px;margin-top:12px}
.ps-btn{display:inline-block;padding:8px 14px;border-radius:10px;background:var(--ink);color:#fff!important;font-weight:600;font-size:13px;border:0!important}
.ps-btn.alt{background:#fff;color:var(--ink)!important;box-shadow:inset 0 0 0 1px rgba(36,31,49,.18)}
.ps-flow{display:flex;flex-wrap:wrap;align-items:center;gap:6px;margin:6px 0 4px;font-size:12.5px;font-weight:600}
.ps-flow span{background:#fff;border:1px solid rgba(36,31,49,.12);padding:6px 10px;border-radius:10px}
.ps-flow span.hot{background:linear-gradient(135deg,#ffe3dc,#e7e2ff);border-color:transparent}
.ps-flow em{font-style:normal;color:var(--mute)}
.ps-kv{display:grid;grid-template-columns:130px 1fr;gap:8px 12px}
.ps-kv dt{color:var(--mute);font-weight:600}
.ps-kv dd{margin:0}
.ps-frames{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin:12px 0}
.ps-frames div{aspect-ratio:9/16;border-radius:12px;background:linear-gradient(160deg,#ffd9cf,#d6ceff 60%,#c4f1ff);display:grid;place-items:center;font-size:26px;color:#fff;text-shadow:0 2px 8px rgba(36,31,49,.3)}

/* терминал */
.ps-win.ps-termwin{background:rgba(26,22,38,.94);border-color:rgba(255,255,255,.12)}
.ps-termwin .ps-bar{border-bottom-color:rgba(255,255,255,.1)}
.ps-termwin .ps-ttl{color:#a9a1c4}
.ps-term{font-family:ui-monospace,SFMono-Regular,Menlo,Consolas,monospace;font-size:13px;color:#e9e4ff}
.ps-term p{margin:0 0 7px}
.ps-term b{color:#ff8a78}
.ps-term u{display:inline-block;min-width:104px;color:#8fe3ff;text-decoration:none}
.ps-term .ok{color:#7dffb0}
.ps-tl{opacity:0;transform:translateY(4px);transition:opacity .25s,transform .25s}
.ps-tl.on{opacity:1;transform:none}
.ps-term .cur{display:inline-block;width:8px;height:15px;background:#e9e4ff;vertical-align:-3px;animation:ps-blink 1s steps(2) infinite}
@keyframes ps-blink{50%{opacity:0}}

/* док */
.ps-dock{position:absolute;left:50%;bottom:14px;transform:translateX(-50%);z-index:40;display:flex;gap:10px;padding:8px 12px;
  background:rgba(255,255,255,.55);backdrop-filter:blur(16px);-webkit-backdrop-filter:blur(16px);border:1px solid rgba(255,255,255,.8);border-radius:22px}
.ps-dock button{position:relative;width:52px;height:52px;border:0;border-radius:14px;background:#fff;font-size:26px;display:grid;place-items:center;
  box-shadow:0 6px 12px rgba(36,31,49,.14);transition:transform .15s}
.ps-dock button:hover,.ps-dock button:focus-visible{transform:translateY(-8px) scale(1.12);outline:none}
.ps-dock button.on:after{content:"";position:absolute;bottom:-7px;left:50%;width:5px;height:5px;margin-left:-2.5px;border-radius:50%;background:var(--ink)}
.ps-dock button[data-tip]:hover:before{content:attr(data-tip);position:absolute;bottom:68px;left:50%;transform:translateX(-50%);white-space:nowrap;
  background:var(--ink);color:#fff;font-size:12px;font-weight:600;padding:4px 9px;border-radius:8px}

/* мобильная версия */
@media (max-width:720px){
  .ps-root{min-height:560px}
  .ps-note{display:none}
  .ps-pill{display:none}
  .ps-desktop{grid-auto-flow:row;grid-template-rows:none;grid-template-columns:repeat(3,1fr);grid-auto-columns:auto;gap:4px;padding:50px 10px 96px}
  .ps-win{left:8px!important;right:8px!important;top:46px!important;width:auto!important;max-height:calc(100% - 140px)}
  .ps-bar{cursor:default}
  .ps-kv{grid-template-columns:1fr}
  .ps-dock{gap:6px;padding:7px 9px}
  .ps-dock button{width:46px;height:46px;font-size:22px}
}
@media (prefers-reduced-motion:reduce){
  .ps-wall i,.ps-pill:before,.ps-win{animation:none}
  .ps-tl{opacity:1;transform:none;transition:none}
}
</style>

<div class="ps-root" id="psRoot">
  <svg width="0" height="0" style="position:absolute" aria-hidden="true">
    <symbol id="ps-folder" viewBox="0 0 96 80">
      <path d="M6 14a8 8 0 0 1 8-8h22l10 10h34a8 8 0 0 1 8 8v8H6z" fill="currentColor" opacity=".6"/>
      <rect x="4" y="26" width="88" height="50" rx="10" fill="currentColor"/>
      <rect x="4" y="26" width="88" height="15" rx="10" fill="#fff" opacity=".28"/>
    </symbol>
    <symbol id="ps-doc" viewBox="0 0 80 96">
      <path d="M8 10a8 8 0 0 1 8-8h32l24 24v60a8 8 0 0 1-8 8H16a8 8 0 0 1-8-8z" fill="#fff"/>
      <path d="M48 2l24 24H56a8 8 0 0 1-8-8z" fill="currentColor" opacity=".55"/>
      <rect x="18" y="44" width="44" height="5" rx="2.5" fill="currentColor"/>
      <rect x="18" y="56" width="44" height="5" rx="2.5" fill="currentColor" opacity=".6"/>
      <rect x="18" y="68" width="28" height="5" rx="2.5" fill="currentColor" opacity=".35"/>
    </symbol>
  </svg>

  <div class="ps-wall" aria-hidden="true"><i></i><i></i><i></i><i></i></div>

  <header class="ps-menubar">
    <div class="ps-brand"><b></b>Полина Страхова</div>
    <div class="ps-right"><span class="ps-pill">открыта к предложениям</span><span id="psClock">--:--</span></div>
  </header>

  <aside class="ps-note" aria-label="Приветствие">
    <h2>Привет, я Полина&nbsp;👋</h2>
    <p>Внедряю ИИ и автоматизацию: LLM, RAG, компьютерное зрение. Верстаю сайты и делаю AI-видео.</p>
    <small>Открой любую папку — внутри мои проекты</small>
  </aside>

  <nav class="ps-desktop" aria-label="Проекты">
    <button class="ps-icon" data-open="main" style="--c:#ff7a66"><svg viewBox="0 0 96 80"><use href="#ps-folder"/></svg><span>Мониторинг оборудования</span><em class="ps-badge">ВКР</em></button>
    <button class="ps-icon" data-open="rag" style="--c:#8f84ff"><svg viewBox="0 0 96 80"><use href="#ps-folder"/></svg><span>RAG-ассистент</span></button>
    <button class="ps-icon" data-open="cv" style="--c:#33c2e8"><svg viewBox="0 0 96 80"><use href="#ps-folder"/></svg><span>Компьютерное зрение</span></button>
    <button class="ps-icon" data-open="app" style="--c:#58cf8d"><svg viewBox="0 0 96 80"><use href="#ps-folder"/></svg><span>Мобильное приложение</span></button>
    <button class="ps-icon" data-open="web" style="--c:#ffb85c"><svg viewBox="0 0 96 80"><use href="#ps-folder"/></svg><span>Веб и Tilda</span></button>
    <button class="ps-icon" data-open="video" style="--c:#ff8ec7"><svg viewBox="0 0 96 80"><use href="#ps-folder"/></svg><span>AI-видео</span><em class="ps-badge soon">скоро</em></button>
    <button class="ps-icon ps-file" data-open="about" style="--c:#6a5cff"><svg viewBox="0 0 80 96"><use href="#ps-doc"/></svg><span>Обо мне.txt</span></button>
    <button class="ps-icon ps-file" data-open="contacts" style="--c:#ff6b57"><svg viewBox="0 0 80 96"><use href="#ps-doc"/></svg><span>Контакты</span></button>
  </nav>

  <div class="ps-windows" id="psWindows"></div>

  <div class="ps-dock" role="toolbar" aria-label="Док">
    <button data-open="about" data-tip="Обо мне" aria-label="Обо мне">📝</button>
    <button data-open="skills" data-tip="Навыки" aria-label="Навыки">⌨️</button>
    <button data-open="pubs" data-tip="Публикации" aria-label="Публикации">📚</button>
    <button data-open="contacts" data-tip="Связаться" aria-label="Связаться">✉️</button>
  </div>

  <!-- ===== СОДЕРЖИМОЕ ОКОН ===== -->

  <template id="ps-t-main" data-title="Мониторинг оборудования" data-w="660">
    <h3>Система мониторинга оборудования</h3>
    <p class="ps-lead">Корпоративная система для энергетической компании. Началась как выпускная работа, сейчас развивается как рабочий проект для реального заказчика.</p>
    <p>Система опрашивает промышленные контроллеры, замечает отклонения и сразу сообщает людям. Всё, от сбора требований до документации, я делаю сама.</p>
    <h4>Как это устроено</h4>
    <div class="ps-flow">
      <span>Контроллеры</span><em>→</em><span>Сбор данных по IP</span><em>→</em><span>Своя БД</span><em>→</em><span class="hot">Фильтры и пороги</span><em>→</em><span>Telegram</span><em>·</em><span>Яндекс Мессенджер</span><em>·</em><span>Веб-кабинет</span>
    </div>
    <h4>Что сделано</h4>
    <ul>
      <li>Собрала требования, спроектировала архитектуру, разработала систему full-stack</li>
      <li>Сбор данных с контроллеров по IP, запись в собственную базу данных</li>
      <li>Фильтрация показаний и уведомления по порогам в Telegram, Яндекс Мессенджер и на веб-платформу</li>
      <li>Веб-кабинет: роли (администратор и обычный пользователь), графики, фильтры, выгрузка отчётов в Excel и Word</li>
      <li>LLM-ассистент по базе знаний компании (RAG) для консультаций сотрудников</li>
      <li>Техническая документация</li>
    </ul>
    <h4>Что делаю сейчас</h4>
    <ul>
      <li>Превращаю решение в универсальное: цель — 1000+ установок, у каждой своя конфигурация регистров и свои пороги</li>
      <li>Перерабатываю схему данных и перехожу на PostgreSQL, пишу загрузку файлов конфигураций</li>
      <li>Готовлю предиктивную аналитику: прогноз неисправностей и времени до техобслуживания</li>
    </ul>
    <div class="ps-tags">
      <span class="ps-tag hot">LLM</span><span class="ps-tag hot">RAG</span><span class="ps-tag">Python</span><span class="ps-tag">Modbus</span>
      <span class="ps-tag">PostgreSQL</span><span class="ps-tag">Telegram API</span><span class="ps-tag">Яндекс Мессенджер API</span><span class="ps-tag">Excel / Word-экспорт</span>
    </div>
    <p class="ps-nda">🔒 Название заказчика и показатели под NDA. Скриншоты и разбор архитектуры покажу на собеседовании.</p>
  </template>

  <template id="ps-t-rag" data-title="RAG-ассистент" data-w="580">
    <h3>Умный поиск по документам</h3>
    <p class="ps-lead">Вопросно-ответная система на LLM и RAG. Результат: выступление на конференции и статья в Proceedings of SPIE.</p>
    <p>В отличие от обычного чат-бота, модель не выдумывает ответы, а находит точные фрагменты в базе знаний, ведёт контекстный диалог и настраивается под компанию.</p>
    <h4>Что я сделала</h4>
    <ul>
      <li>Спроектировала пайплайн индексации документов</li>
      <li>Подключила эмбеддинги Hugging Face для смыслового поиска</li>
      <li>Настроила LlamaIndex для оркестрации запросов к LLM</li>
      <li>Использовала ChromaDB как векторное хранилище, сделала агента с промптами</li>
    </ul>
    <div class="ps-tags"><span class="ps-tag hot">LLM</span><span class="ps-tag hot">RAG</span><span class="ps-tag">Python</span><span class="ps-tag">LlamaIndex</span><span class="ps-tag">ChromaDB</span><span class="ps-tag">HuggingFace</span></div>
    <div class="ps-btns"><a class="ps-btn" href="http://dx.doi.org/10.1117/12.3109759" target="_blank" rel="noopener">Статья в SPIE</a></div>
  </template>

  <template id="ps-t-cv" data-title="Компьютерное зрение" data-w="580">
    <h3>Своя модель детекции на YOLO</h3>
    <p class="ps-lead">Командный проект: от разметки данных до онлайн-подсчёта объектов. Статья в РИНЦ и диплом I степени научной конференции (2025).</p>
    <h4>Что сделано</h4>
    <ul>
      <li>Вручную собрала датасеты: более 1000 изображений, разметка и анализ</li>
      <li>Обучила модели для детекции, классификации и сегментации</li>
      <li>Оценила качество по метрикам mAP, IoU и другим</li>
      <li>Разработала фильтрацию и автоматический подсчёт объектов в режиме онлайн</li>
    </ul>
    <div class="ps-tags"><span class="ps-tag hot">Computer Vision</span><span class="ps-tag">YOLOv5 / v8</span><span class="ps-tag">PyTorch</span><span class="ps-tag">OpenCV</span><span class="ps-tag">Python</span></div>
    <div class="ps-btns"><a class="ps-btn" href="https://www.elibrary.ru/item.asp?id=82747602&pff=1" target="_blank" rel="noopener">Научная статья</a></div>
    <!-- Когда будет ссылка на видео демонстрации, добавьте сюда вторую кнопку: <a class="ps-btn alt" href="ССЫЛКА">Видео работы</a> -->
  </template>

  <template id="ps-t-app" data-title="Мобильное приложение" data-w="540">
    <h3>Приложение для изучения английских слов</h3>
    <p class="ps-lead">Командная разработка Android-приложения: трекер привычек и заучивание слов. MVP.</p>
    <h4>Мой вклад</h4>
    <ul>
      <li>Реализовала интерфейс по макетам Figma, вёрстка экранов и навигация</li>
      <li>Работа с сетевыми запросами и локальным хранилищем</li>
      <li>Кликабельный прототип и собственный дизайн экранов</li>
    </ul>
    <div class="ps-tags"><span class="ps-tag">Kotlin</span><span class="ps-tag">Android Studio</span><span class="ps-tag">Room Database</span><span class="ps-tag">Figma</span></div>
    <div class="ps-btns"><a class="ps-btn" href="https://github.com/ps-strakhova/EnglishLearningApp" target="_blank" rel="noopener">Код на GitHub</a></div>
  </template>

  <template id="ps-t-web" data-title="Веб и Tilda" data-w="560">
    <h3>Сайты: от вёрстки до бэкенда</h3>
    <p class="ps-lead">Адаптивная вёрстка по макетам, Tilda с Zero Block и собственным кодом, REST API и базы данных.</p>
    <h4>Коммерческий проект</h4>
    <p><b>StandupPoint.ru</b> (октябрь 2025): подбор стиля под бренд, анимации и интерактивные блоки в Zero Block и на JS, адаптация под мобильные, запуск.</p>
    <div class="ps-btns" style="margin:0 0 6px"><a class="ps-btn" href="https://standuppoint.ru/" target="_blank" rel="noopener">Открыть сайт</a></div>
    <h4>Что ещё умею</h4>
    <ul>
      <li>Вёрстка из Figma на HTML, CSS и чистом JavaScript</li>
      <li>REST API на Laravel, проектирование БД в MySQL, тестирование в Postman</li>
      <li>Веб-платформа мониторинга с ролями, графиками и выгрузкой отчётов (см. папку проекта)</li>
    </ul>
    <div class="ps-tags"><span class="ps-tag">Tilda</span><span class="ps-tag">HTML / CSS / JS</span><span class="ps-tag">Laravel</span><span class="ps-tag">FastAPI</span><span class="ps-tag">MySQL</span><span class="ps-tag">Figma</span></div>
  </template>

  <!-- <template id="ps-t-video" data-title="AI-видео" data-w="520">
    <h3>AI-видео и генеративный контент</h3>
    <p class="ps-lead">Моё любимое направление. Подборка работ в процессе, скоро выложу сюда лучшие ролики.</p>
    <div class="ps-frames"><div>▶</div><div>▶</div><div>▶</div></div>
    <p>Делаю ролики от идеи и промпта до монтажа. Прошла курс по видеомонтажу (май–июль 2026).</p>
    <div class="ps-tags"><span class="ps-tag">Kling</span><span class="ps-tag">Seedance</span><span class="ps-tag">CapCut</span><span class="ps-tag">Canva</span><span class="ps-tag">Figma</span></div>
  </template> -->

  <template id="ps-t-about" data-title="Обо мне.txt" data-w="580">
    <h3>Полина Страхова</h3>
    <p class="ps-lead">Специалист по внедрению ИИ и автоматизации · Тюмень · удалённо или гибрид</p>
    <p>Проектирую решения на LLM и RAG, учусь в магистратуре по инженерии ИИ, делаю AI-видео и верстаю сайты. Разрабатываю вместе с AI-ассистентами (Claude Code), читаю и рефакторю код, быстро осваиваю новое.</p>
    <dl class="ps-kv">
      <dt>Магистратура</dt><dd>ТюмГУ, прикладная информатика (инженерия ИИ), 2026–2028</dd>
      <dt>Бакалавриат</dt><dd>ТюмГУ, информационные системы и технологии, 2026, средний балл 4,75</dd>
      <dt>Переподготовка</dt><dd>Специалист по анализу данных (432 ч), 2024</dd>
      <dt>Опыт</dt><dd>Разработчик проекта мониторинга оборудования, 2025 — н.в.<br>Программист, ООО «СБУ 89», 12.2025 — 10.2026</dd>
      <dt>Языки</dt><dd>Русский, английский B1–B2</dd>
      <dt>Командировки</dt><dd>Готова (Москва, Санкт-Петербург, Казань)</dd>
    </dl>
  </template>

  <template id="ps-t-skills" data-title="Terminal — навыки" data-w="620" data-class="ps-termwin">
    <div class="ps-term">
      <p class="ps-tl"><b>$</b> whoami</p>
      <p class="ps-tl">Полина Страхова · внедрение ИИ и автоматизации</p>
      <p class="ps-tl"><b>$</b> skills --list</p>
      <p class="ps-tl"><u>AI и LLM</u>LLM · RAG · LlamaIndex · ChromaDB · эмбеддинги · промпт-инжиниринг · AI-агенты</p>
      <p class="ps-tl"><u>Данные и ML</u>Python · SQL · PostgreSQL · SQLite · YOLO · PyTorch · OpenCV</p>
      <p class="ps-tl"><u>Веб</u>HTML · CSS · JS · Tilda · Laravel · FastAPI · MySQL · REST API · Figma</p>
      <p class="ps-tl"><u>Контент</u>Kling · Seedance · CapCut · Canva</p>
      <p class="ps-tl"><u>Инструменты</u>Claude Code · ChatGPT · DeepSeek · Kimi · Notion · Miro · Git</p>
      <p class="ps-tl"><b>$</b> status</p>
      <p class="ps-tl ok">● открыта к предложениям</p>
      <p class="ps-tl"><b>$</b> <span class="cur"></span></p>
    </div>
  </template>

  <template id="ps-t-pubs" data-title="Публикации и награды" data-w="560">
    <h3>Публикации и награды</h3>
    <h4>Статьи</h4>
    <ul>
      <li><b>Proceedings of SPIE</b>: интеллектуальная Q&amp;A-система по корпоративной документации на LLM и RAG, собственная база знаний, эмбеддинги, агент с промптами. <a href="http://dx.doi.org/10.1117/12.3109759" target="_blank" rel="noopener">DOI</a></li>
      <li><b>РИНЦ</b>: компьютерное зрение и обнаружение объектов с YOLO, кастомная модель командой. <a href="https://www.elibrary.ru/item.asp?id=82747602&pff=1" target="_blank" rel="noopener">elibrary.ru</a></li>
    </ul>
    <h4>Награды и обучение</h4>
    <ul>
      <li>Диплом I степени научной конференции, проект по компьютерному зрению, 2025</li>
      <li>Профессиональная переподготовка «Специалист по анализу данных», 432 ч, ТюмГУ, 2024</li>
      <li>Повышение квалификации «Дизайн сайтов и мультимедийных лонгридов», 50 ч, ТюмГУ, 2023</li>
      <li>Курс по видеомонтажу, 2026</li>
    </ul>
  </template>

  <template id="ps-t-contacts" data-title="Контакты" data-w="460">
    <h3>Давайте общаться</h3>
    <p class="ps-lead">Отвечаю быстро. Лучше всего в Telegram.</p>
    <dl class="ps-kv">
      <dt>Telegram</dt><dd><a href="https://t.me/ps_strakhova" target="_blank" rel="noopener">@ps_strakhova</a></dd>
      <dt>Почта</dt><dd><a href="mailto:pstrakhova@gmail.com">pstrakhova@gmail.com</a></dd>
      <dt>WhatsApp</dt><dd><a href="https://wa.me/79222636346" target="_blank" rel="noopener">+7 922 263-63-46</a></dd>
      <dt>GitHub</dt><dd><a href="https://github.com/ps-strakhova" target="_blank" rel="noopener">ps-strakhova</a></dd>
      <dt>Город</dt><dd>Тюмень</dd>
    </dl>
    <div class="ps-btns"><a class="ps-btn" href="https://t.me/ps_strakhova" target="_blank" rel="noopener">Написать в Telegram</a><a class="ps-btn alt" href="mailto:pstrakhova@gmail.com">Написать на почту</a></div>
  </template>
</div>

<script>
(function(){
  var root=document.getElementById('psRoot'); if(!root)return;
  var layer=document.getElementById('psWindows');
  var wins={}, z=20;
  var reduce=window.matchMedia&&matchMedia('(prefers-reduced-motion:reduce)').matches;

  function clock(){
    var d=new Date(), h=('0'+d.getHours()).slice(-2), m=('0'+d.getMinutes()).slice(-2);
    var el=document.getElementById('psClock'); if(el) el.textContent=h+':'+m;
  }
  clock(); setInterval(clock,20000);

  function mark(id,on){
    root.querySelectorAll('.ps-dock [data-open="'+id+'"]').forEach(function(b){b.classList.toggle('on',on)});
  }
  function focusWin(w){ w.style.zIndex=++z; }

  function typeTerm(body){
    var lines=body.querySelectorAll('.ps-tl'), i=0;
    if(reduce){lines.forEach(function(l){l.classList.add('on')});return;}
    (function next(){ if(i>=lines.length)return; lines[i++].classList.add('on'); setTimeout(next,i%3===0?380:240); })();
  }

  function openWin(id){
    if(wins[id]){ focusWin(wins[id]); return; }
    var tpl=document.getElementById('ps-t-'+id); if(!tpl)return;
    var title=tpl.getAttribute('data-title'), width=+tpl.getAttribute('data-w')||540, cls=tpl.getAttribute('data-class')||'';
    var w=document.createElement('section');
    w.className='ps-win '+cls; w.setAttribute('role','dialog'); w.setAttribute('aria-label',title);
    w.innerHTML='<div class="ps-bar"><span class="ps-dots"><button type="button" aria-label="Закрыть"></button><i></i><i></i></span><span class="ps-ttl"></span></div><div class="ps-body"></div>';
    w.querySelector('.ps-ttl').textContent=title;
    var body=w.querySelector('.ps-body'); body.appendChild(tpl.content.cloneNode(true));

    var n=Object.keys(wins).length, rw=root.clientWidth;
    width=Math.min(width,rw-16);
    w.style.width=width+'px';
    w.style.left=Math.max(8,Math.min(rw-width-8, 150+n*30))+'px';
    w.style.top=(58+n*26)+'px';
    layer.appendChild(w); focusWin(w); wins[id]=w; mark(id,true);

    w.addEventListener('pointerdown',function(){focusWin(w)});
    w.querySelector('.ps-dots button').addEventListener('click',function(){ w.remove(); delete wins[id]; mark(id,false); });

    var bar=w.querySelector('.ps-bar'), sx,sy,ox,oy,drag=false;
    bar.addEventListener('pointerdown',function(e){
      if(e.target.closest('button')||window.innerWidth<=720)return;
      drag=true; sx=e.clientX; sy=e.clientY; ox=w.offsetLeft; oy=w.offsetTop; bar.setPointerCapture(e.pointerId);
    });
    bar.addEventListener('pointermove',function(e){
      if(!drag)return;
      var nx=ox+e.clientX-sx, ny=oy+e.clientY-sy;
      w.style.left=Math.max(-width+90,Math.min(root.clientWidth-90,nx))+'px';
      w.style.top=Math.max(40,Math.min(root.clientHeight-80,ny))+'px';
    });
    function end(){drag=false}
    bar.addEventListener('pointerup',end); bar.addEventListener('pointercancel',end);

    if(id==='skills') typeTerm(body);
  }

  root.addEventListener('click',function(e){
    var t=e.target.closest('[data-open]'); if(t) openWin(t.getAttribute('data-open'));
  });
  document.addEventListener('keydown',function(e){
    if(e.key!=='Escape')return;
    var top=null,tz=-1; Object.keys(wins).forEach(function(k){var v=+wins[k].style.zIndex||0; if(v>tz){tz=v;top=k}});
    if(top){ wins[top].remove(); delete wins[top]; mark(top,false); }
  });

  if(window.innerWidth>=900) setTimeout(function(){openWin('about')},500);
})();
</script>

</body>
</html>
