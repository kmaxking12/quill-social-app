# Quill Architecture

## Project Structure

```
src/
├── App.tsx                 # Main application shell and navigation
├── main.tsx                # React entry point
├── styles.css              # Theme tokens and global styles
├── types.ts                # TypeScript interfaces and types
├── data/
│   └── mockData.ts         # Sample content for development
├── components/             # (Ready for reusable UI components)
├── services/               # (Ready for API and auth services)
├── hooks/                  # (Ready for custom React hooks)
└── context/                # (Ready for React Context providers)
```

## Design System

### Color Tokens (CSS Variables)

**Light Mode:**
- Background: `#f6f1ea` (warm ivory)
- Primary: `#5b4ae3` (royal violet)
- Accent: `#ff7f69` (electric coral)
- Text: `#1a1c23` (dark charcoal)
- Panels: White with transparency

**Dark Mode:**
- Background: `#0b1226` (midnight navy)
- Primary: `#8c7cff` (luminous violet)
- Accent: `#ff8a7c` (coral)
- Text: `#edf3ff` (soft white)
- Panels: Navy with transparency

## Integration Roadmap

### Phase 1: Authentication (Next)
- [ ] Google OAuth via Supabase Auth
- [ ] Phone verification flow with SMS OTP
- [ ] Persistent session storage
- [ ] Session revocation and recovery flows

### Phase 2: Database & API
- [ ] Supabase PostgreSQL for users, posts, messages
- [ ] Real feed fetching and pagination
- [ ] Message sync and real-time updates
- [ ] Following/follower relationships

### Phase 3: Media & Storage
- [ ] Supabase Storage for avatars, images, videos
- [ ] Image upload and optimization
- [ ] Video upload and processing

## How to Run Locally

```bash
npm install
npm run dev -- --host 0.0.0.0
```

Then open http://localhost:3000
