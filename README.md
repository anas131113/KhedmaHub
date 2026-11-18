# KhedmaHub

A job and internship platform for Tunisia, built with Symfony.
Companies publish offers, students apply with their CV, and admins manage everything from a dashboard.

## Features
**Client side**
- Sign up, log in, edit profile
- Browse and filter offers (keyword, type, category, city)
- Apply with a CV upload and follow application status
- Save favorite offers

**Admin dashboard**
- Manage companies, categories, skills and job offers (with logo upload)
- Review applications and interviews
- Manage users
- Statistics and charts

## Tech stack
Symfony, PHP, Doctrine ORM, Twig, MySQL, Bootstrap

## Team
| Name | Part |
|---|---|
| Name 1 | Accounts and client area |
| Name 2 | Offers, companies and filters |
| Name 3 | Applications and admin statistics |

## Run it locally
```bash
git clone https://github.com/USERNAME/khedmahub.git
cd khedmahub
composer install
```
Create a file named `.env.local` and set your database:
```
DATABASE_URL="mysql://root:@127.0.0.1:3306/khedmahub"
```
Then:
```bash
php bin/console doctrine:database:create
php bin/console doctrine:migrations:migrate
symfony server:start
```