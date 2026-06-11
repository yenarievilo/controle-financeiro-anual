# Personal Finance Tracker

A web app for tracking monthly expenses, installments, and net salary calculation.

## Features

- Expense tracking by category
- Installment purchase control
- Net salary calculation 
- Cloud sync via Supabase
- Offline mode with local cache

## Stack

- Vanilla HTML/CSS/JS (no framework)
- Supabase (PostgreSQL + REST API)

## Security

This project uses Supabase's `publishable key` exposed in the frontend —
an intentional pattern explicitly documented by Supabase for client-side
applications.

Data protection is enforced via **Row Level Security (RLS)** at the database
level, with policies that isolate access by `device_id` through a request
header. 
