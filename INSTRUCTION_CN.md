# 快速研究 - 使用说明

## 什么是特性（Traits）

**特性（Traits）**是群星（Stellaris）中的物种特征。创建新帝国时：

1. **选择物种肖像** →
2. **选择特性**（例如"聪慧"、"强壮"、"敏捷"）→
3. **这些特性为整个物种提供加成**

### 游戏中的标准特性：
- `trait_intelligent` - 聪慧（研究速度 +10%）
- `trait_natural_physicists` - 天生物理学家（物理学家产出 +15%）
- `trait_strong` - 强壮（工人产出 +20%）

## 本模组添加了2种加速研究的方法：

### 方法1：特性 - 用于新帝国或基因改造

3个新物种特性：

### 1. 快速研究（trait_QuickResearch_1）
```
country_engineering_tech_research_speed = 1.00  (100%)
country_physics_tech_research_speed = 1.00
country_society_tech_research_speed = 1.00
```
**效果：**技术研究速度提高**2倍**

### 2. 超快速研究（trait_QuickResearch_2）
```
country_engineering_tech_research_speed = 8.00  (800%)
country_physics_tech_research_speed = 8.00
country_society_tech_research_speed = 8.00
```
**效果：**技术研究速度提高**9倍**

### 3. 瞬时研究（trait_UltraResearch）
```
all_technology_research_speed = 25.00  (2500%)
```
**效果：**技术研究速度提高**26倍**（几乎瞬间完成）

### 方法2：法令 - 用于当前游戏 ⭐ 推荐

可随时激活的3个法令：

#### 1. 模组 – 快速研究计划
```
费用：10能量币（一次性）+ 每月10能量币
效果：技术研究速度提高2倍
```

#### 2. 模组 – 超快速研究计划
```
费用：10能量币（一次性）+ 每月10能量币
效果：技术研究速度提高9倍
```

#### 3. 模组 – 瞬时研究计划
```
费用：10能量币（一次性）+ 每月10能量币
效果：技术研究速度提高26倍
```

**如何激活法令：**
1. 打开**"政府"**选项卡 - 顶部面板中的王冠图标
2. 点击**"法令与运动"**
3. 找到所需的研究计划
4. 点击**"激活"**
5. 法令将持续生效，直到你关闭它或能量币耗尽

## 在哪里生效？

这会影响**"科技"**选项卡（顶部面板中的烧瓶按钮）：

```
[物理学]      [社会学]      [工程学]
   ⬇️            ⬇️            ⬇️
科技研究      科技研究      科技研究
剩余50天      剩余50天      剩余50天
```

使用 `trait_UltraResearch` 特性后：
- 50天 → **2天**
- 1000天 → **40天**

## 如何使用模组：

### ⭐ 方案1：法令（用于当前游戏 - 最简单的方式！）

1. **启动群星**并启用模组
2. **加载当前游戏**
3. **打开"政府"菜单**（顶部的王冠图标）
4. **点击"法令与运动"**
5. **找到并激活**所需的研究计划
6. **完成！**现在技术研究速度更快了

**优点：**
- ✅ 适用于当前游戏
- ✅ 不需要研究科技
- ✅ 可以开关
- ✅ 成本低廉（10能量币）

### 方案2：特性（用于新帝国）

1. **启动群星**
2. **在启动器中启用模组**（勾选"Faster Research"）
3. **创建新游戏** → "新帝国"
4. **在物种选择界面：**
   - 进入**"特性"**选项卡
   - 找到**"快速研究"**、**"超快速研究"**或**"瞬时研究"**特性
   - **将其添加到物种**（点击它）
5. 开始游戏 - 技术将快速研究！

### 方案3：在当前游戏中使用特性（通过基因改造）

如果游戏已经开始：
1. 研究**"基因剪裁"**（Gene Tailoring）科技
2. 打开**"物种"**界面
3. 选择你的物种 → **"修改模板"**
4. **添加特性** "快速研究"
5. 应用到人口

## 修正器之间的区别：

### `country_engineering_tech_research_speed`
- **仅影响工程学科技**
- 加速特定分支的研究

### `all_technology_research_speed`
- **同时影响所有科技**（物理学 + 社会学 + 工程学）
- 更简单、更高效

## 技术信息

### 模组结构：
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

### 支持版本：
- 群星 4.1.3+

### 兼容性：
- 适用于所有物种类型：BIOLOGICAL（生物）、MACHINE（机械）、LITHOID（岩石）、ROBOT（机器人）
- 不与其他模组冲突

### 支持语言：
- ✅ English（英语）
- ✅ Русский（俄语）
- ✅ 简体中文
