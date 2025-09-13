# HR Management Dashboard - ReactJS & DaisyUI

## Project Overview

A modern, responsive HR Management Dashboard built with ReactJS and DaisyUI that provides comprehensive human resources management capabilities with beautiful light and dark mode themes.

![React](https://img.shields.io/badge/React-18.2.0-blue)
![DaisyUI](https://img.shields.io/badge/DaisyUI-4.4.19-purple)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.3.5-cyan)
![License](https://img.shields.io/badge/License-MIT-green)

## Features

-  **Employee Management**: Complete CRUD operations for employee records
-  **Dashboard Analytics**: Key HR metrics and visual data representations
-  **Attendance Tracking**: Employee check-in/check-out with timesheets
-  **Payroll Management**: Salary processing and payment history
-  **Performance Reviews**: Employee evaluation and goal tracking
-  **Theme Support**: Light/dark mode with custom dark blue theme
-  **Fully Responsive**: Works seamlessly on desktop, tablet, and mobile
-  **Role-based Access**: Different permissions for admin, managers, and staff

## Technology Stack

- **Frontend Framework**: ReactJS (JavaScript)
- **UI Component Library**: DaisyUI with TailwindCSS
- **Build Tool**: Vite
- **Routing**: React Router DOM
- **HTTP Client**: Axios
- **Icons**: React Icons
- **Charts**: Recharts (for data visualization)
- **Form Handling**: React Hook Form
- **State Management**: React Context API

## Prerequisites

- Node.js v22.19.0 or higher
- npm v11.6.0 or higher
- WebStorm 2025.1 (recommended) or any code editor

## Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/hr-management-dashboard.git
   cd hr-management-dashboard
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` to view the application

## Project Structure

```
src/
├── components/
│   ├── layout/          # Header, Sidebar, Footer
│   ├── dashboard/       # Dashboard-specific components
│   ├── employees/       # Employee management components
│   ├── attendance/      # Attendance tracking components
│   ├── payroll/         # Payroll management components
│   └── ui/              # Reusable UI components
├── pages/               # Main page components
├── contexts/            # React contexts (Theme, Auth)
├── hooks/               # Custom React hooks
├── services/            # API services
├── utils/               # Helper functions
├── styles/              # Global styles
└── assets/              # Images, icons, etc.
```

## Theme Configuration

The project uses DaisyUI's built-in theme system with a custom dark blue theme for night mode:

- **Light Theme**: Clean, professional design with light gray and blue accents
- **Dark Theme**: Custom dark blue theme (#0f172a) for reduced eye strain

Toggle between themes using the theme switch in the header.

## API Integration with Apidog

This project uses Apidog for API testing and documentation:

1. **Install Apidog**: Download from [https://apidog.com](https://apidog.com)
2. **Import API Collection**: Import the provided JSON collection from `/apidog` folder
3. **Configure Environment**: Set up your base URL and authentication tokens
4. **Test Endpoints**: Use Apidog to test all HR dashboard API endpoints

### API Services

The dashboard integrates with these core API endpoints:

- `GET /employees` - Retrieve employee list
- `POST /employees` - Create new employee
- `PUT /employees/:id` - Update employee details
- `GET /attendance` - Get attendance records
- `POST /attendance/checkin` - Employee check-in
- `POST /attendance/checkout` - Employee check-out
- `GET /payroll` - Retrieve payroll data
- `POST /payroll/process` - Process payroll

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint
- `npm run test` - Run test suite

## Customization

### Adding New Pages

1. Create component in `/pages` directory
2. Add route in `App.jsx`
3. Add navigation link in `Sidebar.jsx`

### Modifying Themes

Edit the `tailwind.config.js` file to customize color schemes:

```javascript
themes: [
  {
    light: {
      // Light theme customization
      primary: '#4f46e5',
      secondary: '#06b6d4',
    },
    dark: {
      // Dark theme customization
      primary: '#4f46e5',
      secondary: '#06b6d4',
      'base-100': '#0f172a',
    },
  },
],
```

## Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Deployment

### Build for Production

```bash
npm run build
```

The built application will be in the `dist` folder, ready for deployment to any static hosting service like Netlify, Vercel, or GitHub Pages.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

If you have any questions or issues, please create an issue in the GitHub repository or contact the development team.

## Acknowledgments

- DaisyUI for the beautiful component library
- TailwindCSS for the utility-first CSS framework
- Vite for the fast build tooling
- React community for excellent documentation and resources

---

**Happy Coding!** 🚀
