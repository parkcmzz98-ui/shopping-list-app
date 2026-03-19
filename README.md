# Shopping List App

A clean shopping list web app powered by **Supabase** database.

## Features
- Add / Check / Delete items
- Filter: All / Active / Done
- Bulk delete completed items
- Cloud storage via Supabase (data persists across devices)
- Optimistic UI updates with rollback on error

## Database Schema
```sql
CREATE TABLE shopping_items (
  id         TEXT PRIMARY KEY,
  text       TEXT NOT NULL,
  checked    BOOLEAN NOT NULL DEFAULT FALSE,
  created_at TIMESTAMPTZ NOT NULL DEFAULT NOW()
);
```

## Tech Stack
- HTML5 / CSS3 / Vanilla JS
- Supabase (PostgreSQL + REST API)

Made with Claude Code
