# Faster Research - Instructions

## What are Traits

**Traits** are species characteristics in Stellaris. When creating a new empire:

1. **Choose species portrait** →
2. **Choose traits** (e.g., "Intelligent", "Strong", "Quick") →
3. **These traits provide bonuses** to the entire species

### Standard traits in the game:
- `trait_intelligent` - Intelligent (+10% research speed)
- `trait_natural_physicists` - Natural Physicists (physicists produce +15% research)
- `trait_strong` - Strong (workers +20% output)

## The mod adds 2 ways to speed up research:

### Method 1: Traits - for new empires or with genetic modification

3 new species traits:

### 1. Quick Research (trait_QuickResearch_1)
```
country_engineering_tech_research_speed = 1.00  (100%)
country_physics_tech_research_speed = 1.00
country_society_tech_research_speed = 1.00
```
**What this means:** Technologies are researched **2x faster**

### 2. Very Quick Research (trait_QuickResearch_2)
```
country_engineering_tech_research_speed = 8.00  (800%)
country_physics_tech_research_speed = 8.00
country_society_tech_research_speed = 8.00
```
**What this means:** Technologies are researched **9x faster**

### 3. Instant Research (trait_UltraResearch)
```
all_technology_research_speed = 25.00  (2500%)
```
**What this means:** Technologies are researched **26x faster** (almost instantly)

### Method 2: Edicts - for current games ⭐ RECOMMENDED

3 edicts that can be activated at any time:

#### 1. mod – Quick Research Program
```
Cost: 10 energy (upfront) + 10 energy/month
Effect: Technologies are researched 2x faster
```

#### 2. mod – Very Quick Research Program
```
Cost: 10 energy (upfront) + 10 energy/month
Effect: Technologies are researched 9x faster
```

#### 3. mod – Instant Research Program
```
Cost: 10 energy (upfront) + 10 energy/month
Effect: Technologies are researched 26x faster
```

**How to activate an edict:**
1. Open the **"Government"** tab - crown icon in the top panel
2. Click **"Edicts & Campaigns"**
3. Find the desired research program
4. Click **"Activate"**
5. The edict works permanently until you disable it or run out of energy

## Where does this work?

This affects the **"Technology"** tab (flask button in the top panel):

```
[Physics]    [Society]    [Engineering]
    ⬇️            ⬇️            ⬇️
Technology   Technology   Technology
50 days      50 days      50 days
remaining    remaining    remaining
```

With the `trait_UltraResearch` trait:
- Instead of 50 days → **2 days**
- Instead of 1000 days → **40 days**

## How to use the mod:

### ⭐ Option 1: EDICTS (for current games - easiest way!)

1. **Launch Stellaris** with the mod enabled
2. **Load your current game**
3. **Open the "Government" menu** (crown icon at the top)
4. **Click "Edicts & Campaigns"**
5. **Find and activate** the desired research program
6. **Done!** Technologies now research faster

**Advantages:**
- ✅ Works in current games
- ✅ No research required
- ✅ Can be toggled on/off
- ✅ Cheap cost (10 energy)

### Option 2: Traits (for new empire)

1. **Launch Stellaris**
2. **Enable the mod** in the launcher (check "Faster Research")
3. **Create a new game** → "New Empire"
4. **On the species selection screen:**
   - Go to the **"Traits"** tab
   - Find the **"Quick Research"**, **"Very Quick Research"**, or **"Instant Research"** trait
   - **Add it to the species** (click on it)
5. Start the game - technologies will research very quickly!

### Option 3: Traits in current game (with genetic modification)

If the game has already started:
1. Research the **"Gene Tailoring"** technology
2. Open the **"Species"** screen
3. Select your species → **"Modify Template"**
4. **Add the trait** "Quick Research"
5. Apply to population

## Difference between modifiers:

### `country_engineering_tech_research_speed`
- Affects **ONLY engineering technologies**
- Speeds up research for specific branch

### `all_technology_research_speed`
- Affects **ALL technologies at once** (physics + society + engineering)
- Simpler and more efficient

## Technical Information

### Mod structure:
```
my_research/
├── descriptor.mod
├── common/
│   ├── edicts/00_faster_research_edicts.txt
│   └── traits/00_faster_research_traits.txt
└── localisation/
    ├── english/faster_research_l_english.yml
    ├── russian/faster_research_l_russian.yml
    └── simp_chinese/faster_research_l_simp_chinese.yml
```

### Supported versions:
- Stellaris 4.1.3+

### Compatibility:
- Works with all species types: BIOLOGICAL, MACHINE, LITHOID, ROBOT
- Does not conflict with other mods

### Supported languages:
- ✅ English
- ✅ Русский (Russian)
- ✅ 简体中文 (Simplified Chinese)
