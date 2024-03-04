---
colorSchema: dark
layout: cover
mdc: true
transition: fade-out
growSeed: 4
title: WSL - a tool for developers
---

<h1 flex="~ col">
<div text-2xl origin-top-left transition duration-500 :class="$clicks <= 2 ? 'scale-150' : 'op50'">
  <span v-click>A Windows tool for (web) developers</span>
  <sup v-click></sup>
</div>
<div mt1 forward:delay-300 v-click>Windows Subsystem for Linux</div>
</h1>

---
growSeed: 5
layout: two-cols
layoutClass: flex items-center
---

<template v-slot:default>

![](/intro.png){.w-70.h-70.ml-10}

</template>
<template v-slot:right>

# Jan Friebe

<div class="leading-10 opacity-80">
Full Stack developer with passion for Frontend staff<br>
JavaScript/TypeScript // Vue // React // CSS // Design<br>
</div>

<div my-10 w-min flex="~ gap-1" items-center justify-center>
  <div i-ri-user-3-line op50 ma text-xl />
  <div><a href="https://jan-friebe.de" target="_blank" class="border-none! font-300">jan.friebe.de</a></div>
  <div i-ri-github-line op50 ma text-xl ml4/>
  <div><a href="https://github.com/friebe" target="_blank" class="border-none! font-300">friebe</a></div>
  <div i-ri-twitter-x-line op50 ma text-xl ml4/>
  <div><a href="https://twitter.com/jan_friebe" target="_blank" class="border-none! font-300">jan_friebe</a></div>
</div>

</template>

---
layout: center
---

<h1 important-text-5xl>What the hell is WSL now ?</h1>

<div text-white:50 text-2xl v-click>
<span text-yellow2 italic v-mark.yellow.underline>Kompatibilitätschicht</span> zum Ausführen von Linux Executables.
</div>

---
layout: fact
grow: bottom
growSeed: 4
---

Windows-Subsystem für Linux (WSL) ist ein Feature von Windows, mit dem eine Linux-Umgebung auf dem Windows-Computer betrieben werden kann, ohne dass ein separater virtueller Computer oder dualer Start erforderlich ist. WSL wurde entwickelt, um Entwicklern, die Windows und Linux gleichzeitig verwenden möchten, eine nahtlose und produktive Erfahrung zu bieten.

<p text-white:50 text-xs italic>https://learn.microsoft.com/de-de/windows/wsl/about</p>

---


---
layout: center
---

![](/wsl-architecture.png){.w-100}

<!-- 
WSL1 beihnaltete eine Kernelschnitstelle die von MS entwickelt wurde,
aber keinen Linux Code für den Linux-Kernel enthielt. Es gab nur von Canonical bereitgestellte Dateien die ausführbar waren -> Fake Linux, aber ressourcen sparsam als eine komplette VM und der direkteste weg um Linux und WIndows zu vereinenen. Ausschließliches CLI Tool

WSL2 Virtualisierungsansatz mittels Hyper-V (Lightweight Uitility VM). Bessere Performance und bessere Systemkompatibilität. Vollständiger Linux Kernel.
GUI App support möglich.
-->

---
layout: center
---

<h1 important-text-5xl>Sounds interesting, how can I use it ?</h1>
<v-clicks>
```console
wsl --install <Distribution Name> # konfiguration der wsl spezifischen Features + installation image
```
</v-clicks>

---
layout: center
---

<h1 important-text-5xl>And why should i use it ?</h1>
<div text-white:50 text-2xl v-click>
<span text-lime font-bold v-mark.highlight.lime.op5.delay200 inline-block p3 mx--2>It depends on your needs. It feels more sexy</span>
</div>

<div v-click delay200="1" origin-top-left rotate-12 i-emojione-monotone:middle-finger w-5em h-5em absolute top-25 right-25></div>

<!--
Wie bei vielen Antworten im Leben heißt die antwort it depends. Und jeder kann für sich entscheiden, ob er es nutzen möchte oder vollkommen mit windows
zufrieden ist.

Ich bin es nämlich nicht!
Vor ca. 4 Jahren bin ich auf WSL1 aufmerksam geworden und fande damals schon eine coole Sache in Linux und somit Kernal näher zu programmieren und 
Windows ein wenig den Rücken zu kehren und die spezifischen MS Probleme abzuschütteln. Ging leider nicht ganz auf - mit WSL kamen andere Probleme -.-

Ich habe Windows vor vielen Jahren entgültig den Rücken gekehrt und bin auf einen Mac umgestiegen, bereue nichts und bin absolut zufrieden mit der Entscheidung. Viele Probleme habe ich nicht mehr. Leider kam Windows bei Eviden zurück und ich erinnerte mich an WSL, was für mich eine Art zufriedenstellender Kompromiss zwischen MS und MacOS ist. Ich kan viele Linux Programme ausführen, vieles geht schneller, ich habe ein cooles Terminal,
Ich kenne mich in der ZSH SHELL aus...

-->