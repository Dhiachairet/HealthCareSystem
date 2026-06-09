# HealthCare System

A clinic management platform built with Symfony 6, digitizing the full patient journey across three portals.

## Portals
- **Patient** — book appointments, view prescriptions and medical history
- **Doctor** — manage assigned patients, issue prescriptions, view appointment schedule
- **Admin** — full system oversight, user and appointment management

## Features
- Online appointment booking and doctor assignment
- Prescription issuance and medical record tracking
- RBAC using Symfony Security Voters — doctors access only their own patients
- EasyAdmin integration for instant CRUD management
- Secure file uploads with VichUploaderBundle
- Version-controlled schema with Doctrine Migrations

## Tech Stack
- **Backend:** PHP, Symfony 6, Doctrine ORM
- **Frontend:** Twig, HTML/CSS
- **Database:** MySQL
- **Admin:** EasyAdmin Bundle

## Getting Started

### Prerequisites
- PHP 8.1+
- Composer
- MySQL
- Symfony CLI

### Setup
1. Clone the repo
```bash
   git clone https://github.com/Dhiachairet/HealthCareSystem.git
```
2. Install dependencies
```bash
   composer install
```
3. Copy and configure environment
```bash
   cp .env .env.local
   # Edit .env.local with your database credentials
```
4. Run migrations
```bash
   php bin/console doctrine:migrations:migrate
```
5. Start the server
```bash
   symfony serve
```
