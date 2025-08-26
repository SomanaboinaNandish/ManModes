# Deployment Guide

## CI/CD Pipeline Setup (Nandhish)

### Prerequisites
1. GitHub repository for the project
2. Vercel account (or your preferred hosting provider)
3. Node.js 18.x installed locally

### Setup Steps

1. **Create Required Secrets in GitHub**
   - Go to your GitHub repository
   - Navigate to Settings > Secrets > Actions
   - Add the following secrets:
     - `VERCEL_TOKEN`: Your Vercel access token
     - `VERCEL_ORG_ID`: Your Vercel organization ID
     - `VERCEL_PROJECT_ID`: Your Vercel project ID

2. **Vercel Setup**
   - Connect your GitHub repository to Vercel
   - Configure the build settings:
     - Framework: Vite
     - Build Command: `npm run build`
     - Output Directory: `dist`
     - Install Command: `npm ci`

3. **Verify Pipeline**
   - Push changes to the `main` or `develop` branch
   - Check the Actions tab in GitHub to monitor the pipeline
   - Verify the deployment in your Vercel dashboard

### Pipeline Overview
- **Test Job**: Runs on every push/PR to main/develop
- **Build Job**: Creates production build if tests pass
- **Deploy Job**: Deploys to production when pushing to main

### Troubleshooting
1. **Build Failing**
   - Check the logs in GitHub Actions
   - Verify all dependencies are in `package.json`
   - Ensure Node.js version is 18.x

2. **Deployment Issues**
   - Verify Vercel tokens have correct permissions
   - Check environment variables in Vercel
   - Ensure the build output directory matches Vercel settings

### Maintenance
- Keep dependencies updated using `npm outdated`
- Monitor GitHub Actions minutes usage
- Review deployment logs regularly

---
*Maintained by Nandhish - CI/CD Pipeline Lead*
