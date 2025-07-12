# MAETOPIA – Complete Project Blueprint  
*Single source-of-truth for every designer, developer, and AI assistant working on the project.*

---

## Part 1: The Game Vision – “What We Are Building”

### 1.1 High-Concept
Maetopia is an **interactive world for a 9-year-old** (Maelyn) where city-building is only the beginning. Children craft a vibrant neighbourhood, **enter each building**, decorate cosy interiors, play with animals, and invent their own stories—all through an intuitive, text-light interface designed for touch devices.

### 1.2 Core Experience – Gameplay Loop
```
Build → Enter → Decorate → Interact → Save/Share → Repeat
```
1. **Build the City** – Drag buildings and outdoor items onto a 1920×1080 map.  
2. **Enter Buildings** – Tap a building to transition inside.  
3. **Decorate Interiors** – Place furniture, toys, décor.  
4. **Interact with Characters/Animals** – Feed pets, trigger animations, complete tiny tasks.  
5. **Auto-Save & PNG Export** – Progress is stored in Supabase; snapshots can be shared.  
6. **Loop** – Unlock new assets, expand the city, and create imaginative stories.

### 1.3 Game Flow & Screens
```
[Splash] Bear wakes up
   ↓
[Main Menu]
   ├─ New City
   ├─ Load City
   └─ Settings
   ↓
[City Overview (Map)]
   • Place / move buildings & decor
   • Tap 📍 to ENTER → [Building Interior]
   ↓
[Building Interior]
   • Choose Room ▸ Decorate ▸ Interact
   • Back arrow returns to City Overview
```

### 1.4 Detailed Level Breakdown

#### A. City Overview
| Aspect | Details |
|--------|---------|
| Purpose | “Neighbourhood canvas” where the child arranges buildings & outdoor décor. |
| Actions | • **Place Buildings** (House, Shop, School, Hospital)  <br>• **Outdoor Decor** (trees, benches, paths)  <br>• **Drag to Move**  <br>• **Tap Building** → Enter interior |
| Interactions | Points of Interest glow when selected; Bear Mascot gives contextual tips. |

#### B. Building Interiors
| Building | Rooms / Areas | Notes |
|----------|---------------|-------|
| **House 🏡** | Living Room, Kitchen, Bedroom, Bathroom, Backyard | Most early gameplay happens here. |
| **Shop 🛍️** | Display Area, Storage Room, Counter / Checkout | Kids can “stock shelves”. |
| **School 🏫** | Classroom, Cafeteria, Playground, Library | Unlocks educational mini-challenges. |
| **Hospital 🏥** | Waiting Room, Doctor Office, Recovery Room | Animals & characters “get better”. |

#### C. Interior Decoration System
| Category | Examples |
|----------|----------|
| Seating  | Couch, Beanbag, Chair |
| Tables   | Dining, Coffee, Desk |
| Storage  | Shelf, Toy Box, Dresser |
| Décor    | Rug, Lamp, Poster, Curtains |
| Toys & Tech | Blocks, Dollhouse, TV, Game Console |
| Special  | Interactive Piano 🎹, Fairy Lights, Holiday Items |

#### D. Characters & Animals System
- **Animals** (Dog, Cat): Wander, sleep, follow, need feeding.  
- **Human Characters**: Perform daily routines (cook, read, sleep) and express emotions.  
- **🧸 Bear Mascot**: Persistent guide; appears in corner giving tips, dances when tasks are completed.

#### E. Progression & Engagement
```
Start House → decorate 3 rooms
        ↓ unlock Shop
Decorate Shop shelves
        ↓ unlock School
Complete Classroom mini-challenge
        ↓ unlock Hospital
Help 5 patients
        ↓ unlock Park assets
```
**Mini-Challenges (examples):**
1. *Cozy Living Room* – place ≥5 comfort items.  
2. *Pet Paradise* – set up perfect animal space.  
3. *Birthday Party* – decorate with balloons & cake.

#### F. Future Features (Stretch Goals)
Story Mode • Day/Night Cycle • Weather • Sound Design • Photo Mode • Emotion System • Multi-touch zoom • Device shake to clear toys.

---

## Part 2: The Asset Kit – “The Visual Language”

### 2.1 Core Visual Assets

| Category | Size & Format | Notes |
|----------|---------------|-------|
| **Map Backgrounds** | 1920×1080 PNG/WebP | `downtown-v1.webp`, `suburb-v1.webp`, `park-v1.webp` |
| **POI Markers** | 64×64 SVG | Hospital cross, 