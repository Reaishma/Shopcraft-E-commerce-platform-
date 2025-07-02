# GitHub Deployment Guide for ShopCraft E-commerce Platform

This guide will help you deploy your ShopCraft e-commerce portfolio to GitHub and various hosting platforms.

## 📋 Prerequisites

1. GitHub account
2. Git installed on your local machine
3. Database hosting (Neon, Supabase, or similar PostgreSQL provider)

## 🚀 Deployment Steps

### 1. Prepare Your Repository

First, create a new GitHub repository:

1. Go to [GitHub](https://github.com) and create a new repository
2. Name it `shopcraft-ecommerce` or your preferred name
3. Set it to public (for GitHub Pages) or private
4. Don't initialize with README (we already have one)

### 2. Initialize Git and Push to GitHub
Run these commands in your project directory:

```bash
# Initialize git repository

git init
git add .

# Make initial commit
git commit -m "Initial commit: ShopCraft e-commerce platform"

# Add your GitHub repository as origin

git remote add origin https://github.com/Reaishma/shopcraft-ecommerce.git

# Push to GitHub

git branch -M main
git push -u origin main


### 3. Platform Up Environment Variable 

For different hosting platforms, you'll need to configure environment variables:

#### Required Environment Variables:
```
DATABASE_URL=your_postgresql_connection_string
SESSION_SECRET=your_secret_key_here
REPL_ID=your_app_id
ISSUER_URL=https://replit.com/oidc
REPLIT_DOMAINS=your-domain.com
NODE_ENV=production
PORT=5000
```


## 🌐 Hosting Platform Options


### Option 1: Vercel (Recommended for Full-Stack)

1. Go to [Vercel](https://vercel.com)
2. Sign up with your GitHub account
3. Import your repository
4. Add environment variables in the Vercel dashboard
5. Deploy automatically



### Option 2: Netlify + Database

1. Go to [Netlify](https://netlify.com)
2. Connect your GitHub repository
3. Set build command: `npmbuild`uild`
4. Set publish directory: `dist`
5. Add environment variables in Netlify dashboard


### Option 3: Railway

1. Go to [Railway](https://railway.app)
2. Connect GitHub repository
3. Add PostgreSQL database service
4. Configure environment variables
5. Deploy with automatic builds


### Option 4: Render

1. Go to [Render](https://render.com)
2. Create new web service from GitHub
3. Add PostgreSQL database
4. Configure environment variables
5. Deploy


## 🗄️ Database Setup

### Option 1: Neon (Recommended)

1. Sign up at [Neon](https://neon.tech)
2. Create a new database
3. Copy the connection string
4. Add to your environment variables


### Option 2: Supabase

1. Sign up at [Supabase](https://supabase.com)
2. Create new project
3. Get the database URL from settings
4. Add to your environment variables


### Option 3: PlanetScale

1. Sign up at [PlanetScale](https://planetscale.com)
2. Create database
3. Get connection string
4. Add to your environment variables


## 🔧 Build Configuration
The project is already configured with:

- ✅ GitHub Actions workflow in `.github/workflows/deploy.yml`
- ✅ Production build scripts
- ✅ Environment variable examples in `.env.example`
- ✅ Comprehensive README.md


## 📊 Features to Highlight

Your deployed portfolio will showcase:

- **Full-Stack Development**: React frontend with Express backend
- **Database Integration**: PostgreSQL with Drizzle ORM
- **Authentication**: Secure user login system
- **E-commerce Features**: Shopping cart, product management, orders
- **Admin Panel**: Complete product and user management
- **Responsive Design**: Mobile-first approach
- **Modern Tech Stack**: TypeScript, Tailwind CSS, modern tooling


## 🚨 Important Notes

1. **Database**: Make sure to run `npm run db:push` after setting up your database
2. **Environment Variables**: Never commit `.env` files to GitHub
3. **Build Process**: The application uses Vite for frontend and esbuild for backend
4. **Authentication**: Configure Replit Auth or replace with your preferred auth provider


## 📈 Next Steps

After deployment:

1. Test all functionality on the live site
2. Set up monitoring and analytics
3. Configure custom domain (optional)
4. Add SSL certificate (usually automatic)
5. Set up CI/CD for automatic deployments

## 🆘 Troubleshooting

### Common Issues:

1. **Build Failures**: Check environment variables are set correctly
2. **Database Connection**: Verify DATABASE_URL is correct
3. **Authentication Issues**: Ensure REPL_ID and domains are configured
4. **Asset Loading**: Check that static files are being served correctly

### Support:

If you encounter issues:

1. Check the hosting platform's logs
2. Verify all environment variables are set
3. Test the build process locally first
4. Check database connectivity

---

**Developer:** Reaishma N  
**Email:** vra.9618@gmail.com  
**GitHub:** [@Reaishma](https://github.com/Reaishma)

This deployment showcases comprehensive full-stack development skills and modern web development practices.