# Lee Sage - Luxury Fashion E-commerce Website


A premium e-commerce platform for luxury fashion, built with modern web technologies and a comprehensive admin management system.

## 🌟 Overview

Lee Sage is a sophisticated e-commerce website specializing in luxury fashion and lifestyle products. The platform offers a seamless shopping experience with a beautiful, responsive frontend and a powerful admin panel for complete business management.

### ✨ Key Features

#### 🛍️ Customer Features
- **Product Catalog**: Browse products by categories with advanced filtering and search
- **User Authentication**: Secure registration and login system
- **Shopping Cart & Wishlist**: Add to cart, save favorites, and manage quantities
- **Checkout Process**: Secure payment processing with multiple payment methods
- **Order Tracking**: Real-time order status updates and history
- **Product Reviews**: Rate and review products with approval system
- **Address Management**: Multiple delivery addresses per user
- **Coupon System**: Discount codes and promotional offers
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices

#### 👨‍💼 Admin Features
- **Dashboard Analytics**: Comprehensive business insights and statistics
- **Product Management**: Add, edit, delete products with image uploads
- **Category Management**: Hierarchical category system
- **Order Management**: Process orders, update status, manage fulfillment
- **User Management**: View and manage customer accounts
- **Inventory Control**: Stock management with low-stock alerts
- **Review Moderation**: Approve or reject customer reviews
- **Marketing Campaigns**: Create and manage promotional campaigns
- **Message Center**: Handle customer inquiries and support tickets
- **Security Features**: Session management, activity logging, and access control

## 🛠️ Tech Stack

### Frontend
- **HTML5** - Semantic markup and structure
- **CSS3** - Custom styling with responsive design
- **JavaScript (ES6+)** - Interactive functionality and DOM manipulation
- **Font Awesome** - Icon library for UI elements

### Backend
- **PHP 8.1+** - Server-side scripting and API development
- **MySQL 8.0+** - Relational database management
- **PDO** - Secure database connectivity

### Development Tools
- **XAMPP** - Local development environment
- **Git** - Version control
- **Composer** - PHP dependency management (if needed)

## 📁 Project Structure

```
leesage/
├── index.html                    # Landing page with logo animation
├── admin/                        # Admin panel directory
│   ├── index.html               # Admin login page
│   ├── pages/                   # Admin pages
│   │   ├── dashboard.php        # Main dashboard
│   │   ├── products.html        # Product management
│   │   ├── categories.html      # Category management
│   │   ├── orders.html          # Order management
│   │   ├── users.html           # User management
│   │   ├── reviews.html         # Review moderation
│   │   ├── messages.html        # Customer messages
│   │   ├── payments.html        # Payment management
│   │   ├── inventory.html       # Stock management
│   │   ├── marketing.html       # Marketing campaigns
│   │   ├── profile.html         # Admin profile
│   │   ├── security.html        # Security settings
│   │   └── settings.html        # System settings
│   └── static/                  # Admin assets
│       ├── css/                 # Admin stylesheets
│       ├── js/                  # Admin JavaScript files
│       └── images/              # Admin images
├── public/                      # Public website directory
│   ├── pages/                   # Public pages
│   │   ├── home.html            # Homepage
│   │   ├── shop.html            # Product catalog
│   │   ├── product.html         # Product detail page
│   │   ├── cart.html            # Shopping cart
│   │   ├── checkout.html        # Checkout process
│   │   ├── login.html           # User login
│   │   ├── register.html        # User registration
│   │   ├── profile.html         # User profile
│   │   ├── wishlist.html        # Wishlist page
│   │   ├── about.html           # About us page
│   │   ├── contact.html         # Contact page
│   │   ├── address.html         # Address management
│   │   ├── includes/            # Reusable components
│   │   │   └── footer.html      # Site footer
│   │   └── policies/            # Legal pages
│   │       ├── privacy-policy.html
│   │       └── shipping-policy.html
│   └── static/                  # Public assets
│       ├── css/                 # Public stylesheets
│       └── js/                  # Public JavaScript files
├── backend/                     # Backend API and database
│   ├── README.md                # Backend documentation
│   ├── database/                # Database files
│   │   ├── config.php           # Database configuration
│   │   ├── structure.sql        # Main database structure
│   │   ├── ecommerce_tables.sql # E-commerce tables
│   │   └── leesage_db.sql       # Complete database dump
│   └── php/                     # PHP backend code
│       ├── admin/               # Admin API endpoints
│       │   ├── actions/         # CRUD operations
│       │   ├── api/             # Data retrieval endpoints
│       │   └── auth/            # Authentication handlers
│       ├── public/              # Public API endpoints
│       │   ├── api/             # Public data endpoints
│       │   ├── auth/            # User authentication
│       │   ├── models/          # Data models
│       │   └── utils/           # Utility functions
│       └── logs/                # Application logs
├── assets/                      # Shared assets
│   ├── images/                  # Product and site images
│   ├── videos/                  # Video content
│   ├── icons/                   # Icon files
│   └── profiles/                # User profile images
│       ├── admin/               # Admin profile images
│       └── public/              # User profile images
└── README.md                    # This file
```

## 🗄️ Database Schema

The application uses a comprehensive MySQL database with the following main tables:

### Core Tables
- **`admin_users`** - Admin user accounts and permissions
- **`users`** - Customer accounts
- **`products`** - Product catalog with pricing and descriptions
- **`categories`** - Product categories (hierarchical)
- **`orders`** - Customer orders and transactions
- **`order_items`** - Individual items within orders

### Supporting Tables
- **`product_images`** - Product image gallery
- **`product_sizes`** - Size variants and inventory
- **`product_categories`** - Many-to-many product-category relationships
- **`carts`** & **`cart_items`** - Shopping cart functionality
- **`wishlists`** & **`wishlist_items`** - Wishlist management
- **`addresses`** - User delivery addresses
- **`reviews`** - Product reviews and ratings
- **`coupons`** - Discount codes and promotions
- **`payments`** - Payment transaction records
- **`messages`** - Customer inquiries and support
- **`notifications`** - User notifications
- **`inventory_history`** - Stock change tracking
- **`order_status_history`** - Order status change logs
- **`admin_sessions`** & **`user_sessions`** - Session management
- **`admin_activity_logs`** - Admin action tracking
- **`marketing_campaigns`** - Promotional campaigns

## 🚀 Installation & Setup

### Prerequisites
- **XAMPP** (or similar Apache/MySQL/PHP stack)
- **PHP 8.1+** with PDO extension
- **MySQL 8.0+**
- **Web browser** (Chrome, Firefox, Safari, Edge)
- **Git** (optional, for version control)

### Step-by-Step Installation

1. **Clone or Download the Project**
   ```bash
   git clone <repository-url>
   cd leesage
   ```

2. **Setup XAMPP**
   - Install XAMPP from [apachefriends.org](https://www.apachefriends.org/)
   - Start Apache and MySQL services

3. **Database Setup**
   - Open phpMyAdmin (http://localhost/phpmyadmin)
   - Create a new database named `leesage_db`
   - Import the database files in order:
     1. `backend/database/structure.sql`
     2. `backend/database/ecommerce_tables.sql`
   - Alternatively, import the complete dump: `backend/database/leesage_db.sql`

4. **Configuration**
   - Update database credentials in `backend/database/config.php` if needed
   - Default admin credentials:
     - Username: `admin`
     - Password: `admin123`
     - Email: `admin@leesage.com`

5. **File Permissions**
   - Ensure web server has write permissions for:
     - `assets/images/products/` (for product image uploads)
     - `assets/profiles/` (for profile image uploads)
     - `backend/php/logs/` (for error logging)

6. **Access the Application**
   - Public website: `http://localhost/leesage/`
   - Admin panel: `http://localhost/leesage/admin/`

## 📖 Usage Guide

### For Customers
1. **Browse Products**: Visit the homepage and explore the product catalog
2. **Create Account**: Register for a new account or login to existing one
3. **Shop**: Add products to cart, apply coupons, and checkout
4. **Track Orders**: View order history and current status
5. **Manage Profile**: Update personal information and addresses

### For Administrators
1. **Login**: Access the admin panel with admin credentials
2. **Dashboard**: View business analytics and recent activity
3. **Manage Products**: Add/edit products, manage inventory, upload images
4. **Process Orders**: Update order status, manage fulfillment
5. **Customer Service**: Respond to messages and moderate reviews
6. **Marketing**: Create campaigns and manage promotions

## 🔗 API Endpoints

### Public API
- `GET /backend/php/public/api/get_products.php` - Get products with filters
- `GET /backend/php/public/api/get_categories.php` - Get product categories
- `POST /backend/php/public/auth/login.php` - User authentication
- `POST /backend/php/public/auth/register.php` - User registration

### Admin API
- `GET /backend/php/admin/api/get_dashboard_stats.php` - Dashboard statistics
- `GET /backend/php/admin/api/get_products.php` - Admin product management
- `GET /backend/php/admin/api/get_orders.php` - Order management
- `POST /backend/php/admin/actions/add_product.php` - Add new product
- `POST /backend/php/admin/actions/update_order_status.php` - Update order status

## 🔒 Security Features

- **Password Hashing**: Bcrypt password encryption
- **Session Management**: Secure session handling with expiration
- **CSRF Protection**: Cross-site request forgery prevention
- **Input Validation**: Server-side data validation and sanitization
- **SQL Injection Prevention**: Prepared statements with PDO
- **Activity Logging**: Admin action tracking and audit trails
- **File Upload Security**: Image validation and secure file handling

## 🎨 Design & UX

- **Responsive Design**: Mobile-first approach with breakpoints
- **Modern UI**: Clean, elegant interface with luxury aesthetic
- **Smooth Animations**: CSS transitions and JavaScript animations
- **Accessibility**: WCAG compliant with proper ARIA labels
- **Performance**: Optimized images and lazy loading
- **SEO Friendly**: Semantic HTML and meta tags

## 📱 Mobile Responsiveness

The website is fully responsive and optimized for:
- **Desktop** (1200px+)
- **Tablet** (768px - 1199px)
- **Mobile** (320px - 767px)

## 🧪 Testing

### Manual Testing Checklist
- [ ] User registration and login
- [ ] Product browsing and search
- [ ] Add to cart and checkout process
- [ ] Admin panel functionality
- [ ] Order management workflow
- [ ] Payment processing (if integrated)
- [ ] Mobile responsiveness
- [ ] Cross-browser compatibility

## 🚀 Deployment

### Production Deployment
1. **Web Server**: Apache/Nginx with PHP 8.1+
2. **Database**: MySQL 8.0+ or MariaDB
3. **SSL Certificate**: HTTPS configuration
4. **File Permissions**: Secure file system permissions
5. **Environment Variables**: Production database credentials
6. **Backup Strategy**: Regular database and file backups

### Recommended Hosting
- **Shared Hosting**: SiteGround, Bluehost, HostGator
- **VPS/Cloud**: DigitalOcean, AWS, Google Cloud
- **Managed Hosting**: Heroku, Vercel (with modifications)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit changes (`git commit -am 'Add new feature'`)
4. Push to branch (`git push origin feature/new-feature`)
5. Create a Pull Request

### Development Guidelines
- Follow PHP PSR standards
- Use meaningful commit messages
- Test thoroughly before submitting PR
- Update documentation for new features

## 📄 License

This project is proprietary software. All rights reserved.

## 📞 Support

For support and inquiries:
- **Email**: support@leesage.com
- **Admin Panel**: Built-in message system
- **Documentation**: This README and backend/README.md

## 🔄 Version History

- **v1.0.0** - Initial release with core e-commerce functionality
- Complete admin panel and user management
- Responsive design and mobile optimization
- Payment gateway integration ready

---

**Lee Sage** - Elevating fashion with technology and elegance. ✨
