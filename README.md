# Waxtix Authentication

This is a deploy-ready Waxtix authentication frontend using Supabase Auth.

## Supported sign-in methods
- Email + password
- Google OAuth
- Phone number + SMS OTP

## GitHub
Upload all files/folders in this project to a GitHub repository.

## Render
Create a Static Site from the GitHub repository.
- Build Command: `npm install && npm run build`
- Publish Directory: `dist`

Add these environment variables in Render:
- `VITE_SUPABASE_URL`
- `VITE_SUPABASE_ANON_KEY`

## Supabase setup
In Supabase Authentication:
1. Enable Email.
2. Enable Google and create/configure Google OAuth credentials.
3. Enable Phone and configure an SMS provider.
4. Add your Render site URL to the Authentication URL configuration / redirect URLs.

Do not put a Supabase service-role key in this website. Only the public anon/publishable key belongs in frontend environment variables.

## Important
The supplied phone login uses SMS OTP. SMS-provider configuration is required in Supabase before it can send real codes.
