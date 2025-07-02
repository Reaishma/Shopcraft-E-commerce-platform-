

# ShopCraft E-commerce Platform

A modern full-stack e-commerce application built with React, TypeScript, Express.js, and PostgreSQL. This project demonstrates comprehensive web development skills including user authentication, shopping cart functionality, product management, and admin capabilities.

## 🚀 Features

- **User Authentication**: Secure login system with Replit Auth integration
- **Product Catalog**: Browse products with categories, search, and filtering
- **Shopping Cart**: Add/remove items, quantity management, persistent cart
- **Admin Panel**: Complete product and user management system
- **Responsive Design**: Mobile-first approach with modern UI components
- **Database Integration**: PostgreSQL with Drizzle ORM for type-safe operations

## 🛠️ Technology Stack

### Frontend
- **React 18** with TypeScript
- **Vite** for fast development and optimized builds
- **Tailwind CSS** with shadcn/ui component library
- **TanStack Query** for server state management
- **Wouter** for lightweight client-side routing

### Backend
- **Node.js** with Express.js framework
- **TypeScript** with ES modules
- **Drizzle ORM** for database operations
- **PostgreSQL** database
- **Replit Auth** for authentication

### DevOps & Tools
- **ESBuild** for production bundling
- **Drizzle Kit** for database migrations
- **WebSocket** support for real-time features

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/Reaishma/shopcraft-ecommerce.git
cd shopcraft-ecommerce
```
2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.example .env
```

Required environment variables:
- `DATABASE_URL`: PostgreSQL connection string
- `SESSION_SECRET`: Secret key for session management
- `REPL_ID`: Replit application ID
- `ISSUER_URL`: OAuth issuer URL

4. Set up the database:
```bash
npm run db:push
```
5. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## 🏗️ Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Page components
│   │   ├── hooks/          # Custom React hooks
│   │   └── lib/            # Utilities and configurations
├── server/                 # Backend Express application
│   ├── routes.ts          # API route definitions
│   ├── storage.ts         # Database operations
│   ├── db.ts              # Database connection
│   └── replitAuth.ts      # Authentication setup
├── shared/                # Shared types and schemas
│   └── schema.ts          # Database schema definitions
└── package.json           # Project dependencies
```

## 🎯 Key Features Implementation

### Authentication System
- Integrated Replit OpenID Connect for secure user authentication
- Session management with PostgreSQL-backed storage
- Protected routes and API endpoints
- User profile management

Implementation Functionality
- Product catalog with categories and search
- Shopping cart with persistent storage
- Order management system
- Review and rating system
- Newsletter subscription

### Admin Capabilities
- Product CRUD operations
- Category management
- User management with role-based access
- Order status tracking

## 🚀 Deployment

### Development
```bash
npm run dev
```

### Production Build
```bash
npm run build
npm start
```

### Database Management
```bash
# Push schema changes
npm run db:push

# Generate migrations (if needed)
npm run db:generate
```

## 📝 API Endpoints

### Authentication
- `GET /api/auth/user` - Get current user
- `GET /api/login` - Initiate login flow
- `GET /api/logout` - Logout user

### Products
- `GET /api/products` - Get products with filtering
- `GET /api/products/:id` - Get single product
- `POST /api/products` - Create product (admin)
- `PUT /api/products/:id` - Update product (admin)
- `DELETE /api/products/:id` - Delete product (admin)
### Categories
- `GET /api/categories` - Get all categories
- `POST /api/categories` - Create category (admin)

### Orders
- `GET /api/orders` - Get user orders
- `POST /api/orders` - Create new order
- `PUT /api/orders/:id` - Update order status (admin)

## 🧪 Testing
The application includes comprehensive error handling and validation:
- Form validation with Zod schemas
- Database constraint validation
- Authentication middleware protection
- Input sanitization and security measures

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Developer
**Reaishma N**
- Email: [vra.9618@gmail.com](mailto:vra.9618@gmail.com)
- GitHub: [@Reaishma](https://github.com/Reaishma)
- Portfolio: [https://new.express.adobe.com/webpage/3dP7n40mSx6LX]

##  Acknowledgments

- Built with modern web development best practices
- Utilizes industry-standard tools and frameworks
- Designed for scalability and maintainability
- Optimized for performance and user experience

---

*This project demonstrates full-stack development capabilities including frontend design, backend API development, database design, authentication systems, and deployment strategies.*