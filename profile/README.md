<div align="center">

# ⚡ LogicAI

**La plateforme d'automatisation de workflows, alimentée par l'IA.**

Déployez des instances LogicAI en un clic, générez vos workflows par IA,
collaborez en temps réel — dans le cloud ou en auto-hébergé via Docker.

</div>

---

## 📑 Sommaire

- [Qu'est-ce que LogicAI ?](#-quest-ce-que-logicai-)
- [Architecture](#-architecture)
- [Nos dépôts](#-nos-dépôts)
- [Par où commencer ?](#-par-où-commencer-)
- [Stack technique](#-stack-technique)

---

## 🚀 Qu'est-ce que LogicAI ?

LogicAI est un **SaaS d'automatisation** qui permet de créer, héberger et exécuter
des workflows (intégrations, IA, data, notifications…). Chaque utilisateur obtient
une ou plusieurs **instances** isolées dans des conteneurs Docker, accessibles
depuis le web, le desktop et le mobile.

- 🧩 **Nodes riches** : IA/LLM, HTTP, bases de données, Slack/Discord/Notion/Stripe…
- 🤖 **IA intégrée** : génération de workflows en langage naturel.
- 👥 **Collaboration** : partage d'instances et gestion des accès en temps réel.
- 🐳 **Auto-hébergeable** : l'instance est open-source et tourne à ~90 % en local.
- 🔌 **API + SDK** : automatisez tout depuis votre code.

---

## 🏗 Architecture

```
   web · desktop · mobile
            │
            ▼
   API LogicAI (Express + Prisma + PostgreSQL)
            │  orchestration Docker
            ▼
   Instances LogicAI (conteneurs open-source)
```

---

## 📦 Nos dépôts

| Dépôt | Accès | Description |
|---|---|---|
| [**logicai-instance**](https://github.com/LogicAI-SaaS/logicai-instance) | 🌐 public | Instance LogicAI **open-source**, auto-hébergeable via Docker (`docker run logicai/logicai`). |
| [**sdk**](https://github.com/LogicAI-SaaS/sdk) | 🌐 public | `logicai-sdk` — client **TypeScript** officiel de l'API. |
| **platform** | 🔒 privé | Monorepo de la plateforme SaaS (API, web, desktop, mobile, code partagé). |

---

## 🧭 Par où commencer ?

**Vous voulez héberger votre propre instance ?**
```bash
docker run -d --name logicai -p 5678:3000 logicai/logicai:latest
# → http://localhost:5678
```
👉 [Guide complet](https://github.com/LogicAI-SaaS/logicai-instance)

**Vous voulez automatiser via du code ?**
```bash
npm install logicai-sdk
```
👉 [Documentation du SDK](https://github.com/LogicAI-SaaS/sdk)

---

## 🧰 Stack technique

`Node.js` · `Express` · `Prisma` · `PostgreSQL` · `Docker` · `React` · `Vite` ·
`Tailwind CSS` · `Tauri` · `Expo / React Native` · `TypeScript`

---

<div align="center">

**LogicAI** — l'automatisation pour tout le monde 🚀

</div>
