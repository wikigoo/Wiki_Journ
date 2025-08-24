# **Professional Text-to-Image Prompt System for Iranian News Agency**

## **Table of Contents**

1. [System Architecture and Core Principles](#1.-system-architecture-and-core-principles)  
2. [Platform Configuration Guide](#2.-platform-configuration-guide)  
3. [Content Category Templates](#3.-content-category-templates)  
4. [Visual Style Frameworks](#4.-visual-style-frameworks)  
5. [Cultural Sensitivity and Compliance](#5.-cultural-sensitivity-and-compliance)  
6. [Quality Assurance and Optimization](#6.-quality-assurance-and-optimization)  
7. [Implementation Workflow](#7.-implementation-workflow)

---

## **1\. System Architecture and Core Principles** {#1.-system-architecture-and-core-principles}

### **Universal Prompt Formula**

Every effective prompt follows this hierarchical structure:

\[STYLE DECLARATION\] \+ \[SUBJECT/SCENE\] \+ \[COMPOSITION\] \+ \[LIGHTING\] \+ \[TECHNICAL SPECS\] \+ \[CULTURAL CONTEXT\]

**Component Breakdown:**

- **Style Declaration (10%)**: Artistic approach and medium  
- **Subject/Scene (30%)**: Primary content and action  
- **Composition (20%)**: Framing, perspective, and arrangement  
- **Lighting (15%)**: Illumination style and mood  
- **Technical Specs (15%)**: Quality, resolution, format  
- **Cultural Context (10%)**: Sensitivity and authenticity markers

### **Core Quality Principles**

**Professional Standards:**

- **Accuracy**: Factual and culturally authentic representation  
- **Clarity**: Clear communication of intended message  
- **Efficiency**: Optimized for 1-2 day production deadlines  
- **Compliance**: Adherent to Iranian media standards  
- **Versatility**: Adaptable across multiple AI platforms

---

## **2\. Platform Configuration Guide** {#2.-platform-configuration-guide}

### **DALL-E 3 Configuration**

**Strengths**: Natural language processing, content safety, text integration **Best For**: News graphics, social media content, quick turnaround

**Optimization Settings:**

Approach: Conversational and descriptive

Style: "Professional news photography" or "Editorial illustration"

Quality Boosters: "8K resolution, professional photography standards"

Safety: Built-in content filtering for public figures

Text Integration: "Include readable Persian text: \[specific text\]"

**Template Structure for DALL-E 3:**

"Professional \[style\] showing \[subject\] in \[setting\], \[composition details\], \[lighting description\], photographed with \[camera specs\], \[cultural context\], high resolution, news quality"

### **Leonardo AI Configuration**

**Strengths**: PhotoReal mode, canvas editing, preset styles **Best For**: Cinematic content, video covers, artistic content

**Recommended Settings:**

Model: Phoenix or Leonardo Diffusion XL

PhotoReal: Enable for documentary content

Alchemy: Enable for enhanced quality

Guidance Scale: 7-12 (7 for creative, 12 for precise)

Elements: Add relevant style elements

Negative Prompt: "low quality, amateur, inappropriate"

**Template Structure for Leonardo:**

\[Style element\], \[detailed subject description\], \[environmental context\], \[lighting specifics\], \[emotional tone\], professional quality, \[aspect ratio\]

### **Stable Diffusion 3.5 Configuration**

**Strengths**: Maximum control, custom models, negative prompting **Best For**: High-quality production, batch generation, custom styles

**Technical Parameters:**

Sampler: DPM++ 2M Karras

Steps: 25-35 (journalism), 40-50 (artistic)

CFG Scale: 7-9 (balanced), 10-12 (strict adherence)

Resolution: 1024x1024 base, upscale to 2048x2048

Negative Prompt: \[Comprehensive quality control\]

**Advanced Features:**

- **ControlNet**: For composition control  
- **LoRA Models**: For specific artistic styles  
- **Inpainting**: For corrections and refinements

### **Flux/Imagine-AI Configuration**

**Strengths**: Fast generation, good prompt understanding **Best For**: Rapid prototyping, concept development

**Settings:**

Model: Flux.1-dev or Schnell

Steps: 20-30

Guidance: 3.5-7

Aspect Ratio: Custom based on need

Quality: High

---

## **3\. Content Category Templates** {#3.-content-category-templates}

### **3.1 News and Media Content**

#### **YouTube Video Covers (16:9)**

**Template A \- Political Coverage:**

"Professional news photography showing \[political figure/event\] in \[official setting\], dynamic composition with subject positioned on left third, dramatic studio lighting with soft shadows, shot with 85mm lens creating shallow depth of field, serious authoritative mood, Persian governmental context, ultra-high resolution 16:9 format, broadcast quality"

**Template B \- Economic/Social Issues:**

"Documentary style photograph of \[economic subject/social scene\], wide establishing shot showing environmental context, natural daylight illumination, multiple depth layers with foreground elements, journalistic authenticity, Iranian cultural setting, professional news standards, 16:9 cinematic composition"

#### **Instagram Reels/Stories (9:16)**

**Template:**

"Vertical mobile-optimized composition showing \[subject\] in \[context\], centered subject with strong background contrast, portrait lighting setup, bold visual hierarchy for small screen viewing, engaging eye contact or action, culturally appropriate Iranian setting, high contrast colors, 9:16 aspect ratio, social media optimized"

#### **Educational Explainer Graphics**

**Template:**

"Clean infographic style illustration of \[concept\], minimalist design with clear visual hierarchy, educational color palette (blues and greens), professional typography integration space, balanced composition with icons and symbols, Persian cultural elements subtly integrated, high clarity for digital display, informative and accessible design"

### **3.2 Cultural and Religious Content**

#### **Shiite Religious Imagery**

**Template A \- Ceremonial Events:**

"Respectful documentation of \[religious ceremony\] in \[traditional setting\], participants in appropriate religious attire, warm natural lighting creating reverent atmosphere, wide angle showing community participation, cultural authenticity prioritized, traditional Persian Islamic architectural elements, dignified composition respecting religious sensitivities, high quality documentary style"

**Template B \- Symbolic Representation:**

"Sacred symbolic composition featuring \[religious symbols \- Alam, Zuljanah, etc.\], traditional Persian artistic style, rich jewel tones (emerald green, deep blue, gold), symbolic rather than literal representation, respectful treatment of religious themes, traditional Islamic geometric patterns, spiritual atmosphere with divine light effects, cultural heritage preservation quality"

#### **Iranian Cultural Heritage**

**Template:**

"Authentic Persian cultural scene showing \[cultural element\], traditional Iranian artistic style, rich heritage colors reflecting regional traditions, environmental storytelling through architectural details, celebration of Iranian identity, historical accuracy in costume and setting, warm natural lighting, cultural pride and dignity, museum exhibition quality"

#### **Historical Figures**

**Template:**

"Historically accurate representation of \[historical period/context\], figure shown in silhouette or from behind maintaining dignity, authentic period clothing and architectural setting, dramatic lighting suggesting historical significance, Persian miniature painting influence, symbolic elements representing historical importance, respectful artistic interpretation, educational value prioritized"

---

## **4\. Visual Style Frameworks** {#4.-visual-style-frameworks}

### **4.1 Hyperrealistic Style**

**Core Formula:**

"Hyperrealistic \[subject\] with ultra-detailed surface textures, professional photography lighting, every material showing authentic wear patterns, realistic skin texture with natural imperfections, precise fabric weave detail, environmental elements with photographic accuracy, shot with professional DSLR camera, studio lighting setup, 8K resolution, photojournalistic quality"

**Enhancement Keywords:**

- "Ultra-detailed surface textures"  
- "Photographic accuracy"  
- "Professional DSLR quality"  
- "Realistic material properties"  
- "Natural lighting physics"

### **4.2 Cinematic Style**

**Core Formula:**

"Cinematic \[subject\] with dramatic movie lighting, epic composition using rule of thirds, color grading with \[warm/cool\] tones, depth of field creating professional film look, atmospheric haze and lens flares, shot with anamorphic lens, Hollywood production values, epic scale and grandeur, movie poster quality, 16:9 widescreen format"

**Enhancement Keywords:**

- "Cinematic lighting"  
- "Anamorphic lens"  
- "Color grading"  
- "Epic composition"  
- "Film production quality"

### **4.3 Photography Style**

**Portrait Photography:**

"Professional portrait of \[subject\] with three-point lighting setup, shallow depth of field isolating subject, natural expression and posture, professional headshot quality, studio or environmental portrait setting, appropriate cultural context, expert photography techniques, commercial portrait standards"

**Documentary Photography:**

"Documentary photograph capturing \[scene\] with authentic candid moment, natural available lighting, environmental storytelling, photojournalistic integrity, real-world authenticity, unposed natural behavior, cultural sensitivity, Pulitzer Prize photography quality"

### **4.4 Realistic Style**

**Core Formula:**

"Realistic \[subject\] with natural proportions and accurate details, balanced lighting without dramatic effects, authentic materials and textures, true-to-life colors and shading, practical everyday setting, honest representation without artistic exaggeration, clean professional presentation, high quality realistic rendering"

### **4.5 Pixar/Disney Style**

**Core Formula:**

"Pixar animation style \[subject\] with smooth 3D rendering, bright cheerful colors, exaggerated but appealing character design, friendly facial expressions, soft rounded features, magical atmosphere with warm lighting, family-friendly content, high-quality 3D animation, Disney/Pixar production standards"

**Cultural Adaptation:**

"Persian-inspired Pixar style characters wearing traditional Iranian clothing, Middle Eastern architectural backgrounds, warm desert color palette, respectful cultural representation suitable for Iranian children, Islamic artistic sensibilities maintained"

### **4.6 Sticker/Graffiti Style**

**Core Formula:**

"Bold graphic sticker design of \[subject\] with thick black outlines, vibrant flat colors, simplified iconic form, street art aesthetics, spray paint texture effects, urban artistic style, high contrast design readable at small sizes, vector art quality, contemporary graphic design"

---

## **5\. Cultural Sensitivity and Compliance** {#5.-cultural-sensitivity-and-compliance}

### **Iranian Media Standards Checklist**

**Religious Content:**

- ✅ No direct facial depiction of religious figures  
- ✅ Respectful symbolic representation  
- ✅ Appropriate religious dress codes  
- ✅ Cultural authenticity in architectural elements  
- ✅ Dignified treatment of sacred themes

**Political Content:**

- ✅ Neutral diplomatic representation  
- ✅ Appropriate formal protocols  
- ✅ Balanced international coverage  
- ✅ Professional governmental settings  
- ✅ Respectful leadership portrayal

**Social Content:**

- ✅ Family-appropriate imagery  
- ✅ Cultural diversity representation  
- ✅ Progressive while traditional balance  
- ✅ Educational value prioritized  
- ✅ Community dignity maintained

### **Universal Negative Prompts by Category**

**Quality Control:**

"low quality, blurry, pixelated, amateur, distorted, watermark, signature, text artifacts, jpeg compression, low resolution, bad anatomy, deformed"

**Cultural Sensitivity:**

"inappropriate religious content, disrespectful portrayal, western stereotypes, orientalist clichés, culturally insensitive elements, anachronistic elements"

**Professional Standards:**

"unprofessional, casual snapshot, poor lighting, bad composition, cluttered background, distracting elements, off-brand"

---

## **6\. Quality Assurance and Optimization** {#6.-quality-assurance-and-optimization}

### **Pre-Generation Checklist**

**Content Planning:**

- [ ] Clear objective defined  
- [ ] Target audience identified  
- [ ] Cultural context considered  
- [ ] Platform requirements noted  
- [ ] Style approach selected

**Technical Preparation:**

- [ ] Appropriate AI platform chosen  
- [ ] Template selected and customized  
- [ ] Parameters optimized  
- [ ] Negative prompts prepared  
- [ ] Quality standards defined

### **Post-Generation Evaluation**

**Technical Quality:**

- [ ] Resolution meets requirements  
- [ ] Composition professionally executed  
- [ ] Lighting appropriate for content  
- [ ] Color accuracy maintained  
- [ ] No visible artifacts or distortions

**Content Accuracy:**

- [ ] Cultural elements authentic  
- [ ] Religious sensitivity maintained  
- [ ] Historical accuracy verified  
- [ ] Brand guidelines followed  
- [ ] Message clearly communicated

**Platform Optimization:**

- [ ] Aspect ratio correct  
- [ ] File size appropriate  
- [ ] Format suitable for intended use  
- [ ] Color space optimized  
- [ ] Metadata properly tagged

### **Iteration Strategy**

**First Generation (Concept):**

- Use simplified prompt for basic composition  
- Focus on overall layout and style  
- Generate 3-5 variations quickly

**Second Generation (Refinement):**

- Enhance best concept with detailed descriptors  
- Add specific cultural and technical elements  
- Fine-tune composition and lighting

**Final Generation (Polish):**

- Perfect selected version with highest quality settings  
- Apply post-processing if needed  
- Optimize for final delivery format

---

## **7\. Implementation Workflow** {#7.-implementation-workflow}

### **Daily Workflow Integration**

**Morning Setup (15 minutes):**

1. Review day's content requirements  
2. Select appropriate templates  
3. Prepare platform-specific settings  
4. Queue generation tasks by priority

**Content Production (45-90 minutes per item):**

1. **Analysis** (10 min): Define requirements and select template  
2. **Generation** (20-40 min): Create multiple variations  
3. **Selection** (10 min): Choose best results  
4. **Refinement** (15-30 min): Enhance and optimize  
5. **Review** (10 min): Quality check and approval

**Batch Processing Strategy:**

- Group similar content types together  
- Use consistent settings within batches  
- Maintain template library for quick access  
- Document successful approaches

### **Emergency/Breaking News Protocol**

**30-Minute Turnaround:**

1. Use DALL-E 3 for fastest generation  
2. Apply pre-tested breaking news template  
3. Focus on single strong concept  
4. Minimal post-processing  
5. Quick cultural sensitivity check

**Template for Breaking News:**

"Breaking news style photograph of \[event/situation\] in \[location\], urgent journalistic documentation, professional news photography, dramatic natural lighting, serious authoritative mood, Iranian news standards, broadcast quality, immediate news value"

### **Quality Control Documentation**

**Success Metrics Tracking:**

- Generation time vs. quality achieved  
- Cultural accuracy assessment scores  
- Audience engagement on published content  
- Platform performance analytics  
- Feedback from editorial team

**Continuous Improvement:**

- Weekly review of generated content  
- Template refinement based on results  
- Platform performance comparison  
- Cultural consultant feedback integration  
- Technology advancement adoption

---

## **Template Quick Reference Library**

### **Copy-Paste Ready Templates**

**Political News (16:9):**

Professional news photography of \[political subject\] in \[governmental setting\], authoritative composition with dramatic studio lighting, official Iranian governmental context, broadcast journalism quality, 16:9 aspect ratio

**Cultural Event (1:1):**

Documentary photograph of \[Iranian cultural celebration\] with authentic traditional elements, warm natural lighting, respectful cultural representation, community celebration atmosphere, social media optimized square format

**Religious Content:**

Respectful symbolic representation of \[religious theme\] in traditional Persian artistic style, sacred atmosphere with divine lighting, cultural authenticity prioritized, Islamic artistic sensibilities, spiritual reverence maintained

**Educational Content:**

Clean educational illustration explaining \[concept\], minimalist design with clear visual hierarchy, professional color palette, Iranian educational context, high clarity for digital learning platforms

**Breaking News:**

Urgent news photography documenting \[breaking situation\], immediate journalistic value, dramatic natural lighting, serious news atmosphere, professional broadcast standards, Iranian media compliance

---

## **8\. Troubleshooting and Debugging Guide**

### **8.1 Common Generation Issues and Solutions**

#### **Problem: Poor Image Quality**

**Symptoms:**

- Blurry or pixelated outputs  
- Low detail resolution  
- Artificial or fake-looking results  
- Poor lighting and composition

**Debugging Steps:**

1. **Check Platform Settings:**  
     
   DALL-E 3: Add "8K resolution, professional photography, ultra-detailed"  
     
   Leonardo AI: Enable Alchemy \+ PhotoReal, set Guidance to 10+  
     
   Stable Diffusion: Increase steps to 35+, CFG scale 8-10  
     
   Flux: Set quality to High, increase guidance to 7  
     
2. **Enhance Prompt Structure:**  
     
   Add: "professional photography, studio lighting, high resolution"  
     
   Add: "masterpiece quality, award-winning photography"  
     
   Add: "ultra-detailed, sharp focus, perfect composition"  
     
3. **Improve Negative Prompts:**  
     
   "low quality, blurry, pixelated, amateur, distorted, bad anatomy,   
     
   worst quality, jpeg artifacts, watermark, signature"

#### **Problem: Culturally Inappropriate Content**

**Symptoms:**

- Western stereotypes in Iranian/Islamic content  
- Inappropriate religious representations  
- Culturally insensitive elements  
- Anachronistic details

**Debugging Steps:**

1. **Strengthen Cultural Context:**  
     
   Add: "authentic Iranian culture, respectful Islamic representation"  
     
   Add: "traditional Persian aesthetics, cultural authenticity"  
     
   Add: "appropriate religious sensitivity, dignified portrayal"  
     
2. **Use Specific Cultural Markers:**  
     
   Architecture: "Persian Islamic architecture, traditional Iranian design"  
     
   Clothing: "authentic Middle Eastern attire, culturally appropriate dress"  
     
   Context: "Iranian cultural setting, Persian cultural elements"  
     
3. **Apply Cultural Negative Prompts:**  
     
   "western stereotypes, orientalist clichés, inappropriate religious content,   
     
   cultural insensitivity, anachronistic elements, disrespectful portrayal"

#### **Problem: Inconsistent Results Across Platforms**

**Symptoms:**

- Same prompt produces different quality on different platforms  
- Style inconsistency between generations  
- Unpredictable output quality

**Debugging Steps:**

1. **Platform-Specific Optimization:**  
     
   DALL-E 3: Use natural, descriptive language  
     
   Leonardo AI: Add specific style elements  
     
   Stable Diffusion: Use technical parameters and negative prompts  
     
   Flux: Keep prompts clear and concise  
     
2. **Standardize Quality Markers:**  
     
   Universal: "professional quality, high resolution, masterpiece"  
     
   Add platform-specific quality boosters from Section 2  
     
3. **Test and Document:**  
     
   \- Generate same concept on all platforms  
     
   \- Document which platform works best for each content type  
     
   \- Create platform-specific template variations

### **8.2 Platform-Specific Troubleshooting**

#### **DALL-E 3 Issues**

**Issue: Content Policy Blocks**

Solution: Rephrase sensitive terms

Replace: "battle, war, violence" → "historical event, commemoration"

Replace: "martyrdom" → "sacrifice, devotion"

Add: "artistic representation, cultural documentation"

**Issue: Text Generation Problems**

Solution: Be specific about text requirements

Add: "readable Persian text saying '\[exact text\]'"

Add: "clear calligraphy, legible text, professional typography"

#### **Leonardo AI Issues**

**Issue: PhotoReal Mode Not Working**

Check: Model compatibility (Phoenix works best with PhotoReal)

Settings: Enable both Alchemy and PhotoReal

Prompt: Add "photorealistic, professional photography"

**Issue: Style Inconsistency**

Use Elements: Add specific style elements from library

Fix Guidance: Set to 10-12 for better prompt adherence

Add Keywords: "consistent style, unified aesthetic"

#### **Stable Diffusion Issues**

**Issue: Anatomy Problems**

Negative Prompt: "bad anatomy, deformed, mutated, extra limbs, 

malformed hands, poorly drawn face"

Parameters: Increase CFG scale to 10-12

Add: "correct anatomy, natural proportions, realistic human form"

**Issue: Style Mixing**

Strengthen Style: Use (style:1.3) weighting

Negative: "mixed styles, inconsistent art style, style confusion"

LoRA: Use specific style LoRAs for consistency

#### **Flux Issues**

**Issue: Poor Prompt Understanding**

Simplify: Use clear, direct language

Structure: Subject \+ action \+ style \+ quality

Avoid: Complex artistic terminology

### **8.3 Content-Specific Debugging**

#### **News Content Issues**

**Problem: Not Professional Enough**

Add: "professional journalism, news photography standards"

Add: "broadcast quality, editorial photography"

Settings: Use higher quality settings on all platforms

**Problem: Poor Mobile Optimization**

Composition: "mobile-optimized, clear subject focus"

Contrast: "high contrast, bold visual hierarchy"

Simplify: Reduce background complexity

#### **Religious Content Issues**

**Problem: Inappropriate Religious Representation**

Template: Use symbolic representation templates from Section 3.2

Add: "respectful symbolic representation, no direct depiction"

Cultural Review: Always run through cultural compliance checklist

**Problem: Historical Inaccuracy**

Research: Verify historical details before generation

Add: "historically accurate, authentic period details"

Consult: Check with cultural experts for sensitive content

### **8.4 Quality Improvement Protocols**

#### **Iterative Enhancement Process**

**Step 1: Diagnostic Analysis**

1\. Identify specific quality issues

2\. Check against quality standards checklist

3\. Determine if issue is technical or content-related

4\. Select appropriate debugging approach

**Step 2: Systematic Testing**

1\. Apply one fix at a time

2\. Test on same prompt to isolate variables

3\. Document what works and what doesn't

4\. Build successful approach into template

**Step 3: Template Refinement**

1\. Update templates based on successful fixes

2\. Add successful phrases to enhancement keywords

3\. Update negative prompts with problem preventers

4\. Document platform-specific optimizations

#### **Emergency Fixes for Deadline Pressure**

**30-Second Fixes:**

Quality: Add "professional, high quality, masterpiece"

Detail: Add "ultra-detailed, sharp focus"

Style: Add "professional photography" or relevant style

**2-Minute Fixes:**

Platform Switch: Try different AI platform

Template Switch: Use proven template from library

Parameter Adjustment: Apply known good settings

**5-Minute Fixes:**

Complete Rewrite: Start with proven template

Research: Quick check of successful similar content

Platform Optimization: Apply full platform-specific settings

### **8.5 Prevention Strategies**

#### **Pre-Generation Prevention**

**Quality Prevention Checklist:**

- [ ] Appropriate platform selected for content type  
- [ ] Template tested and proven for similar content  
- [ ] Cultural elements verified for appropriateness  
- [ ] Technical parameters optimized for platform  
- [ ] Negative prompts comprehensive and updated

**Cultural Prevention Checklist:**

- [ ] Religious sensitivity requirements reviewed  
- [ ] Iranian cultural elements authenticated  
- [ ] Historical accuracy verified where applicable  
- [ ] International representation balanced and respectful  
- [ ] Community standards compliance confirmed

#### **Documentation and Learning**

**Issue Tracking:**

Problem: \[Specific issue description\]

Platform: \[AI platform used\]

Prompt: \[Original prompt that failed\]

Solution: \[What fixed the issue\]

Prevention: \[How to avoid in future\]

**Success Pattern Documentation:**

Content Type: \[News/Religious/Cultural\]

Working Template: \[Successful template used\]

Platform Settings: \[Optimal configuration\]

Quality Markers: \[Effective enhancement keywords\]

Notes: \[Special considerations or tips\]

---

