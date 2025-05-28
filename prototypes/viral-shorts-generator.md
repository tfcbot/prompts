

---

**Create a clickable prototype for "Viral Shorts Generator" - an AI-powered YouTube shorts creation platform.**

## App Overview
Build a modern, sleek web application that helps content creators generate viral YouTube shorts using AI video generation. The target audience is YouTubers, TikTokers, and content creators looking to scale their short-form video production.

## Pages & User Flow

### 1. Landing Page (`/`)
- **Hero Section**: Bold headline "Create Viral Shorts with AI" with subtext about generating engaging short videos in minutes
- **Features Grid**: 3-4 feature cards highlighting AI generation, quick turnaround, viral optimization, and easy editing
- **Demo Video Section**: Placeholder for a demo video showing the app in action
- **Pricing Teaser**: Brief mention of pricing with CTA to pricing page
- **Header**: Logo, navigation (Features, Pricing, Login, Sign Up), clean and minimal
- **Footer**: Simple links and social media icons
- **CTA Buttons**: Primary "Get Started Free" and secondary "Watch Demo"

### 2. Authentication Pages
- **Sign Up/Login**: Clean Clerk-style authentication forms
- **Onboarding**: Welcome screen after signup with quick tutorial steps

### 3. Dashboard Layout
**Sidebar Navigation**:
- Dashboard overview
- Studio (video creation)
- My Videos (video library)
- Settings
- Billing/Upgrade

**Top Navigation**:
- User avatar/menu
- Notifications bell
- Upgrade button (if on free plan)

### 4. Studio Page (`/dashboard/studio`)
**Video Generation Interface**:
- **Input Section**: 
  - Text area for video description/prompt
  - Dropdown for video style/genre (Comedy, Educational, Trending, etc.)
  - Duration selector (15s, 30s, 60s)
  - Advanced options toggle (aspect ratio, music style, etc.)
- **Preview Area**: Large placeholder for video preview
- **Generate Button**: Prominent "Generate Video" CTA
- **Generation Status**: Progress bar and status updates during generation
- **Recent Generations**: Sidebar showing last 3-5 generated videos

### 5. Videos Library (`/dashboard/videos`)
**Video Management Grid**:
- **Filter Bar**: Search, date range, status filter (completed, processing, failed)
- **Video Cards Grid**: 
  - Thumbnail preview
  - Title/description snippet
  - Creation date
  - Status badge
  - Action buttons (Download, Edit, Delete, Share)
- **Bulk Actions**: Select multiple videos for batch operations
- **Pagination**: Navigate through video library

### 6. Pricing Page (`/pricing`)
**Pricing Tiers**:
- **Free Plan**: Limited generations per month
- **Pro Plan**: Unlimited generations, priority processing, advanced features
- **Enterprise**: Custom solutions
- **Feature Comparison Table**
- **FAQ Section**: Common pricing questions
- **Money-back guarantee badge**

## Design Requirements

### Visual Style
- **Color Scheme**: Modern dark theme with purple/blue accents (think AI/tech focused)
- **Typography**: Clean, modern sans-serif fonts
- **Buttons**: Rounded corners, gradient backgrounds for primary actions
- **Cards**: Subtle shadows, rounded corners, clean borders
- **Icons**: Consistent icon set (video, AI, upload, download, etc.)

### Key Interactive Elements
- **Hover States**: Smooth transitions on buttons and cards
- **Loading States**: Skeleton loaders and progress indicators
- **Success/Error States**: Toast notifications for user feedback
- **Modal Dialogs**: For confirmations, settings, video previews
- **Responsive Design**: Mobile-friendly layout that works on all devices

### Specific UI Components Needed
1. **Video Player**: Custom player with controls for preview
2. **Generation Progress**: Real-time progress bar with percentage
3. **File Upload**: Drag-and-drop areas for additional assets
4. **Settings Panel**: Collapsible panel for advanced video options
5. **Usage Meter**: Show remaining generations/credits
6. **Tooltip System**: Helpful explanations for features

## Mock Data & Content
- Use placeholder video thumbnails (colorful gradients or abstract shapes)
- Sample video titles: "Top 5 Life Hacks", "Quick Recipe Tutorial", "Motivational Quote"
- Fake generation times: "Generating... 45% complete (2 min remaining)"
- Mock user data: Profile pictures, usernames, usage statistics

## Key User Interactions to Prototype
1. **Sign up flow**: Landing page → Auth → Onboarding → Dashboard
2. **Video creation**: Studio page → Fill form → Generate → View result
3. **Video management**: Library → Filter/search → Select video → Actions
4. **Upgrade flow**: Free user → Usage limit → Pricing page → Upgrade

## Technical Notes
- Make it feel like a real SaaS application
- Include realistic loading times and states
- Add subtle animations and micro-interactions
- Ensure the prototype feels premium and professional
- Include proper empty states ("No videos yet", "Start creating")

**Style References**: Think Loom, Canva, or Figma - clean, modern SaaS interfaces with a focus on creativity and productivity.


