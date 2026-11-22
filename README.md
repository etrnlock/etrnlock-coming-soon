# ETRNLock Coming Soon — static landing page

Contains a static `index.html`, `style.css`, approved ETRNLock logo and purple smoke background, and a Dockerfile using Nginx.

## Coolify deployment

1. Create a new private GitHub repository (e.g. `etrnlock-coming-soon`).
2. Upload the contents of this folder to the root of that repository (not the ZIP itself).
3. In Coolify: Projects → New Project → New Resource → Application → Public Repository (for a public repo) or connect your private GitHub repository.
4. Select the repository, branch `main`, and build pack `Dockerfile` (Dockerfile path: `/Dockerfile`).
5. Set exposed/container port to `80` and assign the domain as `https://your-actual-domain.example` (replace with your real domain).
6. Deploy. Ensure DNS points to the VPS and HTTPS certificate is issued successfully.
7. Once the real application is ready, replace this deployment with your production Blazor application.

Do not deploy the unfinished Blazor application, PostgreSQL admin interface, or registration endpoints publicly for this placeholder.
