# Assets Organization Guide

## Directory Structure

```
/assets
├── images
│   └── projects
│       ├── enterprise-design-system
│       │   ├── hero.png
│       │   ├── benchmark-1.png
│       │   ├── benchmark-2.png
│       │   ├── benchmark-3.png
│       │   ├── benchmark-4.png
│       │   ├── result-1.png
│       │   ├── result-2.png
│       │   ├── result-3.png
│       │   └── result-4.png
│       ├── product-discovery-platform
│       │   ├── hero.png
│       │   ├── dashboard.png
│       │   ├── insights.png
│       │   └── collaboration.png
│       ├── digital-workspace-redesign
│       │   ├── hero.png
│       │   ├── before-after.png
│       │   ├── mobile-view.png
│       │   └── workflow.png
│       └── mobile-banking-app
│           ├── hero.png
│           ├── financial-health.png
│           ├── transactions.png
│           └── security.png
└── README.md
```

## How to Add Images

1. **For Project Hero Images**: 
   - Place in `/assets/images/projects/[project-id]/hero.png`
   - Recommended size: 1920x1080px or 16:9 aspect ratio

2. **For Process/Results Images**:
   - Place in respective project folder with descriptive names
   - Recommended size: 1200x800px or 3:2 aspect ratio

3. **Importing in Code**:
   ```typescript
   // In your project data file
   import heroImage from '../../assets/images/projects/enterprise-design-system/hero.png';
   import benchmarkImage1 from '../../assets/images/projects/enterprise-design-system/benchmark-1.png';
   ```

## Current Setup

For now, we're using:
- Figma imported assets for the enterprise-design-system project
- Unsplash API for placeholder images in other projects

To replace with your own images:
1. Create the folder structure above
2. Add your images to the appropriate folders
3. Update the imports in the project data files
4. The ImageWithFallback component will handle any loading issues gracefully
