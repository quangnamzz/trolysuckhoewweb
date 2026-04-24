# Asset Guide - Trợ lý Sức khỏe

Hướng dẫn chi tiết về các tài sản (assets), biểu tượng SVG, màu sắc, và cách tùy chỉnh chúng.

## 📋 Danh sách SVG Assets

Tất cả SVG assets được nhúng trực tiếp trong file `index.html`. Dưới đây là danh sách đầy đủ:

### 1. Logo (Header)
**Vị trí**: Line ~130-145 trong `<nav>`  
**ID**: `logoGradient`  
**Mô tả**: Medical cross icon với gradient cyan-to-lime

```svg
<svg class="w-8 h-8" viewBox="0 0 32 32">
  <defs>
    <linearGradient id="logoGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#00f0ff;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#22c55e;stop-opacity:1" />
    </linearGradient>
  </defs>
  <!-- Medical Cross -->
  <rect x="14" y="6" width="4" height="20" fill="url(#logoGradient)" rx="2"/>
  <rect x="6" y="14" width="20" height="4" fill="url(#logoGradient)" rx="2"/>
  <circle cx="16" cy="16" r="14" stroke="url(#logoGradient)" stroke-width="2" fill="none"/>
</svg>
```

**Tùy chỉnh**:
- Thay đổi viewBox để scale khác
- Sửa `fill="url(#logoGradient)"` thành hex color: `fill="#00f0ff"`
- Điều chỉnh stroke-width cho độ dày

### 2. Checkmark Icon (Navigation)
**Vị trí**: Line ~152-156  
**Mô tả**: Tick icon xanh dương

```svg
<svg class="w-4 h-4 text-cyan-400" fill="currentColor" viewBox="0 0 20 20">
  <path d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"/>
</svg>
```

### 3. Feature Icons (Feature Cards Section)

#### Icon 1: People/Share (Chia sẻ hồ sơ)
**Vị trí**: Line ~360 trong feature card 1  
**Color**: `text-amber-500`

```svg
<svg class="w-12 h-12 text-amber-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" 
        d="M17 20h5v-2a3 3 0 00-5.856-1.487M15 10a3 3 0 11-6 0 3 3 0 016 0zM15 20H9m6 0h.01M9 20H3v-2a6 6 0 0112 0v2z" />
</svg>
```

#### Icon 2: Chart/Analytics (Theo dõi)
**Vị trí**: Line ~381 trong feature card 2  
**Color**: `text-cyan-500`

```svg
<svg class="w-12 h-12 text-cyan-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" 
        d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
</svg>
```

#### Icon 3: Family/Heart (Gia đình)
**Vị trí**: Line ~402 trong feature card 3  
**Color**: `text-orange-500`

```svg
<svg class="w-12 h-12 text-orange-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" 
        d="M12 4.354a4 4 0 110 5.292M15 19H9a6 6 0 016-6h0a6 6 0 016 6v1" />
</svg>
```

### 4. Footer Social Icons

#### Facebook Icon
```svg
<svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
  <path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/>
</svg>
```

#### Twitter/X Icon
```svg
<svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
  <path d="M23 3a10.9 10.9 0 01-3.14 1.53 4.48 4.48 0 00-7.86 3v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2s9 5 20 5a9.5 9.5 0 00-9-5.5c4.75 2.25 7-7 7-7"/>
</svg>
```

## 🎨 Color Palette Reference

### Primary Colors (Neon)
| Tên | Hex | RGB | Sử dụng |
|-----|-----|-----|--------|
| Neon Cyan | `#00f0ff` | rgb(0, 240, 255) | Logo, text accent, borders |
| Neon Lime | `#22c55e` | rgb(34, 197, 94) | Accent text, highlights |
| Neon Orange | `#f97316` | rgb(249, 115, 22) | CTA buttons, important text |
| Amber/Gold | `#fbbf24` | rgb(251, 191, 36) | Button background, hover states |

### Background Colors
| Tên | Hex | RGB | Sử dụng |
|-----|-----|-----|--------|
| Dark Slate 950 | `#0f172a` | rgb(15, 23, 42) | Main background |
| Dark Slate 900 | `#1e293b` | rgb(30, 41, 59) | Secondary background |
| Dark Slate 800 | `#1e293b` | rgb(30, 41, 59) | Card backgrounds |
| Light Slate 100 | `#f1f5f9` | rgb(241, 245, 249) | Feature cards section |

### Text Colors
| Tên | Class | Sử dụng |
|-----|-------|--------|
| White | `text-white` | Main headings, primary text |
| Slate 300 | `text-slate-300` | Body text, secondary text |
| Slate 400 | `text-slate-400` | Tertiary text, labels |
| Slate 600 | `text-slate-600` | Light section text |
| Cyan 400 | `text-cyan-400` | Accent text, hover states |

## 🎨 Gradient Definitions

### Logo Gradient
```css
linear-gradient(90deg, #00f0ff, #22c55e)
```
Sử dụng cho: Logo, gradient text, headings

### Hero Background Gradient
```css
linear-gradient(135deg, rgba(0, 240, 255, 0.15) 0%, rgba(138, 43, 226, 0.1) 50%, rgba(34, 197, 94, 0.15) 100%)
```
Sử dụng cho: Hero section background

### Button Gradient
```css
linear-gradient(135deg, #fbbf24 0%, #f97316 100%)
```
Sử dụng cho: CTA buttons (amber to orange)

## ✨ Glow & Shadow Effects

### Text Glow (Neon Text)
```css
text-shadow: 0 0 10px rgba(0, 240, 255, 0.6), 
             0 0 20px rgba(34, 197, 94, 0.3);
```

### Button Glow
```css
box-shadow: 0 0 20px rgba(251, 191, 36, 0.4), 
            inset 0 0 20px rgba(255, 255, 255, 0.1);
```

### Card Hover Glow
```css
box-shadow: 0 20px 40px rgba(0, 240, 255, 0.15);
```

## 🎬 Animations

### Fade In
```css
animation: fadeIn 0.8s ease-in-out;

@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
```

### Glow Movement
```css
animation: glow-move 15s ease-in-out infinite;

@keyframes glow-move {
    0%, 100% { transform: translate(0, 0); }
    50% { transform: translate(30px, -30px); }
}
```

### Hover Transform
```css
transition: all 0.3s ease;
transform: translateY(-8px);
```

## 📐 iPhone Mockup Specifications

### Frame Dimensions
- **Width**: 280px (desktop), 240px (mobile)
- **Height**: 580px (desktop), 500px (mobile)
- **Border Radius**: 40px (main frame), 32px (screen)
- **Border**: 8px solid black
- **Notch**: 24px height, 150px width

### Screen Content Area
- **Padding**: 16px
- **Border Radius**: 32px
- **Overflow**: Hidden (content scaled to fit)

### Health Data Display
- **Stats**: Cyan background with 1px border, 12px padding
- **Chart Bars**: 3px width, gradient cyan-to-lime
- **Family Avatars**: 6px size, rounded full, gradient fills

## 🔄 How to Add Custom SVG Icons

1. **Find your SVG** on icon library (Heroicons, Feather, Font Awesome)
2. **Copy the SVG code**
3. **Locate insertion point** in index.html
4. **Paste SVG** ensuring viewBox is present
5. **Add Tailwind classes** for sizing and color:
   ```html
   <svg class="w-12 h-12 text-cyan-400" ...>
   ```

**Example**:
```html
<!-- Before -->
<div class="mb-6"></div>

<!-- After -->
<div class="mb-6">
    <svg class="w-12 h-12 text-cyan-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="..." />
    </svg>
</div>
```

## 🎯 Color Class Mappings (Tailwind)

### Text Colors
- `text-white` → White
- `text-slate-300` → Light gray
- `text-slate-400` → Medium gray
- `text-slate-600` → Darker gray
- `text-cyan-400` → Neon cyan
- `text-amber-500` → Amber/gold
- `text-orange-500` → Neon orange

### Background Colors
- `bg-slate-950` → Dark background
- `bg-slate-900` → Secondary dark
- `bg-slate-800` → Card background
- `bg-white` → Light background
- `bg-gradient-to-r from-X to-Y` → Gradient

### Border Colors
- `border-slate-800` → Dark border
- `border-slate-700` → Medium border
- `border-cyan-400` → Neon cyan border

## 🖼️ Image Placeholder Strategy

Since the project uses only SVG and CSS, here are alternatives for adding images:

### Option 1: Data URIs (Base64)
```html
<img src="data:image/png;base64,iVBORw0KGgo..." alt="...">
```

### Option 2: External Images
```html
<img src="https://cdn.example.com/image.jpg" alt="..." loading="lazy">
```

### Option 3: CSS Background Images
```css
.card {
    background-image: url('data:image/svg+xml;...');
}
```

## 📊 Responsive Image Sizing

Use Tailwind width classes:
- `w-4` → 16px (small icons)
- `w-6` → 24px (medium icons)
- `w-8` → 32px (large icons)
- `w-12` → 48px (feature icons)
- `w-full` → 100% (responsive images)

## 🔧 Advanced Customization

### Change All Neon Cyan References
Search & Replace in index.html:
- `#00f0ff` → your hex color
- `text-cyan-400` → `text-your-color-400`
- `rgba(0, 240, 255, ...` → `rgba(yourR, yourG, yourB, ...`

### Add New Color Scheme
1. Define new CSS variables:
   ```css
   :root {
       --primary: #your-color;
       --secondary: #your-color-2;
   }
   ```

2. Replace existing color references

### Create Dark Mode Toggle
```javascript
document.documentElement.classList.toggle('dark');
```

## 📝 Notes

- All colors use hex notation for consistency
- RGB values provided for reference only
- Opacity/alpha values use 0-1 scale (0 = transparent, 1 = opaque)
- Tailwind CDN automatically handles vendor prefixes
- SVG filters (feGaussianBlur, etc.) supported in all modern browsers

---

**Last Updated**: April 23, 2026  
**Version**: 1.0
