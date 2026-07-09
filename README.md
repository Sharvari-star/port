# Sharvari Kadam — Portfolio

React Bits powered portfolio — built exactly to your specs.

✨ Stack
- React 18 + Vite + TypeScript + TailwindCSS
- React Bits components:
  - `Galaxy` — animated galaxy WebGL background (OGL)
  - `BorderGlow` — mesh-gradient border glow
  - `GooeyNav` — gooey particle nav
  - `ProfileCard` — 3D tilt holo card
  - `ScrambledText` — free, dependency-free scramble (React Bits API-compatible, no GSAP Club needed)

## Sections

1. **Hero / Home**
   - Fullscreen Galaxy background
     ```tsx
     <Galaxy
       starSpeed={0.5}
       density={1}
       hueShift={140}
       speed={1}
       glowIntensity={0.3}
       saturation={0}
       mouseRepulsion
       repulsionStrength={2}
       twinkleIntensity={0.3}
       rotationSpeed={0.1}
       transparent
     />
     ```
   - Big type:
     ```
     heya
     this is my
     portfolio
     ```
   - Subline: `sharvari kadam` — Graphic Designer • Web Developer

2. **About — BorderGlow**
   ```tsx
   <BorderGlow
     edgeSensitivity={30}
     glowColor="40 80 80"
     backgroundColor="#120F17"
     borderRadius={28}
     glowRadius={44}
     glowIntensity={1.4}
     coneSpread={25}
     animated
     colors={['#c084fc', '#f472b6', '#38bdf8']}
   >
   ```
   Inside:
   - “my name is sharvari kadam im a graphic designer and a web devloper I create stunning visual identities, compelling brand experiences, and beautiful design solutions that help businesses connect with their audience meaningfully.”
   - ScrambledText hover effect
   - Stats: 30+ projects done / 2yrs experience

3. **Nav**
   ```tsx
   <GooeyNav
     items={[
       { label: "Home", href: "#home" },
       { label: "About", href: "#about" },
       { label: "Work", href: "#work" },
       { label: "Contact", href: "#contact" },
     ]}
     particleCount={15}
     particleDistances={[90, 10]}
     particleR={100}
     initialActiveIndex={0}
     animationTime={600}
     timeVariance={300}
     colors={[1,2,3,1,2,3,1,4]}
   />
   ```

4. **ProfileCard**
   ```tsx
   <ProfileCard
     name="Sharvari Kadam"
     title="Graphic Designer • Web Developer"
     handle="sharvarikadam"
     status="Available"
     contactText="Contact Me"
     avatarUrl="https://i.pravatar.cc/400?img=32"
     showUserInfo={true}
     enableTilt={true}
     behindGlowColor="rgba(192,132,252,0.55)"
     innerGradient="linear-gradient(145deg,#60496e8c 0%,#71C4FF44 100%)"
   />
   ```

## Run locally

```bash
cd sharvari-portfolio
npm install
npm run dev
# → http://localhost:5173
```

Build:
```bash
npm run build
npm run preview
```

## Notes

- ScrambledText: I shipped a **free, open-source clone** that is 100% API compatible with React Bits, because the official React Bits version requires GSAP Club plugins (`SplitText` + `ScrambleTextPlugin`). 
  - You can swap back to the official one by:
    ```
    npx shadcn@latest add @react-bits/ScrambledText-JS-CSS
    ```
    and installing GSAP Club.
  - My version file: `src/components/ScrambledText.tsx`

- All 5 React Bits components you asked for are included in `src/components/` — unmodified except ScrambledText.

- Tailwind theme:
  - Syne (display) + Space Grotesk (body)
  - ink #120F17
  - violet #c084fc / pink #f472b6 / cyan #38bdf8

Made for Sharvari Kadam • Indapur, Maharashtra, IN
2026
