# requerimientos

A personal wardrobe and shared-memory web app with a mobile-first interface.

Live app: https://requerimientos-psi.vercel.app/

## Current features

- Email account access with a session held in memory.
- Private clothing uploads, filters and favorites.
- Outfit composition on a silhouette, saved outfits and a date agenda.
- Shared spaces with owner, editor and viewer roles.
- Memories with private photo/video galleries, letters and plans.
- Home-screen metadata and an application icon. Internet is required.

## Hosting and privacy

The frontend is static HTML, CSS and JavaScript hosted on Vercel Hobby. Supabase provides Authentication, PostgreSQL and private Storage on its Free plan. The app imports a pinned Supabase JavaScript client from jsDelivr. There are no server functions, paid APIs or AI services. Free-plan quotas still apply.

The browser uses a publishable Supabase key; authorization is enforced by database RLS and private Storage policies. Never add a service-role key, password, access token or private user data to this public repository. The original application and its database remain separate.

## First access

Create an account with the Supabase project owner email and confirm the email. Supabase's default email service restricts delivery to project-team addresses and has a low rate limit. Onboarding other email addresses requires configuring an email provider or another sign-in method.

## Validation and scope

The installed database passed 60 transactional permission/behavior checks and 3 clothing-reference/account-deletion checks; test fixtures were rolled back. The frontend received targeted static reviews and a public-load check. Authenticated browser flows still require the first real account.

This is an initial working version. Album management, background removal, image-search integration, photo-based outfit canvases, password recovery and offline operation are not implemented.

