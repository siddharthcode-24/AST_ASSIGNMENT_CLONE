

## 🚀 Running the Project

### Development Server
```bash
npm run dev
```
Opens at: **http://localhost:3000**

Press `Ctrl+C` to stop

### Type Checking
```bash
npm run type-check
```

### Linting
```bash
npm run lint
```

### Production Build
```bash
npm run build
npm start
```

---

## 🎯 Features

### ✨ Frontend Features
- **Responsive Design** - Mobile, tablet, desktop optimized
- **Image Optimization** - WebP format, lazy loading, responsive images
- **Dynamic Routing** - Click articles to see `/article/1` pages
- **Error Handling** - Graceful error states and fallbacks
- **Loading States** - Skeleton screens while fetching
- **Accessibility** - Semantic HTML, proper ARIA labels

### ⚡ Performance
- **Static Generation** - Pre-rendered HTML for instant loads
- **ISR (Incremental Static Regeneration)** - Revalidates every 60 seconds
- **Code Splitting** - Automatic chunking by Next.js
- **Image Optimization** - Automatic format conversion

### 🔍 SEO
- Meta tags (title, description)
- Open Graph tags (og:title, og:image, etc.)
- JSON-LD structured data (NewsArticle schema)
- Canonical URLs
- Semantic HTML

### 📱 Responsive Breakpoints
- Mobile: 375px (1 column)
- Tablet: 768px (2 columns)
- Desktop: 1920px (3 columns + sidebar)

---

## 🛠️ Customization

### Change Colors
Edit `tailwind.config.js` - adjust orange to your brand color

### Add Real API
Replace `mockData.ts` with your API endpoint:
```typescript
// Replace: const articles = mockData
// With: const articles = await fetch('https://newsapi.org/...')
```

### Modify Articles
Edit `lib/mockData.ts` - add/remove articles from `mockArticles` array

### Update Categories
Edit `components/Navigation.tsx` - change category list

### Customize Styling
All styling uses Tailwind CSS in component `className` attributes

---

## 🐛 Troubleshooting

### "Cannot find module" error
```bash
npm install
npm run dev
```

### "Port 3000 already in use"
```bash
npm run dev -- -p 3001
```

### Images not loading
- Check image URLs are valid
- Check browser console (F12) for errors
- Use real images (not localhost URLs)

### TypeScript errors (blue squiggles)
- These are just warnings
- Run: `npm run type-check` to verify
- App still runs fine

### Blank page or no content
- Check browser console (F12) for errors
- Restart dev server: `Ctrl+C` then `npm run dev`
- Verify all files were copied correctly

---

## 📖 Learning Resources

### Understanding the Project
1. Read **DESIGN_DOCUMENT.md** - learn the design decisions
2. Read **DOCUMENTATION.md** - understand each component
3. Explore the code - open `components/Header.tsx` and read comments

### Setting Up VS Code
1. Read **VS CODE SETUP & RUNNING GUIDE**
2. Install recommended extensions
3. Configure Prettier for auto-formatting

### Deploying
1. Push code to GitHub
2. Connect to Vercel (automatic deploys)
3. Or self-host with: `npm run build && npm start`

---

## 📋 Next Steps

After getting it running:

1. **Explore Components** - Open `components/Header.tsx` and understand structure
2. **View Mock Data** - Open `lib/mockData.ts` to see article format
3. **Test Features** - Click articles, test mobile view (F12)
4. **Customize** - Modify colors, add articles, change content
5. **Add API** - Replace mock data with real NewsAPI endpoint
6. **Deploy** - Push to GitHub and deploy to Vercel

---

## 🎓 Learning Path

### Beginner
1. Follow STEP-BY-STEP SETUP
2. Get it running (`npm run dev`)
3. Explore the UI in browser
4. Read component code

### Intermediate
1. Read DESIGN_DOCUMENT (understand why)
2. Modify component styling
3. Add/remove mock articles
4. Test error scenarios

### Advanced
1. Integrate real API
2. Add search/filtering
3. Implement infinite scroll
4. Add user authentication
5. Deploy to production

---

## 🔧 Technology Stack

- **Next.js 14** - React framework with SSG/ISR
- **React 18** - UI library
- **TypeScript** - Type-safe JavaScript
- **Tailwind CSS** - Utility-first CSS
- **ESLint** - Code quality
- **Prettier** - Code formatting

---

## 📞 Common Questions

**Q: How do I add a real API?**
A: Replace `getMockNews()` in pages with real API fetch

**Q: Can I change the language?**
A: Yes - all Hindi text is in components, change to English

**Q: How do I deploy?**
A: Push to GitHub, connect Vercel, auto-deploys on push

**Q: Is this production-ready?**
A: Yes - but add authentication, real API, and testing for production

**Q: Can I use this for my project?**
A: Yes - it's completely yours to modify and use

---

## 📄 Files Included

### Code Files (16 total)
- 8 Components
- 2 Pages
- 1 Type definition file
- 1 Mock data file
- 3 Config files
- 1 VS Code settings file

### Documentation (8 files)
- Setup guides
- Design document
- Code documentation
- Testing guide
- Troubleshooting guide
- Complete index

---


## 📝 License

This project is provided as-is for educational purposes. Use and modify freely.

---

## 🙏 Credits

Built with:
- Next.js
- React
- TypeScript
- Tailwind CSS
- Mock data for demonstration
