# ⚡ Vite React TypeScript TailwindCSS Starter

<div align="center">

![Vite](https://img.shields.io/badge/Vite-4.4+-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![React](https://img.shields.io/badge/React-18+-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5+-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3+-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

🚀 *A modern, blazing-fast React starter template with the best development experience*

[📖 Usage](#-usage) • [⚡ Features](#-features) • [🛠️ Tech Stack](#️-tech-stack) • [🎯 Getting Started](#-getting-started)

</div>

---

## ✨ Why This Template?

Stop wasting time configuring your React projects! This template comes with everything you need to build modern, scalable web applications with **zero configuration**. Built with performance and developer experience in mind.

---

## 🎯 Features

- ⚡ **Instant HMR** - Lightning-fast hot module replacement with Vite
- 🔷 **TypeScript** - Full type safety and better DX
- 🎨 **TailwindCSS** - Utility-first CSS framework with unlimited customization
- 📦 **Lucide React** - Beautiful, consistent icon library (pre-installed!)
- 🔧 **ESLint** - Code quality and consistency
- 📱 **Mobile-First** - Responsive design out of the box
- 🚀 **Production Ready** - Optimized builds with tree-shaking
- 🎯 **Zero Config** - Start coding immediately

---

## 🛠️ Tech Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| **Vite** | ^5.0 | Build tool & dev server |
| **React** | ^18.2 | UI library |
| **TypeScript** | ^5.2 | Type safety |
| **TailwindCSS** | ^3.4 | Styling framework |
| **Lucide React** | ^0.445 | Icon library |

---

## 🚀 Getting Started

### Prerequisites

Make sure you have **Node.js 18+** installed:

```bash
node --version
npm --version
```

### Quick Start

1. **Clone & Install**
   ```bash
   git clone <your-repo-url>
   cd your-project-name
   npm install
   ```

2. **Start Development**
   ```bash
   npm run dev
   ```

3. **Open Browser**
   Navigate to `http://localhost:5173`

---

## 📋 Available Scripts

```bash
# Start development server with HMR
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Run linter
npm run lint

# Type checking
npm run type-check
```

---

## 🎨 Customization Guide

### Adding New Components

```tsx
// src/components/Button.tsx
import { ButtonHTMLAttributes } from 'react'

interface ButtonProps extends ButtonHTMLAttributes<HTMLButtonElement> {
  variant?: 'primary' | 'secondary'
}

export function Button({ variant = 'primary', className = '', ...props }: ButtonProps) {
  const baseClass = 'px-4 py-2 rounded-lg font-medium transition-colors'
  const variantClass = variant === 'primary' 
    ? 'bg-blue-500 text-white hover:bg-blue-600' 
    : 'bg-gray-200 text-gray-900 hover:bg-gray-300'
    
  return (
    <button 
      className={`${baseClass} ${variantClass} ${className}`}
      {...props} 
    />
  )
}
```

### Using Icons

```tsx
import { Star, Heart, Download } from 'lucide-react'

export function IconExample() {
  return (
    <div className="flex gap-4">
      <Star className="text-yellow-500" size={24} />
      <Heart className="text-red-500" size={24} />
      <Download className="text-blue-500" size={24} />
    </div>
  )
}
```

### TailwindCSS Configuration

Edit `tailwind.config.js` to customize your design system:

```javascript
export default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {
      colors: {
        primary: '#your-brand-color',
        secondary: '#your-accent-color',
      },
      fontFamily: {
        sans: ['Inter', 'system-ui', 'sans-serif'],
      },
    },
  },
  plugins: [],
}
```

---

## 📁 Project Structure

```
your-project/
├── public/              # Static assets
├── src/
│   ├── components/      # Reusable components
│   ├── pages/          # Page components
│   ├── hooks/          # Custom hooks
│   ├── utils/          # Utility functions
│   ├── types/          # TypeScript types
│   ├── App.tsx         # Main app component
│   ├── main.tsx        # App entry point
│   └── index.css       # TailwindCSS imports
├── index.html          # HTML template
├── package.json        # Dependencies
├── tailwind.config.js  # TailwindCSS config
├── tsconfig.json       # TypeScript config
└── vite.config.ts      # Vite config
```

---

## 🏗️ Building for Production

```bash
# Build optimized production bundle
npm run build

# Preview production build locally
npm run preview
```

The build output will be in the `dist/` folder, ready for deployment to any static hosting service.

---

## 🚀 Deployment

This template works perfectly with:

- **Vercel** - Zero-config deployment
- **Netlify** - Drag & drop deployment
- **GitHub Pages** - Static hosting
- **AWS S3 + CloudFront** - Enterprise hosting
- **Any static hosting service**

---

## 🤝 Contributing

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- [Vite](https://vitejs.dev/) for the amazing build tool
- [React](https://react.dev/) for the UI library
- [TailwindCSS](https://tailwindcss.com/) for the utility-first CSS framework
- [Lucide](https://lucide.dev/) for the beautiful icons

---

<div align="center">

**⭐ Star this repository if it helped you!**

Made with ❤️ by [mhanafi09051998](https://github.com/mhanafi09051998)

</div>