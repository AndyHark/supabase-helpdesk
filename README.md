# Supabase Helpdesk

A lightweight, hosted helpdesk inspired by Gorgias. Built with Supabase, React, OpenAI, Shopify API, and Gmail IMAP.

## ✨ Features
- Email/password login
- Ticket inbox, AI suggestions, reply + status/tags
- Shopify customer lookup via email
- Gmail integration: auto-ticketing from central inbox
- Deployed via Vercel + Railway (or your choice)

## 🛠 Tech Stack
- Supabase (Auth, DB, RLS)
- React + Tailwind (frontend)
- Node.js + Express or Vercel functions (backend)
- OpenAI (reply suggestions)
- Shopify GraphQL API
- IMAP email parsing (Gmail)

## 🚀 Setup
1. Clone the repo
2. Create a Supabase project
3. Run `sql/schema.sql` in Supabase SQL editor
4. Copy `.env.example` → `.env` and fill in values
5. Run Gmail script locally with Node: `node scripts/poll-gmail.js`
6. Deploy frontend with Vercel
7. Deploy backend with Vercel API or Railway

## 🔒 Security Notes
- Gmail polling requires an App Password
- Use Supabase RLS for user ticket protection
- Use `.env` to protect API keys
