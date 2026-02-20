# Modern CSS Snippets for Future Enhancements

## 🎨 CSS Variables Customization

You can easily customize colors by modifying these variables in `assets/css/style.css`:

```css
:root {
  /* Change primary color */
  --primary-color: #6366f1;
  --primary-dark: #4f46e5;
  
  /* Change secondary color */
  --secondary-color: #8b5cf6;
  
  /* Change accent color */
  --accent-color: #ec4899;
  
  /* Change text colors */
  --text-primary: #1e293b;
  --text-secondary: #64748b;
}
```

## 🌙 Dark Mode Implementation

Add this to your CSS for dark mode support:

```css
@media (prefers-color-scheme: dark) {
  :root {
    --primary-color: #818cf8;
    --light-bg: #1e293b;
    --text-primary: #f1f5f9;
    --text-secondary: #cbd5e1;
  }
  
  body {
    background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
  }
}
```

## ✨ Additional Animation Classes

Add these for enhanced animations:

```css
/* Slide in from left */
.slide-in-left {
  animation: slideInLeft 0.6s cubic-bezier(0.4, 0, 0.2, 1);
}

@keyframes slideInLeft {
  from {
    opacity: 0;
    transform: translateX(-30px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

/* Fade in */
.fade-in {
  animation: fadeIn 0.6s cubic-bezier(0.4, 0, 0.2, 1);
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Scale up */
.scale-up {
  animation: scaleUp 0.6s cubic-bezier(0.4, 0, 0.2, 1);
}

@keyframes scaleUp {
  from {
    opacity: 0;
    transform: scale(0.9);
  }
  to {
    opacity: 1;
    transform: scale(1);
  }
}

/* Bounce effect */
.bounce {
  animation: bounce 0.6s cubic-bezier(0.4, 0, 0.2, 1);
}

@keyframes bounce {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}
```

## 🎯 Advanced Button Styles

```css
/* Glass button */
.btn-glass {
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
  color: white;
  padding: 1rem 2rem;
  border-radius: 50px;
  font-weight: 700;
  transition: all 0.3s ease;
}

.btn-glass:hover {
  background: rgba(255, 255, 255, 0.2);
  transform: translateY(-3px);
  box-shadow: 0 15px 40px rgba(0, 0, 0, 0.2);
}

/* Outline button */
.btn-outline {
  background: transparent;
  border: 2px solid var(--primary-color);
  color: var(--primary-color);
  padding: 0.8rem 1.8rem;
  border-radius: 50px;
  font-weight: 700;
  transition: all 0.3s ease;
}

.btn-outline:hover {
  background: var(--primary-color);
  color: white;
  transform: translateY(-3px);
  box-shadow: 0 10px 30px rgba(99, 102, 241, 0.3);
}

/* Icon button */
.btn-icon {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  background: var(--gradient-primary);
  color: white;
  border: none;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 1.5rem;
}

.btn-icon:hover {
  transform: scale(1.1) translateY(-3px);
  box-shadow: 0 10px 30px rgba(99, 102, 241, 0.3);
}
```

## 🎨 Card Variations

```css
/* Elevated card */
.card-elevated {
  background: white;
  border-radius: 1.5rem;
  padding: 2rem;
  box-shadow: 0 20px 50px rgba(99, 102, 241, 0.15);
  transition: all 0.3s ease;
}

.card-elevated:hover {
  transform: translateY(-10px);
  box-shadow: 0 30px 60px rgba(99, 102, 241, 0.25);
}

/* Gradient card */
.card-gradient {
  background: var(--gradient-primary);
  border-radius: 1.5rem;
  padding: 2rem;
  color: white;
  box-shadow: 0 20px 50px rgba(99, 102, 241, 0.2);
}

/* Glassmorphic card */
.card-glass {
  background: rgba(255, 255, 255, 0.8);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(99, 102, 241, 0.1);
  border-radius: 1.5rem;
  padding: 2rem;
  box-shadow: 0 10px 30px rgba(99, 102, 241, 0.1);
}

/* Border card */
.card-border {
  background: white;
  border: 2px solid var(--primary-color);
  border-radius: 1.5rem;
  padding: 2rem;
  transition: all 0.3s ease;
}

.card-border:hover {
  border-color: var(--accent-color);
  box-shadow: 0 10px 30px rgba(99, 102, 241, 0.2);
}
```

## 🌈 Gradient Backgrounds

```css
/* Subtle gradient */
.bg-gradient-subtle {
  background: linear-gradient(135deg, #f8fafc 0%, #f1f5f9 100%);
}

/* Bold gradient */
.bg-gradient-bold {
  background: var(--gradient-primary);
}

/* Accent gradient */
.bg-gradient-accent {
  background: var(--gradient-accent);
}

/* Mesh gradient effect (requires multiple gradients) */
.bg-gradient-mesh {
  background: 
    radial-gradient(at 20% 50%, rgba(99, 102, 241, 0.1) 0px, transparent 50%),
    radial-gradient(at 80% 80%, rgba(139, 92, 246, 0.1) 0px, transparent 50%),
    radial-gradient(at 40% 80%, rgba(236, 72, 153, 0.05) 0px, transparent 50%);
}
```

## 🎯 Text Effects

```css
/* Gradient text */
.text-gradient {
  background: var(--gradient-primary);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Accent gradient text */
.text-gradient-accent {
  background: var(--gradient-accent);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Shadow text */
.text-shadow {
  text-shadow: 0 4px 15px rgba(99, 102, 241, 0.2);
}
```

## 🔄 Transition Utilities

```css
/* Fast transition */
.transition-fast {
  transition: all 0.15s cubic-bezier(0.4, 0, 0.2, 1);
}

/* Normal transition */
.transition-normal {
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

/* Slow transition */
.transition-slow {
  transition: all 0.6s cubic-bezier(0.4, 0, 0.2, 1);
}
```

## 📊 Shadow System

```css
/* Subtle shadow */
.shadow-sm {
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
}

/* Medium shadow */
.shadow-md {
  box-shadow: 0 10px 30px rgba(99, 102, 241, 0.1);
}

/* Large shadow */
.shadow-lg {
  box-shadow: 0 20px 50px rgba(99, 102, 241, 0.15);
}

/* XL shadow */
.shadow-xl {
  box-shadow: 0 30px 60px rgba(99, 102, 241, 0.25);
}
```

## 🎬 Tips for Implementation

1. **Use CSS Variables**: Always use `var(--primary-color)` for consistency
2. **Test Animations**: Use DevTools to check performance
3. **Mobile First**: Test all effects on mobile devices
4. **Accessibility**: Ensure animations don't distract or cause issues
5. **Performance**: Use `transform` and `opacity` for animations (GPU accelerated)
6. **Fallbacks**: Provide fallback styles for older browsers

## 🚀 Performance Tips

```css
/* Enable GPU acceleration */
.element {
  transform: translateZ(0);
  will-change: transform;
}

/* Optimize hover states */
@media (hover: hover) {
  .element:hover {
    /* Hover effects only on devices that support hover */
  }
}

/* Reduce motion for accessibility */
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

Happy styling! 🎨✨
