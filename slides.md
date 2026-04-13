---
theme: seriph
monaco: true
highlighter: shiki
title: SDD 2026
info: |
  Specs Driven Development with Agentic IDEs in 2026
---

<h1 style="color: #0f172a !important; text-shadow: 0 2px 6px rgba(0,0,0,0.2), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Specs Driven Development with Agentic IDEs in 2026</h1>

<div class="pt-4">
  <span class="text-[#10a0be] text-5xl font-normal tracking-tight" style="-webkit-text-stroke: 0.7px rgba(0,0,0,0.75); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Зміна парадигми: від синтаксису до оркестрації</span>
</div>

<style global>
:root {
  --slidev-theme-primary: #10a0be !important;
  --slidev-theme-background: white !important;
}
html, body, .slidev-layout {
  background-color: white !important;
  background-image: none !important;
}
.slidev-layout h1,
.slidev-layout h2,
.slidev-layout h3,
.slidev-layout h4,
.slidev-layout h5,
.slidev-layout h6 {
  color: #0e8fab !important;
  text-shadow: 0 2px 4px rgba(0,80,120,0.18), 0 1px 1px rgba(0,0,0,0.12) !important;
  -webkit-text-stroke: 0.4px rgba(0, 70, 100, 0.30) !important;
}
.slidev-layout p:not([class*="text-"]),
.slidev-layout > p,
.slidev-layout .default > p {
  color: #1f2937 !important;
  text-shadow: 0 1px 2px rgba(0,0,0,0.12) !important;
}
</style>

<!--
Тут ми розпочнемо розмову про те, як Spec замінює код.
-->

---
layout: default
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Що таке SDD?</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Specs Driven Development — це парадигма програмування, створена для епохи штучного інтелекту.</p>

- <span v-click><b>Зміна парадигми</b>, а не еволюція TDD: фокус зміщується з тестів як специфікації на декларативний опис як первинний артефакт.</span>
- <span v-click>Перехід фокусу з написання тестів на написання чітких бізнес- та технічних правил (<b>Constraints</b>).</span>
- <span v-click>Код — це наслідок. Spec — це причина.</span>

<!--
SDD робить код деталлю імплементації, а специфікацію - головним активом.
-->

---
layout: center
---

<h1 class="text-6xl leading-20" style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">The Spec is the single Source of Truth.</h1>

---
layout: center
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">The Agentic Loop</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Цикл <b>Plan-Action-Verify</b></p>

<div class="grid grid-cols-3 gap-8 mt-12 text-xl font-bold">
  <div v-click class="p-6 bg-dark-800 rounded shadow border-l-4 border-blue-500">
    <div class="text-blue-400 mb-2">1. Plan</div>
    <span class="text-gray-200">Аналіз <i>Spec</i>, створення стратегії</span>
  </div>
  <div v-click class="p-6 bg-dark-800 rounded shadow border-l-4 border-emerald-500">
    <div class="text-emerald-400 mb-2">2. Action</div>
    <span class="text-gray-200">Редагування файлів, виклик інструментів</span>
  </div>
  <div v-click class="p-6 bg-dark-800 rounded shadow border-l-4 border-purple-500">
    <div class="text-purple-400 mb-2">3. Verify</div>
    <span class="text-gray-200">Запуск тестів, перевірка результату</span>
  </div>
</div>

<!--
Agentic IDEs більше не автодоповнюють код. Вони планують зміни, виконують дії в системі і самостійно перевіряють результати.
-->

---
layout: image-right
image: https://images.unsplash.com/photo-1555066931-4365d14bab8c?q=80&w=600&auto=format&fit=crop
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Cursor</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Найкращий щоденний AI-інструмент у знайомому IDE-середовищі.</p>

- <span v-click><b>Composer 2</b>: Дозволяє швидко генерувати багатофайлові зміни.</span>
- <span v-click><b>Rules for AI</b>: Кастомні інструкції, які Cursor інтерпретує як глобальні правила проекту.</span>
- <span v-click><b>Skills</b>: Кастомні інструменти, інтегровані в IDE. Вони дозволяють агенту автоматизувати специфічні рутинні задачі.</span>

---
layout: image-left
image: https://images.unsplash.com/photo-1677442136019-21780ecad995?q=80&w=600&auto=format&fit=crop
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Codex</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Асинхронний хмарний агент для фонового виконання задач (<b>fire-and-forget</b>).</p>

- <span v-click><b>Repository Understanding</b>: Глибоке розуміння репозиторію.</span>
- <span v-click>Отримує задачу → запускає ізольовану VM → повертає готовий Pull Request.</span>
- <span v-click>Масштабна інтеграція з існуючою корпоративною архітектурою.</span>

---
layout: two-cols
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Claude Code</h1>

- <span v-click>Найкраще підходить для <b>CLI-based refactoring</b> та архітектурних змін.</span>
- <span v-click>Фокус на <b>High Reasoning</b> (високому рівні логічного мислення) при виконанні складних задач.</span>
- <span v-click>Ідеально працює як фоновий Terminal Agent.</span>

::right::

<div class="h-full flex items-center p-8 bg-dark-800 rounded-lg m-4">
<pre class="text-green-400 text-sm">
$ claude "refactor src/auth to use new strategy"
&#10003; Analyzed 14 files
&#10003; Planned architectural change
&#10003; Executed file edits
&#10003; Verified TS compilation
</pre>
</div>

---
layout: image-right
image: https://images.unsplash.com/photo-1620712943543-bcc4688e7485?q=80&w=600&auto=format&fit=crop
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Antigravity</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Платформа від Google для <b>BA-to-Dev handoff</b> та кастомних воркфлоу.</p>

- <span v-click><b>Advanced Agentic Workflows</b>: Кастомні багатокрокові пайплайни з контролем виконання на кожному етапі.</span>
- <span v-click><b>Kit Templates</b>: Готові пресети для типових задач — від spec-generation до code review.</span>
- <span v-click>Нативна інтеграція з <b>Google Docs/Sheets</b> — ідеальний інструмент для <b>BA-to-Dev handoff</b>.</span>

---
layout: default
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Порівняння Agentic IDEs</h1>

<div class="mt-6 overflow-x-auto text-lg text-white bg-dark-900 p-6 rounded-lg border border-gray-700">

| Інструмент | Complex Projects | Rapid Prototyping | High Reasoning | BA-to-Dev Handoff |
| :--- | :--- | :--- | :--- | :--- |
| **Cursor** | <span class="text-yellow-400">Good</span> | <span class="text-emerald-400">Excellent</span> | <span class="text-yellow-400">Good</span> | <span class="text-yellow-400">Good</span> |
| **Codex** | <span class="text-yellow-400">Good</span> | <span class="text-yellow-400">Good</span> | <span class="text-yellow-400">Good</span> | <span class="text-yellow-400">Good</span> |
| **Claude Code** | <span class="text-teal-400 font-bold">Best</span> | <span class="text-yellow-400">Good</span> | <span class="text-teal-400 font-bold">Best</span> | <span class="text-yellow-400">Good</span> |
| **Antigravity** | <span class="text-orange-400">Rising Star</span> | <span class="text-yellow-400">Good</span> | <span class="text-yellow-400">Good</span> | <span class="text-yellow-400">Good</span> |

</div>

<div v-click class="mt-4 text-sm text-gray-400 italic">
  * На основі відгуків розробників та бенчмарків SWE-bench Verified (Q1 2026). Найкращий результат залежить від контексту задачі.
</div>

---
layout: center
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Управління Context Window</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Більший контекст ≠ Кращий код</p>

<div v-click class="mt-8 text-xl text-left bg-gray-800 p-8 rounded shadow-lg border-l-4 border-rose-500">
  <p class="text-white">Важливість <b>ізоляції контексту</b> та гранулярності в Specs.</p>
  <p class="mt-4 text-white">Переповнення <i>Context Window</i> веде до галюцинацій та втрати архітектурних обмежень.</p>
</div>

---
layout: two-cols
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Роль розробника у 2026</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Зміна парадигми: від Кодера до AI-Архітектора.</p>

<div class="mt-8 space-y-4">
  <div v-click>Головна навичка — <b>writing precise specs</b>.</div>
  <div v-click>Синтаксис більше не є конкурентною перевагою.</div>
  <div v-click>Розробник виступає <b>рецензентом</b> та оркестратором воркфлоу агентів.</div>
</div>

::right::

<div class="flex justify-center items-center h-full">
  <img src="https://images.unsplash.com/photo-1517694712202-14dd9538aa97?q=80&w=600&auto=format&fit=crop" class="rounded-full shadow-2xl p-4 bg-dark-800 w-64 h-64 object-cover" />
</div>

---
layout: two-cols
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Нова роль BA в SDD</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Від посередника — до <b>Spec Engineer</b>.</p>

<div class="mt-6 space-y-5 text-base">
  <div v-click class="p-4 bg-dark-800 rounded-lg border-l-4 border-gray-500">
    <div class="text-gray-400 font-bold mb-1">Раніше</div>
    <div class="text-gray-300">BA збирає вимоги → передає розробнику → розробник інтерпретує → BA перевіряє результат.</div>
  </div>
  <div v-click class="p-4 bg-dark-800 rounded-lg border-l-4 border-teal-500">
    <div class="text-teal-400 font-bold mb-1">Тепер</div>
    <div class="text-gray-300">BA пише <b>машинозрозумілий Spec-контракт</b> → агент виконує → BA верифікує результат <i>без читання коду</i>.</div>
  </div>
  <div v-click class="p-4 bg-dark-800 rounded-lg border-l-4 border-blue-500">
    <div class="text-blue-400 font-bold mb-1">Нова компетенція</div>
    <div class="text-gray-300">Вміння писати <b>точні, однозначні, верифіковані</b> Specs — це новий core-скіл BA, аналогічний SQL або BPMN.</div>
  </div>
</div>

::right::

<div class="flex flex-col justify-center h-full gap-4 pl-8">
  <div v-click class="text-center p-5 bg-dark-800 rounded-xl border border-gray-600">
    <div class="text-4xl mb-2">📋</div>
    <div class="text-gray-300 text-sm">Spec — це <b>єдиний артефакт</b>, зрозумілий і людині, і агенту</div>
  </div>
  <div v-click class="text-center p-5 bg-dark-800 rounded-xl border border-gray-600">
    <div class="text-4xl mb-2">🔁</div>
    <div class="text-gray-300 text-sm">BA стає першою і останньою ланкою контролю якості в SDD-пайплайні</div>
  </div>
</div>

---
layout: default
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">BA Workflow у SDD-пайплайні</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Від вимоги до верифікації — без написання коду.</p>

<div class="flex items-stretch gap-3 mt-8 flex-wrap">
  <div v-click class="flex-1 min-w-36 p-4 bg-blue-900/30 rounded-xl border border-blue-600 text-center">
    <div class="text-2xl mb-2">1️⃣</div>
    <div class="text-black font-bold text-sm">Збір вимог</div>
    <div class="text-gray-700 text-xs mt-1">Confluence / Notion / Jira</div>
  </div>
  <div class="flex items-center text-gray-500 text-2xl">→</div>
  <div v-click class="flex-1 min-w-36 p-4 bg-teal-900/30 rounded-xl border border-teal-600 text-center">
    <div class="text-2xl mb-2">2️⃣</div>
    <div class="text-black font-bold text-sm">Написання Spec</div>
    <div class="text-gray-700 text-xs mt-1">Context · Rules · Schema · AC · Out of Scope</div>
  </div>
  <div class="flex items-center text-gray-500 text-2xl">→</div>
  <div v-click class="flex-1 min-w-36 p-4 bg-purple-900/30 rounded-xl border border-purple-600 text-center">
    <div class="text-2xl mb-2">3️⃣</div>
    <div class="text-black font-bold text-sm">Dry-run з агентом</div>
    <div class="text-gray-700 text-xs mt-1">Агент переказує план — BA перевіряє розуміння до виконання</div>
  </div>
  <div class="flex items-center text-gray-500 text-2xl">→</div>
  <div v-click class="flex-1 min-w-36 p-4 bg-emerald-900/30 rounded-xl border border-emerald-600 text-center">
    <div class="text-2xl mb-2">4️⃣</div>
    <div class="text-black font-bold text-sm">Верифікація</div>
    <div class="text-gray-700 text-xs mt-1">BA перевіряє результат по Acceptance Criteria — не код</div>
  </div>
</div>

<div v-click class="mt-6 p-4 bg-gray-800 rounded-lg border-l-4 border-yellow-500 text-sm text-gray-300">
  <span class="text-yellow-400 font-bold">Ключовий інсайт для QA: </span>
  Тестування зміщується вліво — QA валідує <b>Spec на ambiguity</b> ще до запуску агента, а не шукає баги у готовому коді.
</div>

---
layout: default
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Анатомія "Perfect Spec"</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Структура ідеального контракту для AI Агента.</p>

```markdown {all|2-3|5-8|10-11|13-14|16-17|all}
# Context
Мета компоненту та його місце в архітектурі системи.

# Rules & Constraints
- Не використовувати сторонні бібліотеки.
- Обов'язкова валідація вхідних даних (Zod).
- Мова: TypeScript strict mode.

# Data Schemas
Структура даних (JSON, SQL Schema), з якими працює агент.

# Acceptance Criteria
- [ ] Всі сценарії покриті unit-тестами.
- [ ] Час відповіді < 200ms при навантаженні 100 rps.

# Out of Scope
Авторизація та логування — поза межами цього Spec.
```

---
layout: default
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Bad Spec vs Good Spec</h1>

<div class="grid grid-cols-2 gap-6 mt-8 text-lg">
  <div class="p-6 bg-red-800 rounded-xl border-2 border-red-400 shadow-xl">
    <div class="text-red-100 font-extrabold text-2xl mb-4" style="-webkit-text-stroke: 0.5px rgba(0,0,0,0.4); text-shadow: 0 2px 4px rgba(0,0,0,0.6);">❌ Bad Spec</div>
    <div class="text-white italic font-medium" style="-webkit-text-stroke: 0.3px rgba(0,0,0,0.3); text-shadow: 0 1px 3px rgba(0,0,0,0.6);">"Зроби сторінку входу"</div>
    <div class="mt-4 text-red-50 text-sm font-medium" style="-webkit-text-stroke: 0.2px rgba(0,0,0,0.2); text-shadow: 0 1px 2px rgba(0,0,0,0.6);">Агент не розуміє обмежень — генерує код на власний розсуд, ігнорує бізнес-правила.</div>
  </div>
  <div class="p-6 bg-emerald-800 rounded-xl border-2 border-emerald-400 shadow-xl">
    <div class="text-emerald-100 font-extrabold text-2xl mb-4" style="-webkit-text-stroke: 0.5px rgba(0,0,0,0.4); text-shadow: 0 2px 4px rgba(0,0,0,0.6);">✅ Good Spec</div>
    <div class="space-y-2 text-white text-sm font-medium" style="-webkit-text-stroke: 0.3px rgba(0,0,0,0.3); text-shadow: 0 1px 3px rgba(0,0,0,0.6);">
      <div>• Формат email: <b class="text-emerald-200">RFC 5322</b></div>
      <div>• Пароль: мінімум <b class="text-emerald-200">8 символів</b>, 1 цифра, 1 спецсимвол</div>
      <div>• Після <b class="text-emerald-200">3 невдалих спроб</b> — captcha (Google reCAPTCHA v3)</div>
      <div>• Час блокування акаунту: <b class="text-emerald-200">5 хвилин</b></div>
      <div>• JWT токен: термін дії <b class="text-emerald-200">15 хвилин</b>, refresh — 7 днів</div>
      <div>• Out of scope: реєстрація, OAuth</div>
    </div>
  </div>
</div>

---
layout: default
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Spec Quality is the new Bottleneck</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8); font-style: italic;">Garbage Spec → Garbage Code. В SDD це критично.</p>

<div class="grid grid-cols-2 gap-6 mt-8">
  <div v-click class="p-5 bg-dark-800 rounded-xl border-l-4 border-rose-500">
    <div class="text-rose-400 font-bold text-lg mb-3">🐛 Як дебажити Spec?</div>
    <div class="space-y-2 text-sm text-gray-300">
      <div>• Запитати агента: <span class="text-white italic">"Що саме ти зрозумів з цього Spec?"</span></div>
      <div>• Порівняти <b>Plan</b>-фазу агента з очікуваним результатом — до написання коду.</div>
      <div>• Використовувати <b>dry-run</b>: агент описує план без виконання.</div>
    </div>
  </div>
  <div v-click class="p-5 bg-dark-800 rounded-xl border-l-4 border-amber-500">
    <div class="text-amber-400 font-bold text-lg mb-3">🔍 Як знайти ambiguity?</div>
    <div class="space-y-2 text-sm text-gray-300">
      <div>• Попросити агента: <span class="text-white italic">"Знайди суперечності та неоднозначності в цьому Spec"</span>.</div>
      <div>• Перевірити: чи є у Spec <b>Acceptance Criteria</b> для кожного правила?</div>
      <div>• Edge cases: що відбувається за межами happy path?</div>
    </div>
  </div>
  <div v-click class="col-span-2 p-5 bg-dark-800 rounded-xl border border-gray-600 text-sm text-gray-300">
    <span class="text-teal-400 font-bold">Висновок: </span>
    У TDD баг у тесті ламає один сценарій. Баг у Spec ламає всю функціональність — і агент впевнено генерує неправильний код.
  </div>
</div>

---
layout: two-cols
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Potential Pitfalls of SDD</h1>

- <span v-click><b>Prompt Sensitivity</b>: Мала зміна в <i>Spec</i> може призвести до кардинально іншого коду.</span>
- <span v-click><b>Hallucinations</b>: Агент може ігнорувати <i>Constraints</i> або придумувати неіснуючі API.</span>
- <span v-click><b>Security</b>: Ризик витоку інтелектуальної власності через <i>Context Window</i> у хмарних IDE.</span>

::right::

<div class="flex justify-center items-center h-full">
  <div class="p-8 bg-red-800 rounded-xl border-2 border-red-400 shadow-xl text-center">
    <div class="text-5xl mb-4">⚠️</div>
    <div class="text-red-100 font-extrabold text-2xl" style="-webkit-text-stroke: 0.5px rgba(0,0,0,0.4); text-shadow: 0 2px 4px rgba(0,0,0,0.6);">Caution Required</div>
    <div class="text-red-50 text-sm font-medium mt-2" style="-webkit-text-stroke: 0.2px rgba(0,0,0,0.2); text-shadow: 0 1px 2px rgba(0,0,0,0.6);">Кожна з цих пасток може звести нанівець результат цілого спринту.</div>
  </div>
</div>

---
layout: two-cols
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Коли SDD — це погана ідея?</h1>

<div class="mt-8 space-y-6">
  <div v-click class="p-4 bg-red-800 rounded-xl border-2 border-red-400 shadow-xl">
    <div class="text-red-100 font-extrabold text-lg" style="-webkit-text-stroke: 0.5px rgba(0,0,0,0.4); text-shadow: 0 2px 4px rgba(0,0,0,0.6);">📦 Малі проєкти</div>
    <div class="text-red-50 text-sm font-medium mt-1" style="-webkit-text-stroke: 0.2px rgba(0,0,0,0.2); text-shadow: 0 1px 2px rgba(0,0,0,0.6);">До ~500 рядків коду — вартість написання Spec перевищує вартість самого коду.</div>
  </div>
  <div v-click class="p-4 bg-red-800 rounded-xl border-2 border-red-400 shadow-xl">
    <div class="text-red-100 font-extrabold text-lg" style="-webkit-text-stroke: 0.5px rgba(0,0,0,0.4); text-shadow: 0 2px 4px rgba(0,0,0,0.6);">🏥 Високочутливі системи</div>
    <div class="text-red-50 text-sm font-medium mt-1" style="-webkit-text-stroke: 0.2px rgba(0,0,0,0.2); text-shadow: 0 1px 2px rgba(0,0,0,0.6);">Medtech, avionics, fintech з регуляторними вимогами — AI-агент не забезпечує аудитного сліду та детермінованості.</div>
  </div>
  <div v-click class="p-4 bg-red-800 rounded-xl border-2 border-red-400 shadow-xl">
    <div class="text-red-100 font-extrabold text-lg" style="-webkit-text-stroke: 0.5px rgba(0,0,0,0.4); text-shadow: 0 2px 4px rgba(0,0,0,0.6);">🧭 Відсутність архітектора</div>
    <div class="text-red-50 text-sm font-medium mt-1" style="-webkit-text-stroke: 0.2px rgba(0,0,0,0.2); text-shadow: 0 1px 2px rgba(0,0,0,0.6);">Без досвідченого архітектора некоректний Spec породжує некоректний код у промислових масштабах.</div>
  </div>
</div>

::right::

<div class="flex justify-center items-center h-full">
  <div class="p-8 bg-gray-800 rounded-xl border border-gray-600 text-center">
    <div class="text-5xl mb-4">🚫</div>
    <div class="text-gray-300 text-lg font-medium">SDD підсилює як<br>правильні рішення,<br>так і помилкові.</div>
  </div>
</div>

---
layout: default
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Cost of Context</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Чому SDD — це дорого, але вигідно?</p>

<div class="grid grid-cols-2 gap-8 mt-10">
  <div v-click class="p-6 bg-gray-800 rounded shadow">
    <h3 class="text-emerald-400 font-bold">Витрати на Токени</h3>
    <p class="mt-2 text-sm text-gray-300">Конвеєр постійно споживає Input/Output токени API.</p>
  </div>
  <div v-click class="p-6 bg-gray-800 rounded shadow">
    <h3 class="text-blue-400 font-bold">Agentic Loop vs Senior Time</h3>
    <p class="mt-2 text-sm text-gray-300">Вартість одного циклу агента значно менша за вартість еквівалентного часу Senior розробника.</p>
  </div>
  <div v-click class="col-span-2 p-6 bg-gray-800 rounded shadow border-l-4 border-yellow-500">
    <h3 class="text-yellow-400 font-bold">ROI</h3>
    <p class="mt-2 text-gray-300 text-lg">Зменшення часу на QA та стабілізація кодової бази — головний фактор окупності інвестицій в Agentic IDEs.</p>
  </div>
</div>

---
layout: image-right
image: https://images.unsplash.com/photo-1522071820081-009f0129c71c?q=80&w=600&auto=format&fit=crop
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Collaborative SDD</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">Як змінюється взаємодія ролей в команді.</p>

- <span v-click><b>Spec стає мостом (Contract)</b>, який розуміють і люди (BA, QA, розробник), і Агенти.</span>
- <span v-click>QA інженери тестують не код, а логіку <i>Spec</i>-контракту.</span>
- <span v-click><b>Git for Specs</b>: Версіонування специфікацій стає таким ж важливим, як і версіонування згенерованого коду.</span>

---
layout: center
---

<h1 style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">The "No-Code" vs "Spec-Code" Boundary</h1>

<p style="font-size: 1.15rem; -webkit-text-stroke: 0.5px rgba(0,0,0,0.9); text-shadow: 0 1px 0 rgba(0,0,0,0.5), 0 0px 1px rgba(0,0,0,0.8);">SDD — це <em>не</em> Low-code.</p>

<div class="mt-12 text-2xl max-w-2xl text-left bg-gray-800 p-8 rounded-xl border-2 border-gray-500 shadow-xl">
  <span class="text-white font-medium" style="-webkit-text-stroke: 0.3px rgba(0,0,0,0.3); text-shadow: 0 1px 3px rgba(0,0,0,0.6);">SDD все ще потребує <span class="text-teal-300 font-bold">глобального розуміння архітектури</span> систем.</span>
  <br><br>
  <span class="text-gray-200 font-medium" style="-webkit-text-stroke: 0.2px rgba(0,0,0,0.2); text-shadow: 0 1px 2px rgba(0,0,0,0.5);">Це радикально інша парадигма: ми відмовляємося від "візуального програмування" на користь</span> <b class="text-white" style="text-shadow: 0 1px 3px rgba(0,0,0,0.6);">декларативного опису логіки</b> <span class="text-gray-200" style="-webkit-text-stroke: 0.2px rgba(0,0,0,0.2);">(Specs).</span>
</div>

---
layout: statement
---

<h1 style="color: #0e8fab !important; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75);">Future Outlook: Autonomous Repositories</h1>

<div class="text-gray-800 font-medium">
  <b>Self-healing code</b>:<br>
  Агенти, що самі виправляють баги на основі оновлених Specs.
  <br><br>
  <span class="text-blue-700">Реалістичний сценарій до кінця 2026: <b>часткова автономність дрібних мікросервісів</b> у командах з розвиненою Spec-культурою.</span>
</div>

---
layout: center
---

<div class="mb-8">
  <h1 class="text-6xl font-bold" style="color: #0e8fab; text-shadow: 0 2px 6px rgba(0,80,120,0.25), 0 1px 2px rgba(0,0,0,0.15); -webkit-text-stroke: 0.7px rgba(0,0,0,0.75); background: none;">Conclusion</h1>
</div>

<div class="text-3xl font-medium italic text-gray-800">
"Кодити вручну — застаріло. Писати Specs — майбутнє."
</div>

<div class="absolute bottom-4 right-4 text-sm text-gray-400">
  Зроблено за допомогою <a href="https://sli.dev/" class="text-teal-400 hover:text-teal-300 underline">sli.dev</a>
</div>
